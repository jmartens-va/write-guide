---
Description: The Windows operating system supports authentication using security packages that function as both security support providers and as authentication packages.
ms.assetid: f40060be-fad2-4008-b981-727199d71581
title: Security Support Provider/Authentication Packages
ms.topic: article
ms.date: 05/31/2018
---

# Security Support Provider/Authentication Packages

The Windows operating system supports authentication using [*security packages*](https://msdn.microsoft.com/en-us/library/ms721625(v=VS.85).aspx) that function as both [*security support providers*](https://msdn.microsoft.com/en-us/library/ms721625(v=VS.85).aspx) and as [*authentication packages*](https://msdn.microsoft.com/en-us/library/ms721532(v=VS.85).aspx). Security packages provide the logon process support services of a Windows authentication package and also provide authentication services to applications by implementing a set of functions that are mapped to the [Security Support Provider Interface](sspi.md) (SSPI).

A security package that functions as an authentication package and implements the functionality required by [*SSPI*](https://msdn.microsoft.com/en-us/library/ms721625(v=VS.85).aspx) is called a security support provider/authentication package (SSP/AP).

For more information about security packages, see [SSP Packages Provided by Microsoft](ssp-packages-provided-by-microsoft.md). For information about developing custom SSP/APs, see [Custom Security Packages](custom-security-packages.md).

 

 



