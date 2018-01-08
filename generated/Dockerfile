FROM buildpack-deps:jessie as xar_builder

ENV XAR_VERSION "1.6.1"
USER root

WORKDIR /tmp

# Build xar
ADD https://github.com/downloads/mackyle/xar/xar-$XAR_VERSION.tar.gz .
RUN tar -xzf xar-$XAR_VERSION.tar.gz \
	&& mv xar-$XAR_VERSION xar \
	&& cd xar \
	&& ./autogen.sh --noconfigure \
	&& ./configure \
	&& make 


###############
# Final image #
###############
FROM circleci/ruby:latest
MAINTAINER milch

ENV PATH $PATH:/usr/local/itms/bin

# Java versions to be installed
ENV JAVA_VERSION 8u131
ENV JAVA_DEBIAN_VERSION 8u131-b11-1~bpo8+1
ENV CA_CERTIFICATES_JAVA_VERSION 20161107~bpo8+1

# Needed for fastlane to work
ENV LANG C.UTF-8
ENV LC_ALL C.UTF-8

# Required for iTMSTransporter to find Java
ENV JAVA_HOME /usr/lib/jvm/java-8-openjdk-amd64/jre

USER root

# iTMSTransporter needs java installed
# We also have to install make to install xar
# And finally shellcheck
RUN echo 'deb http://deb.debian.org/debian jessie-backports main' > /etc/apt/sources.list.d/jessie-backports.list \
	&& apt-get update \
	&& apt-get install --yes \
		make \
		shellcheck \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*

USER circleci

COPY --from=xar_builder /tmp/xar /tmp/xar

RUN cd /tmp/xar \
	&& sudo make install \
	&& sudo rm -rf /tmp/*
