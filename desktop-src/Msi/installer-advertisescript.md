---
Description: The AdvertiseScript method of the Installer object advertises an installation package.
ms.assetid: 45e5268f-7a5f-412f-b9f6-0abb75b79361
title: Installer::AdvertiseScript method
ms.topic: reference
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- Installer.AdvertiseScript
api_type: 
- COM
api_location: 
- Msi.dll
---

# Installer::AdvertiseScript method

The **AdvertiseScript** method of the [**Installer**](installer-object.md) object advertises an installation package.

## Syntax


```JScript
.AdvertiseScript(
  scriptPath,
  scriptFlags,
  removeItems
)
```



## Parameters

<dl> <dt>

*scriptPath* 
</dt> <dd>

The full path to the script file generated by the [**CreateAdvertiseScript**](installer-createadvertisescript.md) method.

</dd> <dt>

*scriptFlags* 
</dt> <dd>

The flags that control the advertisement. This parameter can be a combination of the following values.



| Value                                                                                                                                                                                                                                                                                                                                                                           | Meaning                                                                                                                                                                                                                                                                                                                                                                             |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span id="msiAdvertiseScriptCacheInfo"></span><span id="msiadvertisescriptcacheinfo"></span><span id="MSIADVERTISESCRIPTCACHEINFO"></span><dl> <dt>**msiAdvertiseScriptCacheInfo**</dt> <dt>0x001</dt> </dl>                                                                 | Include this flag if the icons need to be created or removed.<br/>                                                                                                                                                                                                                                                                                                            |
| <span id="msiAdvertiseScriptShortcuts"></span><span id="msiadvertisescriptshortcuts"></span><span id="MSIADVERTISESCRIPTSHORTCUTS"></span><dl> <dt>**msiAdvertiseScriptShortcuts**</dt> <dt>0x004</dt> </dl>                                                                 | Include this flag if the shortcuts need to be created or removed.<br/>                                                                                                                                                                                                                                                                                                        |
| <span id="msiAdvertiseScriptMachineAssign"></span><span id="msiadvertisescriptmachineassign"></span><span id="MSIADVERTISESCRIPTMACHINEASSIGN"></span><dl> <dt>**msiAdvertiseScriptMachineAssign**</dt> <dt>0x008</dt> </dl>                                                 | Include this flag if the product is to be assigned to a computer.<br/>                                                                                                                                                                                                                                                                                                        |
| <span id="msiAdvertiseScriptConfigurationRegistration"></span><span id="msiadvertisescriptconfigurationregistration"></span><span id="MSIADVERTISESCRIPTCONFIGURATIONREGISTRATION"></span><dl> <dt>**msiAdvertiseScriptConfigurationRegistration**</dt> <dt>0x020</dt> </dl> | Include this flag if the configuration and management information in the registry data needs to be written or removed.<br/>                                                                                                                                                                                                                                                   |
| <span id="msiAdvertiseScriptValidateTransformList"></span><span id="msiadvertisescriptvalidatetransformlist"></span><span id="MSIADVERTISESCRIPTVALIDATETRANSFORMLIST"></span><dl> <dt>**msiAdvertiseScriptValidateTransformList**</dt> <dt>0x040</dt> </dl>                 | Include this flag to force the validation of the transforms listed in the script against previously registered transforms for this product. Note that transform conflicts are detected using a string comparison that is case insensitive and are evaluated between per-user and per-machine installations across all [installation contexts](installation-context.md).<br/> |
| <span id="msiAdvertiseScriptClassInfoRegistration"></span><span id="msiadvertisescriptclassinforegistration"></span><span id="MSIADVERTISESCRIPTCLASSINFOREGISTRATION"></span><dl> <dt>**msiAdvertiseScriptClassInfoRegistration**</dt> <dt>0x080</dt> </dl>                 | Include this flag if advertisement information in the registry related to COM classes needs to be written or removed.<br/>                                                                                                                                                                                                                                                    |
| <span id="msiAdvertiseScriptExtensionInfoRegistration"></span><span id="msiadvertisescriptextensioninforegistration"></span><span id="MSIADVERTISESCRIPTEXTENSIONINFOREGISTRATION"></span><dl> <dt>**msiAdvertiseScriptExtensionInfoRegistration**</dt> <dt>0x100</dt> </dl> | Include this flag if advertisement information in the registry related to an extension needs to be written or removed.<br/>                                                                                                                                                                                                                                                   |
| <span id="msiAdvertiseScriptAppInfo"></span><span id="msiadvertisescriptappinfo"></span><span id="MSIADVERTISESCRIPTAPPINFO"></span><dl> <dt>**msiAdvertiseScriptAppInfo**</dt> <dt>0x180</dt> </dl>                                                                         | Include this flag if the advertisement information in the registry needs to be written or removed.<br/>                                                                                                                                                                                                                                                                       |
| <span id="msiAdvertiseScriptRegData"></span><span id="msiadvertisescriptregdata"></span><span id="MSIADVERTISESCRIPTREGDATA"></span><dl> <dt>**msiAdvertiseScriptRegData**</dt> <dt>0x1A0</dt> </dl>                                                                         | Include this flag if the advertisement information in the registry needs to be written or removed.<br/>                                                                                                                                                                                                                                                                       |



 

</dd> <dt>

*removeItems* 
</dt> <dd>

TRUE if the specified items are to be removed instead of being created.

</dd> </dl>

## Return value

This method does not return a value.

## Remarks

The **AdvertiseScript** method uses the [**MsiAdvertiseScript**](/windows/desktop/api/Msi/nf-msi-msiadvertisescripta) function. The use of the **AdvertiseScript** method requires that the script be running within a local system process.

## Examples

The following example demonstrates the use of the **AdvertiseScript** method.


```VB
Dim installer
Set installer = CreateObject("WindowsInstaller.Installer")

' Advertise Simple package using an advertise script
'   created by CreateAdvertiseScript Method
'
'  Flags 424 indicate msiAdvertiseScriptMachineAssign, msiAdvertiseScriptRegData

Installer.AdvertiseScript "c:\scratch\simpletst\rtm\simple.aas", 424, false

' Verify Simple is installed
MsgBox Installer.ProductState("{BAE98781-CF88-4309-8E2D-3D8B347F5B53}")

'
' Remove Simple using advertise script
'
Installer.AdvertiseScript "c:\scratch\simpletst\rtm\simple.aas", 424, true

' Verify simple is removed
MsgBox Installer.ProductState("{BAE98781-CF88-4309-8E2D-3D8B347F5B53}")
```



## Requirements



|                    |                                                                                                                                                                                                                                                              |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Version<br/> | Windows Installer 5.0 on Windows Server 2012, Windows 8, Windows Server 2008 R2 or Windows 7. Windows Installer 4.0 or Windows Installer 4.5 on Windows Server 2008 or Windows Vista. Windows Installer 4.5 on Windows Server 2003 and Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                           |
| IID<br/>     | IID\_IInstaller is defined as 000C1090-0000-0000-C000-000000000046<br/>                                                                                                                                                                                |



## See also

<dl> <dt>

[**Installer**](installer-object.md)
</dt> <dt>

[Not Supported in Windows Installer 3.1 and earlier versions](not-supported-in-windows-installer-version-3-1.md)
</dt> </dl>

 

 



