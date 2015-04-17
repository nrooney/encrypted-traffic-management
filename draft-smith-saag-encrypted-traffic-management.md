---
title: Network management of encrypted traffic
abbrev: encrypted-traffic-management
docname: draft-smith-saag-encrypted-traffic-management-latest
date: 2015-04-17
category: info

ipr: trust200902
area: Security
workgroup:
keyword: Internet-Draft

stand_alone: yes
pi: [toc, sortrefs, symrefs]

author:
 -
    ins: K. Smith
    name: Kevin Smith
    organization: Vodafone Group
    email: kevin.smith@vodafone.com

normative:
  RFC7258:

informative:
  mm-effect-encrypt: 
    target: https://datatracker.ietf.org/doc/draft-mm-wg-effect-encrypt/ 
    title: Effect of Ubiquitous Encryption
    author: 
      name: K. Moriarty, A. Morton 
      org: IETF 
      date: 2014-11-14
  
  IAB: 
    target: https://www.iab.org/2014/11/14/iab-statement-on-internet-confidentiality/ 
    title: IAB statement on Internet confidentiality 
    author: 
      name: Internet Architecture Board 
      org: IAB 
      date: 2014-11-14
  
  TAG: 
    target: https://w3ctag.github.io/web-https/ 
    title: Securing the Web 
    author: 
      name: W3C TAG 
      org: W3C	 
      date: 2015-01-15
  
--- abstract

Encrypted Internet traffic may pose traffic management challenges to network operators. This document recommends approaches to help manage encrypted traffic, without breaching user privacy or security.

--- middle

Introduction        {#intro}
============
Networks utilise various management techniques to ensure efficient throughput, congestion management, anti-SPAM and security measures. Historically these functions have utilised visibility of the Internet application layer.

This visibility is rapidly diminishing - encrypted Internet traffic is expected to continue its upward trend, driven by increased privacy
awareness, uptake by major players and advocacy from the {{IAB}},  {{RFC7258}} and W3C {{TAG}}. 

{{IAB}}, {{RFC7258}} and {{mm-effect-encrypt}} recognise that network management functions are impacted by encryption, and that solutions are needed to persist them - as long as they do not threaten privacy. Such solutions would ensure the benefits of encryption do not degrade network efficiency. 


Document conventions   {#conv}
----------------------------
This document
describes the technical details of existing options to persist network management functions
for encrypted traffic. These options are categorised into two main sections: first, where encryption is used 
between the content server and client, and second, where browser proxies tunnel 'http' URIs over TLS. 

Finally a summary is provided of ongoing IETF work which is investigating how middleboxes along the path can improve encrypted traffic delivery. 

‘Mitigation’ is used throughout this document, and refers to a method of fully or partially supporting a
particular network management function when traffic is encrypted. This term is not meant to imply a removal or workaround of encryption.


Existing mitigations  {#exmit}
====================

Mitigation 1
----------

Mitigation 2
----------

Discommended mitigations {#disc}
========================

Prototype mitigations {#proto}
=====================

Acknowledgements
================

IANA Considerations
===================

Security Considerations
=======================



