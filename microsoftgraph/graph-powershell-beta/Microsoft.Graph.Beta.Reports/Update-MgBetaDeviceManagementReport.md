---
external help file: Microsoft.Graph.Beta.Reports-help.xml
Module Name: Microsoft.Graph.Beta.Reports
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/update-mgbetadevicemanagementreport
schema: 2.0.0
---

# Update-MgBetaDeviceManagementReport

## SYNOPSIS
Update the navigation property reports in deviceManagement

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgDeviceManagementReport](/powershell/module/Microsoft.Graph.Reports/Update-MgDeviceManagementReport?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaDeviceManagementReport [-AdditionalProperties <Hashtable>]
 [-CachedReportConfigurations <IMicrosoftGraphDeviceManagementCachedReportConfiguration[]>]
 [-ExportJobs <IMicrosoftGraphDeviceManagementExportJob[]>] [-Id <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Update
```
Update-MgBetaDeviceManagementReport -BodyParameter <IMicrosoftGraphDeviceManagementReports> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property reports in deviceManagement

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
Singleton entity that acts as a container for all reports functionality.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceManagementReports
Parameter Sets: Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CachedReportConfigurations
Entity representing the configuration of a cached report
To construct, see NOTES section for CACHEDREPORTCONFIGURATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceManagementCachedReportConfiguration[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExportJobs
Entity representing a job to export a report
To construct, see NOTES section for EXPORTJOBS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceManagementExportJob[]
Parameter Sets: UpdateExpanded
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
Parameter Sets: UpdateExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDeviceManagementReports
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDeviceManagementReports
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphDeviceManagementReports\>: Singleton entity that acts as a container for all reports functionality.
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[CachedReportConfigurations \<IMicrosoftGraphDeviceManagementCachedReportConfiguration\[\]\>\]: Entity representing the configuration of a cached report
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Filter \<String\>\]: Filters applied on report creation.
    \[Metadata \<String\>\]: Caller-managed metadata associated with the report
    \[OrderBy \<String\[\]\>\]: Ordering of columns in the report
    \[Select \<String\[\]\>\]: Columns selected from the report
    \[Status \<DeviceManagementReportStatus?\>\]: Possible statuses associated with a generated report
  \[ExportJobs \<IMicrosoftGraphDeviceManagementExportJob\[\]\>\]: Entity representing a job to export a report
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[Filter \<String\>\]: Filters applied on the report
    \[Format \<DeviceManagementReportFileFormat?\>\]: Possible values for the file format of a report
    \[LocalizationType \<DeviceManagementExportJobLocalizationType?\>\]: Configures how the requested export job is localized
    \[ReportName \<String\>\]: Name of the report
    \[Select \<String\[\]\>\]: Columns selected from the report
    \[SnapshotId \<String\>\]: A snapshot is an identifiable subset of the dataset represented by the ReportName.
A sessionId or CachedReportConfiguration id can be used here.
If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.
Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.
    \[Status \<DeviceManagementReportStatus?\>\]: Possible statuses associated with a generated report

CACHEDREPORTCONFIGURATIONS \<IMicrosoftGraphDeviceManagementCachedReportConfiguration\[\]\>: Entity representing the configuration of a cached report
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Filter \<String\>\]: Filters applied on report creation.
  \[Metadata \<String\>\]: Caller-managed metadata associated with the report
  \[OrderBy \<String\[\]\>\]: Ordering of columns in the report
  \[Select \<String\[\]\>\]: Columns selected from the report
  \[Status \<DeviceManagementReportStatus?\>\]: Possible statuses associated with a generated report

EXPORTJOBS \<IMicrosoftGraphDeviceManagementExportJob\[\]\>: Entity representing a job to export a report
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[Filter \<String\>\]: Filters applied on the report
  \[Format \<DeviceManagementReportFileFormat?\>\]: Possible values for the file format of a report
  \[LocalizationType \<DeviceManagementExportJobLocalizationType?\>\]: Configures how the requested export job is localized
  \[ReportName \<String\>\]: Name of the report
  \[Select \<String\[\]\>\]: Columns selected from the report
  \[SnapshotId \<String\>\]: A snapshot is an identifiable subset of the dataset represented by the ReportName.
A sessionId or CachedReportConfiguration id can be used here.
If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.
Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.
  \[Status \<DeviceManagementReportStatus?\>\]: Possible statuses associated with a generated report

## RELATED LINKS
[Update-MgDeviceManagementReport](/powershell/module/Microsoft.Graph.Reports/Update-MgDeviceManagementReport?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/update-mgbetadevicemanagementreport](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.reports/update-mgbetadevicemanagementreport)


