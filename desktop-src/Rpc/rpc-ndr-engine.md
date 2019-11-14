---
title: RPC NDR Engine (RPC)
description: The Remote Procedure Call (RPC) Network Data Representation (NDR) Engine is the marshaling engine of the RPC and DCOM components.
ms.assetid: E452AA27-053D-4032-868B-CF2D5C0D4BE0
ms.topic: article
ms.date: 05/31/2018
---

# RPC NDR Engine

The Remote Procedure Call (RPC) Network Data Representation (NDR) Engine is the marshaling engine of the RPC and DCOM components. The NDR Engine handles all stub-related issues of a remote call. As a process, NDR marshaling is driven by the C code from MIDL-generated stubs, a MIDL JIT-type generator, or by stubs generated by other tools or written manually. In turn, the NDR engine drives the underlying run time (DCOM or RPC) that communicates with specific transports.

Although stubs are C code that are generated by MIDL, applications are advised to treat stubs as opaque, and strongly discouraged from modifying anything inside the stub. The behavior is undefined if these NDR routines are called out of context.

The RPC NDR Engine is described in more detail in the following topics:

-   [Transfer Syntax and NDR64](transfer-syntax-and-ndr64.md)
-   [RPC NDR Format Strings](rpc-ndr-format-strings.md)
-   [RPC NDR Interface Reference](rpc-ndr-interface-reference.md)

 

 



