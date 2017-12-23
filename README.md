# fastlane-docker

fastlane tools docker image based on CircleCI's ruby image. Used to run the fastlane test suite on Linux.

The script in this repo's Dockerfile automatically accepts these terms for the iTMSTransporter installer below: 

> APPLE, INC.
> SOFTWARE LICENSE AGREEMENT FOR
> ITMSTRANSPORTER
> 
> PLEASE READ THIS SOFTWARE LICENSE AGREEMENT ("AGREEMENT") BEFORE USING THE SOFTWARE.  BY USING THE SOFTWARE, YOU ARE AGREEING TO BE BOUND BY THE TERMS OF THIS AGREEMENT.  IF YOU WOULD LIKE TO RECEIVE APPLE SOFTWARE PURSUANT TO THIS AGREEMENT, SIGNIFY YOUR AGREEMENT TO BE BOUND BY THE TERMS OF THIS AGREEMENT BY CLICKING THE "AGREE/ACCEPT" BUTTON. IF YOU DO NOT AGREE TO THE TERMS OF THIS LICENSE, CLICK "DISAGREE/DECLINE".
> 
> IMPORTANT NOTE: This software may be used to reproduce materials.  It is licensed to you only for reproduction of non-copyrighted materials, materials in which you own the copyright, or materials you are authorized or legally permitted to reproduce.  If you are uncertain about your right to copy any material you should contact your legal advisor. 
> 
> 1.	Definitions
> 
> 1.1	"Apple" means Apple, Inc. and/or any of its affiliates responsible for operating the iTunes Store in various territories.
> 
> 1.2	"Apple Software" means the iTMSTransporter software, including any and all technologies therein, provided by Apple to Licensee. 
> 
> 1.3	"iTunes Store Agreement" means an agreement with Apple for the provision of materials to Apple for distribution via Apple's iTunes Store.  
> 
> 1.4	"Licensee" means the entity that has received the Apple Software and agreed to be bound by the terms of this Agreement.  Licensee must be, and by accepting this Agreement represents and warrants that it is, either (a) a party to the iTunes Store Agreement with Apple pursuant to which Licensee Materials will be provided to Apple using the Apple Software (the "Content Provider"), (b) a corporate affiliate of the Content Provider authorized by the Content Provider to act on the Content Provider's behalf in the delivery of Licensee Materials to Apple ("Authorized Affiliate"), or (c) a third party content delivery entity authorized by the Content Provider pursuant to a written agreement to act on the Content Provider's behalf in the delivery of Licensee Materials to Apple ("Authorized Representative").  Only a Content Provider, Authorized Affiliate or Authorized Representative is licensed to use the Apple Software pursuant to this Agreement.  
> 
> 1.5	"Licensee Materials" means digital audio tracks, digital video, metadata, artwork and other materials to be provided to Apple pursuant to an iTunes Store Agreement.
> 
> 2.	License to Apple Software 
> 
> Subject to all of the requirements and limitations set forth in this Agreement, Licensee is hereby granted a non-exclusive, non-transferable license to use the Apple Software internally to upload Licensee Materials for the sole purpose of providing Licensee Materials to Apple pursuant to an iTunes Store Agreement.  Except as expressly set forth herein, no other licenses are granted or to be implied pursuant to this Agreement.  
> 
> 3.	License Conditions  
> 
> 3.1	Licensee may copy the Apple Software only for internal use in accordance with this Agreement and may make only as many copies as are necessary in order to deliver Licensee Materials to Apple.  Licensee may not permit any other party to use or copy the Apple Software.
> 
> 3.2	Licensee may not decompile, reverse engineer or disassemble the Apple Software.  
> 
> 3.3	Licensee may not modify, sublicense, rent, lease, lend or distribute the Apple Software and may not create derivative works based upon the Apple Software.
> 
> 3.4	Any use by Licensee of the Apple Software in connection, conjunction or combination with any other software shall be at Licensee's risk and in compliance with any license terms applicable to such other software, and Licensee hereby agrees to indemnify, defend and hold Apple harmless from and against any claim arising from or relating to such use.
> 
> 3.5	Licensee may not use the Apple Software to upload, transmit or distribute content or materials for any purpose other than providing such materials to Apple pursuant to Content Provider's iTunes Store Agreement.
> 
> 3.6	This License will be effective only if the acceptance button is clicked by an authorized representative of Licensee who has the authority to accept this license on behalf of Licensee.  Unless such acceptance by an authorized representative of Licensee has occurred, any use, reproduction, display and/or distribution of the Apple Software is not covered by this license and is prohibited.  The person who clicks the acceptance button for this license agreement represents and warrants that they have the authority to accept this agreement on behalf of Licensee.
> 
> 4.	Term and Termination
> 
> 4.1	Unless terminated earlier in accordance with this Section 4, this Agreement will remain in effect until termination or expiration of Content Provider's iTunes Store Agreement.  
> 
> 4.2	Apple may terminate this Agreement at any time by providing written notice to Licensee.  Termination will become effective immediately upon written notice to Licensee provided in accordance with Section 10 of this Agreement.  Licensee may terminate this Agreement at any time by providing written notice of termination to Apple in accordance with Section 10 of this Agreement, destroying all copies of the Apple Software in its possession or control and providing written assurance of such destruction with the notice of termination.  
> 
> 4.3	This Agreement will automatically terminate if Licensee fails to comply with any term(s) of this Agreement, becomes insolvent, has a receiver appointed, makes an assignment for the benefit of creditors, or becomes the subject of any proceeding under any bankruptcy, insolvency, or debtor's relief law.
> 
> 4.4	Upon any termination or expiration of this Agreement, all rights granted to Licensee herein shall immediately cease and Licensee shall promptly return or destroy all copies of the Apple Software in Licensee's possession and provide written assurance of such return or destruction.  The provisions of Sections 1, 3, 4.4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15 and 16 will survive termination or expiration of this Agreement.  The rights of the parties under this Section 4 are in addition to any other rights and remedies provided by law or under this Agreement.  
> 
> 5.	WARRANTY DISCLAIMER AND LIMITATION OF LIABILITY
> 
> 5.1	Apple licenses the Apple Software to Licensee on an "AS IS" basis.  APPLE MAKES NO WARRANTIES, EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE OR NONINFRINGEMENT, REGARDING THE APPLE SOFTWARE OR ITS USE AND OPERATION ALONE OR IN COMBINATION WITH OTHER SOFTWARE OR HARDWARE.   APPLE DOES NOT WARRANT THAT THE FUNCTIONS CONTAINED IN THE APPLE SOFTWARE WILL MEET PARTICULAR REQUIREMENTS, OR THAT THE OPERATION OF THE APPLE SOFTWARE WILL BE UNINTERRUPTED OR ERROR-FREE, OR THAT DEFECTS IN THE APPLE SOFTWARE WILL BE CORRECTED. 
> 
> 5.2	IN NO EVENT WILL APPLE BE LIABLE FOR SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THIS AGREEMENT, OR ARISING FROM THE USE OF THE APPLE SOFTWARE, WHETHER UNDER THEORY OF CONTRACT, TORT (INCLUDING NEGLIGENCE), PRODUCT LIABILITY OR OTHERWISE, INCLUDING, WITHOUT LIMITATION, LOSS OF PROFITS, LOSS OF DATA, BUSINESS INTERRUPTION OR ANY OTHER COMMERCIAL DAMAGES OR LOSSES. 
> 
> 5.3	IN NO EVENT WILL APPLE'S TOTAL LIABILITY TO LICENSEE FOR ALL DAMAGES, LOSSES, AND CAUSES OF ACTION (WHETHER IN CONTRACT, TORT (INCLUDING NEGLIGENCE) OR OTHERWISE) ARISING OUT OF THIS AGREEMENT OR THE RIGHTS PROVIDED PURSUANT TO THIS AGREEMENT EXCEED $500.
> 
> 5.4	Both parties acknowledge that the disclaimers and limitations of liability set forth herein are an essential element of this Agreement without which Apple would not be willing to enter into this Agreement.  
> 
> 6.	No Indemnification by Apple
> 
> Apple has no obligation to indemnify, defend or hold Licensee harmless from and against any claim that the Apple Software infringes any third party patent, copyright, trademark or other intellectual property right, or any other claim arising out of this Agreement, or relating to the Apple Software.  Licensee will promptly notify Apple of any such claim.    
> 
> 7.	Export
> 
> Licensee agrees to abide by U.S. and other applicable export control laws and not to transfer the Apple Software except as authorized by United States law and the laws of the jurisdiction in which the Apple Software was obtained.  In particular, but without limitation, the Apple Software may not be exported or re-exported (i) into (or to a national or resident of) Cuba, Iran, Iraq, Libya, North Korea, Syria or any other U.S. embargoed country or (ii) to anyone on the U.S. Treasury Department's list of Specially Designated Nationals or the U.S. Department of Commerce's Table of Denial Orders.  Licensee may not knowingly provide the Apple Software to a member located in, under control of, or a national or resident of any such country or on any such list. 
> 
> 8.	Relationship of the Parties
> 
> Neither party may represent or bind the other party in any way and nothing stated in this Agreement will be construed as creating the relationships of joint venturers, partners, employer and employee, franchisor and franchisee, master and servant, or principal and agent.
> 
> 9.	Assignment
> 
> This Agreement will be binding on the assigns, heirs and successors (whether through merger or otherwise) of the parties, except that it may not be assigned by any means, including without limitation, operation of law or merger, by Licensee. Any purported assignment not permitted under this Section will be void.  
> 
> 10.	Notices
> 
> Any notice under this Agreement will be deemed given if notice is provided in accordance with the notice requirements set forth in the Content Provider's iTunes Store Agreement.  
> 
> 11.	CONFIDENTIALITY
> 
> The terms and conditions of this Agreement are confidential and may not be disclosed by Licensee to any third party.
> 
> 12.	Governing Law
> 
> This Agreement will be governed by and construed in accordance with the laws of the State of California as applied to agreements entered into and to be performed entirely within California between California residents.  Any litigation or other dispute resolution between the parties relating to this Agreement will take place in the Northern District of California.  The parties consent to the personal jurisdiction of, and venue in, the state and federal courts within that District.
> 
> 13.	Severability
> 
> If for any reason a court of competent jurisdiction finds any provision of this Agreement, or portion thereof, to be unenforceable, that provision of the Agreement will be enforced to the maximum extent permissible so as to effect the economic benefits and intent of the parties, and the remainder of this Agreement will continue in full force and effect.
> 
> 14.	No Waiver
> 
> No delay, omission or failure to exercise any right or remedy provided for in this Agreement shall be deemed a waiver thereof, nor shall it be deemed to be a waiver of any other or subsequent breach.
> 
> 15.	Government End Users 
> 
> If the Apple Software is supplied to the United States Government, the Apple Software is classified as "restricted computer software" as defined in clause 52.227-19 of the FAR.  The United States Government's rights to the Apple Software are as provided in clause 52.227-19 of the FAR.
> 
> 16.	Complete Agreement
> 
> This Agreement constitutes the entire agreement between the parties with respect to the subject matter set forth herein and supersedes all prior or contemporaneous understandings regarding such subject matter.  No amendment to or modification of this Agreement will be binding unless in writing and signed by Apple.
