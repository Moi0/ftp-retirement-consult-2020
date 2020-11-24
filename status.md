# Working Summary of Community Discussion on Retiring FTP
(last updated per [this message](https://mailarchive.ietf.org/arch/msg/ietf/6nwIcbph4dB9Zujot6oKH_nrkNc/) in the thread; 2020-11-24 1630 GMT-5)

The following is a summary of the feedback in the [Call for Community Feedback: Retiring FTP Service thread](https://mailarchive.ietf.org/arch/msg/ietf/oTleIrHnjuvtEUKjpPXCt4Q31Qw/) on the [IETF Discussion mailing list](https://www.ietf.org/mailman/listinfo/ietf).
* [Proposal](https://www.ietf.org/media/documents/Retiring_IETF_FTP_Service.pdf)
* [FTP Usage Data](https://docs.google.com/document/d/1JAXspeaMWFl8ML3hSezFSM0VsJsHI4uyDlQ2dHip8jo/edit#)

This summary aggregates common questions and concerns, and associated responses with references.  It is not a verbatim transcript of the discussions.  It does not synthesize discussions not directly related to the question of retiring the FTP service.

As this thread consistented of many messages and interleaved ideas, if your position has been misrepresented, please send corrections to the thread on ietf@ietf.org or privately to Roman Danyliw (IESG tool representative).

## Explicitly Stated Positions
The following are pointers to explicitly stated positions (and rationales) on the retirement plan.

* Oppose: [[Ohta]](https://mailarchive.ietf.org/arch/msg/ietf/7Itgz5txNUZATpc5SKRwKLLc-hs/) [[Eckert]](https://mailarchive.ietf.org/arch/msg/ietf/XFJOyi9a8KsrF4vmBAghb0Zo3mo/) 
[[Moore]](https://mailarchive.ietf.org/arch/msg/ietf/mKdnC6vy-E87aj3DbRAMpmsjrQA/) [[Mauch]](https://mailarchive.ietf.org/arch/msg/ietf/Nydu9WAV7OOUDbXTNB6rkH8IIfM/) [[Ned]](https://mailarchive.ietf.org/arch/msg/ietf/RXzbxmpS0kTlbv0iDZNt9vvMMbs/) [[Kulawiec]](https://mailarchive.ietf.org/arch/msg/ietf/j0vrAvb_baoo11tdET5romkRi8c/)

* Support: [[Housley]](https://mailarchive.ietf.org/arch/msg/ietf/RS85sbnQKUIixjL8LNDdnuRqpbI/) [[Eggert]](https://mailarchive.ietf.org/arch/msg/ietf/pb7PmZ67Mhlr2GencT1YAk42OwY/) [[Roach]](https://mailarchive.ietf.org/arch/msg/ietf/Sos9vi8ZQ37PLA8M1VDKqFPZuPE/) [[Migault]](https://mailarchive.ietf.org/arch/msg/ietf/JOOdTgOySn6j-SSJMQCXtnLmTDU/) [[Turner]](https://mailarchive.ietf.org/arch/msg/ietf/ALo7nFk4NyMkpfHhDhh-Pn5duzM/) [[Leymann]](https://mailarchive.ietf.org/arch/msg/ietf/sQF1SUIYZVXqiPDRE1pEHS8WQZM/) [[Livingood]](https://mailarchive.ietf.org/arch/msg/ietf/1lnlpXJDDl5ZSA4Xn9x4sQFPlvU/) [[Farrell]](https://mailarchive.ietf.org/arch/msg/ietf/DW71uz4YNqF0ZjR2MO4yqDpk4O8/) [[Dukhovni]](https://mailarchive.ietf.org/arch/msg/ietf/i_p2XO7phdMB23tMpxQ-v0-wXYM/) [[Wilton]](https://mailarchive.ietf.org/arch/msg/ietf/fw3DVHXyhaMU_mK7C2-joXA8KXY/) [[Inacio]](https://mailarchive.ietf.org/arch/msg/ietf/nLV6GVOYBVCsEYC4fHO1OWkosHw/) [[Tschofenig]](https://mailarchive.ietf.org/arch/msg/ietf/1iNje74SUB4Pd1BY9LjtUY7sPUY/) [[Jennings]](https://mailarchive.ietf.org/arch/msg/ietf/6nwIcbph4dB9Zujot6oKH_nrkNc/) + 4 parties who provided feedback privately to the IESG

## Questions

### What is the "operational complexity" of running FTP? How much does it cost?  [[5]](https://mailarchive.ietf.org/arch/msg/ietf/62aSVFrAErl1ofSBhs6R5PND5mg/) [[6]](https://mailarchive.ietf.org/arch/msg/ietf/GY9hreNv2u-2sf-SuZK0fay0GI8/) [[7]](https://mailarchive.ietf.org/arch/msg/ietf/QryR4cQbSCooGL4TDMUp86bUcIM/) [[19]](https://mailarchive.ietf.org/arch/msg/ietf/XFJOyi9a8KsrF4vmBAghb0Zo3mo/) [[27]](https://mailarchive.ietf.org/arch/msg/ietf/KlM5s0qVWhN9vTdcIYj28g9r99A/)
* Running each additional service takes operational effort [[10]](https://mailarchive.ietf.org/arch/msg/ietf/JvPITMGo_Go0ijS-LQyk6MmIEbc/).  In particular FTP requires a number of back-end scripts to make sure files are exported into the right directory [[25]](https://mailarchive.ietf.org/arch/msg/ietf/py_9b486x8x2io6d5dAb3FAgNng/).
* Running services that are not use expose an unneeded attack surface [[49]](https://mailarchive.ietf.org/arch/msg/ietf/Sos9vi8ZQ37PLA8M1VDKqFPZuPE/) [[62]](https://mailarchive.ietf.org/arch/msg/ietf/y2EXJcnpvAp8dJ9ryYXDgUCOQtI/) [[65]](https://mailarchive.ietf.org/arch/msg/ietf/Gfv2NptSV6XBaOJTyTvixcl6dNc/)

### How small is "small" referenced in the [[retirement proposal]](https://www.ietf.org/media/documents/Retiring_IETF_FTP_Service.pdf) ?
* Per [[12 Days in the Life of the IETF FTP Service]](https://docs.google.com/document/d/1JAXspeaMWFl8ML3hSezFSM0VsJsHI4uyDlQ2dHip8jo/edit#heading=h.h29kmb4dn5ul), 140 unique IPs that are <0.02% of the IP address count on one of the HTTPS services; or <0.2% requests relative to one of the HTTPS services.
* [[28]](https://mailarchive.ietf.org/arch/msg/ietf/_slYpA7EmYg839kEkg_jRYcoyhc/) provides a narrative of this data.


### Why was so much time invested in developing an FTP retirement plan if the community is just now being consulted? [[19]](https://mailarchive.ietf.org/arch/msg/ietf/XFJOyi9a8KsrF4vmBAghb0Zo3mo/)
* This is the second time the community is being asked about retiring the FTP service.  This call for community feedback provided answers to the unaddressed questions posed in the 2015 calls up front [[25]](https://mailarchive.ietf.org/arch/msg/ietf/py_9b486x8x2io6d5dAb3FAgNng/).

## Concerns

### Traffic volumes are not a good indicator of the value of a service [[29]](https://mailarchive.ietf.org/arch/msg/ietf/mKdnC6vy-E87aj3DbRAMpmsjrQA/) [[32]](https://mailarchive.ietf.org/arch/msg/ietf/kWfCMrUPmtGaRbwJWr56_aMXtIY/)

### Cost exists to migrating existing scripts [[5]](https://mailarchive.ietf.org/arch/msg/ietf/62aSVFrAErl1ofSBhs6R5PND5mg/) [[32]](https://mailarchive.ietf.org/arch/msg/ietf/kWfCMrUPmtGaRbwJWr56_aMXtIY/)
* Roman Danyliw and volunteers at Carnegie Mellon University have offered to help anyone with FTP script conversion [[28]](https://mailarchive.ietf.org/arch/msg/ietf/_slYpA7EmYg839kEkg_jRYcoyhc/) [[128]](https://mailarchive.ietf.org/arch/msg/ietf/bkyIrK5NAdlWxFfpnmhK83wpy0M/)

### Calls for community feedback have a cost to the community as they need a response [[8]](https://mailarchive.ietf.org/arch/msg/ietf/7ImbzRpyhUmTfgcqb-hya8xU7GU/) [[11]](https://mailarchive.ietf.org/arch/msg/ietf/Y-f3Vz8icj4XPbXsz_nSLPvHm8c/)
* The IESG feels that deprecating a service requires community consultion and will err on the side of asking rather than acting unilaterally [[14]](https://mailarchive.ietf.org/arch/msg/ietf/DipA84LDtF4e0SLjcyhJbOFzuts/)
[[15]](https://mailarchive.ietf.org/arch/msg/ietf/EPcz9o1qljtnpyoeh_g5ouZ2Z3s/)

### FTP provides a unique interface (Use Cases)

#### FTP preserves unecrypted access [[8]](https://mailarchive.ietf.org/arch/msg/ietf/7ImbzRpyhUmTfgcqb-hya8xU7GU/) [[67]](https://mailarchive.ietf.org/arch/msg/ietf/RXzbxmpS0kTlbv0iDZNt9vvMMbs/)
* In 2014, the IAB issued a [Statement on Confidentiality](https://mailarchive.ietf.org/arch/msg/ietf-announce/ObCNmWcsFPNTIdMX5fmbuJoKFR8/) [[69]](https://mailarchive.ietf.org/arch/msg/ietf/1lnlpXJDDl5ZSA4Xn9x4sQFPlvU/)
* Since 2015, the IETF has been operating under a policy to [maximize encrypted access](https://www.ietf.org/about/groups/iesg/statements/maximizing-encrypted-access/) [[25]](https://mailarchive.ietf.org/arch/msg/ietf/py_9b486x8x2io6d5dAb3FAgNng/).  IETF web properties have redirected HTTP to HTTPS since this time.
* Unclear use case driving need for unencrypted access
[[68]](https://mailarchive.ietf.org/arch/msg/ietf/-jfms6u2UCMiepia0RP1R_LoBrA/) [[71]](https://mailarchive.ietf.org/arch/msg/ietf/iHkRg-TAPE7uQG93H6u7y8n8-bQ/)
[[81]](https://mailarchive.ietf.org/arch/msg/ietf/dcacxBHXCecqP_OHE5-DivUoIZw/)
* Rsync provides unencrypted access [[92]](https://mailarchive.ietf.org/arch/msg/ietf/maUHi4gfaPAH_TfsU6XbqdYYM5Y/) [[122]](https://mailarchive.ietf.org/arch/msg/ietf/b8BfvrcpLmvvjkhJ1MW8DUEzmQ8/)

#### Not all clients can access encrypted content [[19]](https://mailarchive.ietf.org/arch/msg/ietf/XFJOyi9a8KsrF4vmBAghb0Zo3mo/) [[72]](https://mailarchive.ietf.org/arch/msg/ietf/a0U1ofyDlbxS72MTmDGNY2YBpiI/) [[125]](https://mailarchive.ietf.org/arch/msg/ietf/Da4mZ1cC0pQ8IelsdCFjCBLXyO4/) 
* The usage data does not suggest that the current FTP are not in disavantaged enviroments [25](https://mailarchive.ietf.org/arch/msg/ietf/py_9b486x8x2io6d5dAb3FAgNng/) [[122]](https://mailarchive.ietf.org/arch/msg/ietf/b8BfvrcpLmvvjkhJ1MW8DUEzmQ8/)
[137](https://mailarchive.ietf.org/arch/msg/ietf/7rWVjpu1h3M3mR4OT5NqdTkSrSU/)
* Unclear use case driving need for unencrypted access
[[68]](https://mailarchive.ietf.org/arch/msg/ietf/-jfms6u2UCMiepia0RP1R_LoBrA/) [71](https://mailarchive.ietf.org/arch/msg/ietf/iHkRg-TAPE7uQG93H6u7y8n8-bQ/)
[[81]](https://mailarchive.ietf.org/arch/msg/ietf/dcacxBHXCecqP_OHE5-DivUoIZw/)


#### FTP is an alternative to strong TLS v1.3 ciphersuites [[138]](https://mailarchive.ietf.org/arch/msg/ietf/mGkqwXJvRGJz9QSQWdx3VJWrj4A/)
* All IETF web properties with content analogous to FTP (www.ietf.org, datatracker.ietf.org and tools.ietf.org) support TLS v1.0 - v1.2 [[140]](https://mailarchive.ietf.org/arch/msg/ietf/XA_pkg4blflJ7a7vNTdSMuczLlM/) [[170]](https://mailarchive.ietf.org/arch/msg/ietf/Ai6Im8jmmR7wqzfOOzfNLXBbXqc/)

#### The small community that uses FTP might mirror access for users who can't access this content otherwise [[19]](https://mailarchive.ietf.org/arch/msg/ietf/XFJOyi9a8KsrF4vmBAghb0Zo3mo/)
* The usage data does not suggest this is occuring [[25]](https://mailarchive.ietf.org/arch/msg/ietf/py_9b486x8x2io6d5dAb3FAgNng/)

#### FTP provides a search-and-find access pattern [[19]](https://mailarchive.ietf.org/arch/msg/ietf/XFJOyi9a8KsrF4vmBAghb0Zo3mo/) [[98]](https://mailarchive.ietf.org/arch/msg/ietf/oUQqlvFx7AMOkd7GaRGxtCAR2b8/)
* The usage data does not suggest this is occuring [[25]](https://mailarchive.ietf.org/arch/msg/ietf/py_9b486x8x2io6d5dAb3FAgNng/)
* Users can use a browser to visit https://www.ietf.org/ietf-ftp/ [[137]](https://mailarchive.ietf.org/arch/msg/ietf/7rWVjpu1h3M3mR4OT5NqdTkSrSU/)

#### FTP can be mounted as a file share [[29]](https://mailarchive.ietf.org/arch/msg/ietf/mKdnC6vy-E87aj3DbRAMpmsjrQA/) [[58]](https://mailarchive.ietf.org/arch/msg/ietf/wX5dg3qfP8NQpp1mlm4LIhxbb8U/)
* <discussion around WebDAV was occured, but that is not service provided by the IETF>

#### FTP is better for scripting and HTTP+HTML is complex (FTP is stable) [[29]](https://mailarchive.ietf.org/arch/msg/ietf/mKdnC6vy-E87aj3DbRAMpmsjrQA/)
* Raw versions of IETF content (without HTML encoding) is availible over HTTPS transport [[54]](https://mailarchive.ietf.org/arch/msg/ietf/oH68nGeB3GH-MnnRlaQvea6rhcg/)
* Ability to mount FTP as a file share provides stability [[58]](https://mailarchive.ietf.org/arch/msg/ietf/wX5dg3qfP8NQpp1mlm4LIhxbb8U/)
* HTTP has been backward compatible [[79]](https://mailarchive.ietf.org/arch/msg/ietf/eFuGYTJh66xcKtTKxduGuU9zdD8/)
* ...significant general conversation about HTTP vs. FTP APIs and WebDAV as an interface...

### Rsync documentation is lacking and not widely supported [[19]](https://mailarchive.ietf.org/arch/msg/ietf/XFJOyi9a8KsrF4vmBAghb0Zo3mo/) [[30]](https://mailarchive.ietf.org/arch/msg/ietf/_he4v6Gcyez0FAyx4wMqASoGrXE/)
* Guidance on using rysync to make a offline copy of IETF content [exists](https://www.ietf.org/standards/ids/internet-draft-mirror-sites/) [25](https://mailarchive.ietf.org/arch/msg/ietf/py_9b486x8x2io6d5dAb3FAgNng/).
* rsync is availible on Unix, Mac and Windows [[33]](https://mailarchive.ietf.org/arch/msg/ietf/CxhHhd1jWNFSIdV50bmJKMiZfPw/)
* Three rsync servers exist for community use [[60]](https://mailarchive.ietf.org/arch/msg/ietf/SA0IK0dPPujWMOMFvOquwstGb34/)

### FTP provides alternative access mechanism [[101]](https://mailarchive.ietf.org/arch/msg/ietf/j0vrAvb_baoo11tdET5romkRi8c/)
* Highly unlikely case [[105]](https://mailarchive.ietf.org/arch/msg/ietf/DW71uz4YNqF0ZjR2MO4yqDpk4O8/) [[106]](https://mailarchive.ietf.org/arch/msg/ietf/i_p2XO7phdMB23tMpxQ-v0-wXYM/)

## Transition Plan
The following suggestions were made on facilitating the retirement:

### Fix pointers to FTP in embedded in the datatracker status page [[35]](https://mailarchive.ietf.org/arch/msg/ietf/MZbB4JbiyAvMX30CvT_55hGB_74/)

### Retire FTP by having the service only serve a README that points to the locations of the content [[19]](https://mailarchive.ietf.org/arch/msg/ietf/XFJOyi9a8KsrF4vmBAghb0Zo3mo/) [[134]](https://mailarchive.ietf.org/arch/msg/ietf/SZBuNoGOiSajpsvurZ9hQuiNINc/) [[139]](https://mailarchive.ietf.org/arch/msg/ietf/-nZbFI-D1bp-o-LYGJNA_U1k9fQ/)

### Consider building an "FTP-rsync" gateway [[46]](https://mailarchive.ietf.org/arch/msg/ietf/2Ir9MUzPgD3hJMmfPArruDXPd0A/)
* Bespoke tools will add more complexity [[48]](https://mailarchive.ietf.org/arch/msg/ietf/HLdTmVhcgO2a3c-o5FkpOE6Ml0w/)
* Custom tools are important to the IETF [[50]](https://mailarchive.ietf.org/arch/msg/ietf/uDV_Bojxolx0zazwb3Egdavffts/)

### Move FTP and Gopher specifications to historic status [[64]](https://mailarchive.ietf.org/arch/msg/ietf/Nydu9WAV7OOUDbXTNB6rkH8IIfM/) [[75]](https://mailarchive.ietf.org/arch/msg/ietf/6CBooP788Jeb4wyjkxNOL8d8gSQ/) [[129]](https://mailarchive.ietf.org/arch/msg/ietf/XPEx0zMSyi9BdXn79vcbM47351Q/)

