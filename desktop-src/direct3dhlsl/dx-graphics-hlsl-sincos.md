---
title: sincos
description: Returns the sine and cosine of x.
ms.assetid: 2ef9e84e-4539-47f5-9966-d8e02ca15d36
keywords:
- sincos HLSL
topic_type:
- apiref
api_name:
- sincos
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: 
---

# sincos

Returns the sine and cosine of x.



| sincos(*x*, out *s*, out *c*) |
|-------------------------------|



 

## Parameters



| Item                                                   | Description                                        |
|--------------------------------------------------------|----------------------------------------------------|
| <span id="x"></span><span id="X"></span>*x*<br/> | \[in\] The specified value, in radians.<br/> |
| <span id="s"></span><span id="S"></span>*s*<br/> | \[out\] Returns the sine of x.<br/>          |
| <span id="c"></span><span id="C"></span>*c*<br/> | \[out\] Returns the cosine of x.<br/>        |



 

## Return Value

None.

## Type Description



| Name | [**Template Type**](dx-graphics-hlsl-intrinsic-functions.md)                                                  | [**Component Type**](dx-graphics-hlsl-intrinsic-functions.md) | Size                           |
|------|----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------|--------------------------------|
| *x*  | [**scalar**](dx-graphics-hlsl-intrinsic-functions.md), **vector**, or **matrix** | [**float**](https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types)                        | any                            |
| *s*  | same as input *x*                                                                                              | [**float**](https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types)                        | same dimension(s) as input *x* |
| c    | same as input *x*                                                                                              | [**float**](https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types)                        | same dimension(s) as input *x* |



 

## Minimum Shader Model

This function is supported in the following shader models.



| Shader Model                                                                       | Supported           |
|------------------------------------------------------------------------------------|---------------------|
| [Shader Model 2 (DirectX HLSL)](dx-graphics-hlsl-sm2.md) and higher shader models | yes                 |
| [Shader Model 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md)                          | yes (vs\_1\_1 only) |



 

## See also

<dl> <dt>

[**Intrinsic Functions (DirectX HLSL)**](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

 

 




