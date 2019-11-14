---
Description: Control codes used in disk management.
ms.assetid: 488a7d32-cbb5-4f32-9655-0aca8ac69640
title: Disk Management Control Codes
ms.topic: article
ms.date: 05/31/2018
---

# Disk Management Control Codes

The following table identifies the control codes that are used in disk management.

## In this section



| Control Code                                                                                              | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|-----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**IOCTL\_DISK\_ARE\_VOLUMES\_READY**](ioctl-disk-are-volumes-ready.md)<br/>                       | Waits for all volumes on the specified disk to be ready for use.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| [**IOCTL\_DISK\_CREATE\_DISK**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_create_disk)<br/>                                    | Initializes the specified disk and disk partition table using the information in the [**CREATE\_DISK**](/windows/desktop/api/WinIoCtl/ns-winioctl-create_disk) structure.<br/>                                                                                                                                                                                                                                                                                                                                                                                        |
| [**IOCTL\_DISK\_DELETE\_DRIVE\_LAYOUT**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_delete_drive_layout)<br/>                   | Removes the boot signature from the master boot record, so that the disk will be formatted from sector zero to the end of the disk.<br/>                                                                                                                                                                                                                                                                                                                                                                                            |
| [**IOCTL\_DISK\_FORMAT\_TRACKS**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_format_tracks)<br/>                                | Formats a specified, contiguous set of tracks on a floppy disk. To provide additional parameters, use [**IOCTL\_DISK\_FORMAT\_TRACKS\_EX**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_format_tracks_ex) instead.<br/>                                                                                                                                                                                                                                                                                                                                          |
| [**IOCTL\_DISK\_FORMAT\_TRACKS\_EX**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_format_tracks_ex)<br/>                         | Formats a specified, contiguous set of tracks on a floppy disk.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| [**IOCTL\_DISK\_GET\_CACHE\_INFORMATION**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_cache_information)<br/>               | Retrieves the disk cache configuration data.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| [**IOCTL\_DISK\_GET\_CLUSTER\_INFO**](ioctl-disk-get-cluster-info.md)<br/>                         | Retrieves the attributes of the specified disk device.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| [**IOCTL\_DISK\_GET\_DISK\_ATTRIBUTES**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_disk_attributes)<br/>                   | Retrieves the attributes of the specified disk device.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| [**IOCTL\_DISK\_GET\_DRIVE\_GEOMETRY**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_drive_geometry)<br/>                     | Retrieves information about the physical disk's geometry: type, number of cylinders, tracks per cylinder, sectors per track, and bytes per sector.<br/>                                                                                                                                                                                                                                                                                                                                                                             |
| [**IOCTL\_DISK\_GET\_DRIVE\_GEOMETRY\_EX**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_drive_geometry_ex)<br/>              | Retrieves extended information about the physical disk's geometry: type, number of cylinders, tracks per cylinder, sectors per track, and bytes per sector.<br/>                                                                                                                                                                                                                                                                                                                                                                    |
| [**IOCTL\_DISK\_GET\_DRIVE\_LAYOUT**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_drive_layout)<br/>                         | Retrieves information for each entry in the partition tables for a disk.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [**IOCTL\_DISK\_GET\_DRIVE\_LAYOUT\_EX**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_drive_layout_ex)<br/>                  | Retrieves extended information for each entry in the partition tables for a disk.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [**IOCTL\_DISK\_GET\_LENGTH\_INFO**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_length_info)<br/>                           | Retrieves the length of the specified disk, volume, or partition.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [**IOCTL\_DISK\_GET\_PARTITION\_INFO**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_partition_info)<br/>                     | Retrieves information about the type, size, and nature of a disk partition.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| [**IOCTL\_DISK\_GET\_PARTITION\_INFO\_EX**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_partition_info_ex)<br/>              | Retrieves extended information about the type, size, and nature of a disk partition.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [**IOCTL\_DISK\_GROW\_PARTITION**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_grow_partition)<br/>                              | Enlarges the specified partition.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [**IOCTL\_DISK\_IS\_WRITABLE**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_is_writable)<br/>                                    | Determines whether the specified disk is writable.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [**IOCTL\_DISK\_PERFORMANCE**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_performance)<br/>                                     | Enables performance counters that provide disk performance information.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| [**IOCTL\_DISK\_PERFORMANCE\_OFF**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_performance_off)<br/>                            | Disables the performance counters that provide disk performance information.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| [**IOCTL\_DISK\_REASSIGN\_BLOCKS**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_reassign_blocks)<br/>                            | Directs the disk device to map one or more blocks to its spare-block pool.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| [**IOCTL\_DISK\_REASSIGN\_BLOCKS\_EX**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_reassign_blocks_ex)<br/>                     | Directs the disk device to map one or more blocks to its spare-block pool.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| [**IOCTL\_DISK\_RESET\_SNAPSHOT\_INFO**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_reset_snapshot_info)<br/>                   | Clears all Volume Shadow Copy Service (VSS) hardware-based shadow copy (also called "snapshot") information from the disk.<br/> To perform this operation, call the [**DeviceIoControl**](https://docs.microsoft.com/windows/desktop/api/ioapiset/nf-ioapiset-deviceiocontrol) function with the following parameters.<br/>                                                                                                                                                                                                                                                                  |
| [**IOCTL\_DISK\_SET\_CACHE\_INFORMATION**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_set_cache_information)<br/>               | Sets the disk configuration data.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [**IOCTL\_DISK\_SET\_CLUSTER\_INFO**](ioctl-disk-set-cluster-info.md)<br/>                         | Sets the cluster information on a disk.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| [**IOCTL\_DISK\_SET\_DISK\_ATTRIBUTES**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_set_disk_attributes)<br/>                   | Sets the attributes of the specified disk device.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [**IOCTL\_DISK\_SET\_DRIVE\_LAYOUT**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_set_drive_layout)<br/>                         | Partitions a disk as specified by drive layout and partition information data.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [**IOCTL\_DISK\_SET\_DRIVE\_LAYOUT\_EX**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_set_drive_layout_ex)<br/>                  | Partitions a disk according to the specified drive layout and partition information data.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| [**IOCTL\_DISK\_SET\_PARTITION\_INFO**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_set_partition_info)<br/>                     | Sets partition information for the specified disk partition.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| [**IOCTL\_DISK\_SET\_PARTITION\_INFO\_EX**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_set_partition_info_ex)<br/>              | Sets partition information for the specified disk partition, including layout information for AT and EFI (Extensible Firmware Interface) partitions.<br/>                                                                                                                                                                                                                                                                                                                                                                           |
| [**IOCTL\_DISK\_UPDATE\_PROPERTIES**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_update_properties)<br/>                        | Invalidates the cached partition table and re-enumerates the device.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [**IOCTL\_DISK\_VERIFY**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_verify)<br/>                                               | Verifies the specified extent on a fixed disk.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [**IOCTL\_STORAGE\_DEVICE\_POWER\_CAP**](/windows/desktop/api/WinIoctl/ni-winioctl-ioctl_storage_device_power_cap)<br/>                   | Windows applications can use this control code to specify a maximum operational power consumption level for a storage device. The OS will do it's best to transition the device to a power state that will not exceed the given maximum. However, this depends on what the device supports. The actual maximum may be less than or greater than the desired maximum.<br/> To perform this operation, call the [**DeviceIoControl**](https://docs.microsoft.com/windows/desktop/api/ioapiset/nf-ioapiset-deviceiocontrol) function with the following parameters.<br/>                        |
| [**IOCTL\_STORAGE\_FIRMWARE\_ACTIVATE**](/windows/desktop/api/WinIoctl/ni-winioctl-ioctl_storage_firmware_activate)<br/>                  | Windows applications can use this control code to activate a firmware image on a specified device.<br/> To perform this operation, call the [**DeviceIoControl**](https://docs.microsoft.com/windows/desktop/api/ioapiset/nf-ioapiset-deviceiocontrol) function with the following parameters.<br/>                                                                                                                                                                                                                                                                                          |
| [**IOCTL\_STORAGE\_FIRMWARE\_DOWNLOAD**](/windows/desktop/api/WinIoctl/ni-winioctl-ioctl_storage_firmware_download)<br/>                  | Windows applications can use this control code to download a firmware image to the target device, but not activate it. If the image to be downloaded is larger than the controller s maximum data transfer size, this IOCTL will have to be called multiple times until the entire image is downloaded.<br/> To perform this operation, call the [**DeviceIoControl**](https://docs.microsoft.com/windows/desktop/api/ioapiset/nf-ioapiset-deviceiocontrol) function with the following parameters.<br/>                                                                                     |
| [**IOCTL\_STORAGE\_FIRMWARE\_GET\_INFO**](/windows/desktop/api/WinIoctl/ni-winioctl-ioctl_storage_firmware_get_info)<br/>                 | Windows applications can use this control code to query the storage device for detailed firmware information. A successful call will return information about firmware revisions, activity status, as well as read/write attributes for each slot. The amount of data returned will vary based on storage protocol.<br/> To perform this operation, call the [**DeviceIoControl**](https://docs.microsoft.com/windows/desktop/api/ioapiset/nf-ioapiset-deviceiocontrol) function with the following parameters.<br/>                                                                         |
| [**IOCTL\_STORAGE\_PROTOCOL\_COMMAND**](/windows/desktop/api/winioctl/ni-winioctl-ioctl_storage_protocol_command)<br/>                    | Windows applications can use this control code to return properties of a storage device or adapter. The request indicates the kind of information to retrieve, such as inquiry data for a device or capabilities and limitations of an adapter. <br/>                                                                                                                                                                                                                                                                               |
| [**IOCTL\_STORAGE\_QUERY\_PROPERTY**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_storage_query_property)<br/>                        | Windows applications can use this control code to return the properties of a storage device or adapter. The request indicates the kind of information to retrieve, such as the inquiry data for a device or the capabilities and limitations of an adapter. [**IOCTL\_STORAGE\_QUERY\_PROPERTY**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_storage_query_property) can also be used to determine whether the port driver supports a particular property or which fields in the property descriptor can be modified with a subsequent change-property request.<br/> |
| [**IOCTL\_STORAGE\_SET\_TEMPERATURE\_THRESHOLD**](/windows/desktop/api/WinIoctl/ni-winioctl-ioctl_storage_set_temperature_threshold)<br/> | Windows applications can use this control code to set the temperature threshold of a device (when it's supported by the device). <br/>                                                                                                                                                                                                                                                                                                                                                                                              |



 

The following control codes are obsolete:

<dl> **IOCTL\_DISK\_CONTROLLER\_NUMBER**  
[**IOCTL\_DISK\_GET\_DRIVE\_GEOMETRY**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_drive_geometry)  
[**IOCTL\_DISK\_GET\_DRIVE\_LAYOUT**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_drive_layout)  
[**IOCTL\_DISK\_GET\_PARTITION\_INFO**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_get_partition_info)  
**IOCTL\_DISK\_HISTOGRAM\_DATA**  
**IOCTL\_DISK\_HISTOGRAM\_RESET**  
**IOCTL\_DISK\_HISTOGRAM\_STRUCTURE**  
**IOCTL\_DISK\_LOGGING**  
**IOCTL\_DISK\_REQUEST\_DATA**  
**IOCTL\_DISK\_REQUEST\_STRUCTURE**  
[**IOCTL\_DISK\_SET\_DRIVE\_LAYOUT**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_set_drive_layout)  
[**IOCTL\_DISK\_SET\_PARTITION\_INFO**](/windows/desktop/api/WinIoCtl/ni-winioctl-ioctl_disk_set_partition_info)  
</dl>

 

 



