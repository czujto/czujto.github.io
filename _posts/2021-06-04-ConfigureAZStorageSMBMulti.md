---
layout: post
tags: [azure,WVD, Windows Virtual Desktop]
title: Azure Files SMB Multichannel
excerpt_separator: <!--more-->
---
Azure Files SMB Multichannel (preview) enables an SMB 3.x client to establish multiple network connections to the premium file shares in a FileStorage account. 
Learn how to configure it!

![SMB Multichannel ]({{ site.baseurl }}/assets/img/blog/2021-06-06-ConfigureAZStorageSMBMulti/smb-multi.PNG)

<!--more-->
Azure Files SMB Multichannel (preview) enables an SMB 3.x client to establish multiple network connections to the premium file shares in a FileStorage account. The SMB 3.x protocol introduced the SMB Multichannel feature in Windows Server 2012 and Windows 8 clients. Because of this, any Azure Files SMB 3.x client that supports SMB Multichannel can take advantage of the feature for their Azure premium file shares. There is no additional cost for enabling SMB Multichannel on a storage account



Thanks!
