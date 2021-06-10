---
layout: post
tags: [azure,WVD, Windows Virtual Desktop]
title: Azure Files SMB Multichannel
excerpt_separator: <!--more-->
---
Azure Files SMB Multichannel (preview) enables an SMB 3.x client to establish multiple network connections to the premium file shares in a FileStorage account. 
Learn how to configure it!

![SMB Multichannel ]({{ site.baseurl }}/assets/img/blog/2021-06-06-ConfigureAZStorageSMBMulti/smb-multi1.jpg)

<!--more-->

Azure Files SMB Multichannel (preview) enables an SMB 3.x client to establish multiple network connections to the premium file shares in a FileStorage account. The SMB 3.x protocol introduced the SMB Multichannel feature in Windows Server 2012 and Windows 8 clients. Because of this, any Azure Files SMB 3.x client that supports SMB Multichannel can take advantage of the feature for their Azure premium file shares. There is no additional cost for enabling SMB Multichannel on a storage account.

Curently SMB Multichannel for Azure Files is in preview and has limitations listed below:

+ Only supported for Windows clients.
+ Maximum number of channels is four.
+ SMB Direct is not supported.
+ Private endpoints for storage accounts are not supported.
+ For storage accounts with on-premises Active Directory Domain Services (AD DS) or Azure AD DS identity-based authentication enabled for Azure Files, SMB clients would not be able to use Windows File Explorer to configure NTFS permissions on directories and files.
+ Use Windows icacls tool or Set-ACL command instead to configure permissions.

SMB Multichannel for Azure files shares is available in all public cloud regions where premium file shares are available (LRS and ZRS)

Lets move on to the fun part, configuration!

	

Thanks!
