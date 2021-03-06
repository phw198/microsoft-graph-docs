﻿# androidImportedPFXCertificateProfile resource type

> **Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported.

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Android PFX Import certificate profile

Inherits from [androidCertificateProfileBase](../resources/intune_deviceconfig_androidcertificateprofilebase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidImportedPFXCertificateProfiles](../api/intune_deviceconfig_androidimportedpfxcertificateprofile_list.md)|[androidImportedPFXCertificateProfile](../resources/intune_deviceconfig_androidimportedpfxcertificateprofile.md) collection|List properties and relationships of the [androidImportedPFXCertificateProfile](../resources/intune_deviceconfig_androidimportedpfxcertificateprofile.md) objects.|
|[Get androidImportedPFXCertificateProfile](../api/intune_deviceconfig_androidimportedpfxcertificateprofile_get.md)|[androidImportedPFXCertificateProfile](../resources/intune_deviceconfig_androidimportedpfxcertificateprofile.md)|Read properties and relationships of the [androidImportedPFXCertificateProfile](../resources/intune_deviceconfig_androidimportedpfxcertificateprofile.md) object.|
|[Create androidImportedPFXCertificateProfile](../api/intune_deviceconfig_androidimportedpfxcertificateprofile_create.md)|[androidImportedPFXCertificateProfile](../resources/intune_deviceconfig_androidimportedpfxcertificateprofile.md)|Create a new [androidImportedPFXCertificateProfile](../resources/intune_deviceconfig_androidimportedpfxcertificateprofile.md) object.|
|[Delete androidImportedPFXCertificateProfile](../api/intune_deviceconfig_androidimportedpfxcertificateprofile_delete.md)|None|Deletes a [androidImportedPFXCertificateProfile](../resources/intune_deviceconfig_androidimportedpfxcertificateprofile.md).|
|[Update androidImportedPFXCertificateProfile](../api/intune_deviceconfig_androidimportedpfxcertificateprofile_update.md)|[androidImportedPFXCertificateProfile](../resources/intune_deviceconfig_androidimportedpfxcertificateprofile.md)|Update the properties of a [androidImportedPFXCertificateProfile](../resources/intune_deviceconfig_androidimportedpfxcertificateprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the entity. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|renewalThresholdPercentage|Int32|Certificate renewal threshold percentage. Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune_deviceconfig_androidcertificateprofilebase.md)|
|subjectNameFormat|String|Certificate Subject Name Format. Inherited from [androidCertificateProfileBase](../resources/intune_deviceconfig_androidcertificateprofilebase.md) Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.|
|subjectAlternativeNameType|String|Certificate Subject Alternative Name Type. Inherited from [androidCertificateProfileBase](../resources/intune_deviceconfig_androidcertificateprofilebase.md) Possible values are: `emailAddress`, `userPrincipalName`, `customAzureADAttribute`.|
|certificateValidityPeriodValue|Int32|Value for the Certificate Validity Period. Inherited from [androidCertificateProfileBase](../resources/intune_deviceconfig_androidcertificateprofilebase.md)|
|certificateValidityPeriodScale|String|Scale for the Certificate Validity Period. Inherited from [androidCertificateProfileBase](../resources/intune_deviceconfig_androidcertificateprofilebase.md) Possible values are: `days`, `months`, `years`.|
|extendedKeyUsages|[extendedKeyUsage](../resources/intune_deviceconfig_extendedkeyusage.md) collection|Extended Key Usage (EKU) settings. This collection can contain a maximum of 500 elements. Inherited from [androidCertificateProfileBase](../resources/intune_deviceconfig_androidcertificateprofilebase.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection|Device configuration installation stauts by user. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|rootCertificate|[androidTrustedRootCertificate](../resources/intune_deviceconfig_androidtrustedrootcertificate.md)|Trusted Root Certificate. Inherited from [androidCertificateProfileBase](../resources/intune_deviceconfig_androidcertificateprofilebase.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidImportedPFXCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "renewalThresholdPercentage": 1024,
  "subjectNameFormat": "String",
  "subjectAlternativeNameType": "String",
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ]
}
```



