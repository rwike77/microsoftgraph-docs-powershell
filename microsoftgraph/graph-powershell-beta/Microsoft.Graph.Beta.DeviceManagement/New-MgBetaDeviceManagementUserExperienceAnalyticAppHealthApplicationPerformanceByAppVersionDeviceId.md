---
external help file: Microsoft.Graph.Beta.DeviceManagement-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementuserexperienceanalyticapphealthapplicationperformancebyappversiondeviceid
schema: 2.0.0
---

# New-MgBetaDeviceManagementUserExperienceAnalyticAppHealthApplicationPerformanceByAppVersionDeviceId

## SYNOPSIS
Create new navigation property to userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersionDeviceId for deviceManagement

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgDeviceManagementUserExperienceAnalyticAppHealthApplicationPerformanceByAppVersionDeviceId](/powershell/module/Microsoft.Graph.DeviceManagement/New-MgDeviceManagementUserExperienceAnalyticAppHealthApplicationPerformanceByAppVersionDeviceId?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaDeviceManagementUserExperienceAnalyticAppHealthApplicationPerformanceByAppVersionDeviceId
 [-AdditionalProperties <Hashtable>] [-AppCrashCount <Int32>] [-AppDisplayName <String>] [-AppName <String>]
 [-AppPublisher <String>] [-AppVersion <String>] [-DeviceDisplayName <String>] [-DeviceId <String>]
 [-Id <String>] [-ProcessedDateTime <DateTime>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaDeviceManagementUserExperienceAnalyticAppHealthApplicationPerformanceByAppVersionDeviceId
 -BodyParameter <IMicrosoftGraphUserExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersionDeviceId for deviceManagement

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppCrashCount
The number of crashes for the app.
Valid values -2147483648 to 2147483647

```yaml
Type: Int32
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppDisplayName
The friendly name of the application.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppName
The name of the application.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppPublisher
The publisher of the application.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppVersion
The version of the application.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
The user experience analytics application performance entity contains application performance by application version device id.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DeviceDisplayName
The name of the device.
Supports: $select, $OrderBy.
Read-only.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceId
The Intune device id of the device.
Supports: $select, $OrderBy.
Read-only.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The unique identifier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProcessedDateTime
The date and time when the statistics were last computed.
The value cannot be modified and is automatically populated when the statistics are computed.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2022 would look like this: '2022-01-01T00:00:00Z'.
Returned by default.
Read-only.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUserExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUserExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphUserExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId\>: The user experience analytics application performance entity contains application performance by application version device id.
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AppCrashCount \<Int32?\>\]: The number of crashes for the app.
Valid values -2147483648 to 2147483647
  \[AppDisplayName \<String\>\]: The friendly name of the application.
  \[AppName \<String\>\]: The name of the application.
  \[AppPublisher \<String\>\]: The publisher of the application.
  \[AppVersion \<String\>\]: The version of the application.
  \[DeviceDisplayName \<String\>\]: The name of the device.
Supports: $select, $OrderBy.
Read-only.
  \[DeviceId \<String\>\]: The Intune device id of the device.
Supports: $select, $OrderBy.
Read-only.
  \[ProcessedDateTime \<DateTime?\>\]: The date and time when the statistics were last computed.
The value cannot be modified and is automatically populated when the statistics are computed.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2022 would look like this: '2022-01-01T00:00:00Z'.
Returned by default.
Read-only.

## RELATED LINKS
[New-MgDeviceManagementUserExperienceAnalyticAppHealthApplicationPerformanceByAppVersionDeviceId](/powershell/module/Microsoft.Graph.DeviceManagement/New-MgDeviceManagementUserExperienceAnalyticAppHealthApplicationPerformanceByAppVersionDeviceId?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementuserexperienceanalyticapphealthapplicationperformancebyappversiondeviceid](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementuserexperienceanalyticapphealthapplicationperformancebyappversiondeviceid)



