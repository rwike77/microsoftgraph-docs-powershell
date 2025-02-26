---
external help file: Microsoft.Graph.Beta.DeviceManagement.Administration-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement.Administration
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.administration/new-mgbetadevicemanagementvirtualendpointreportexportjob
schema: 2.0.0
ms.prod: cloud-pc
---

# New-MgBetaDeviceManagementVirtualEndpointReportExportJob

## SYNOPSIS
Create a new cloudPcExportJob resource to initiate downloading the entire or specified portion of a report.
Use the GET cloudPcExportJob operation to verify the exportJobStatus property of the cloudPcExportJob resource.
When the property result is completed, the report has finished downloading to the location specified by the exportUrl property.
This API is available in the following national cloud deployments.

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaDeviceManagementVirtualEndpointReportExportJob [-AdditionalProperties <Hashtable>]
 [-ExpirationDateTime <DateTime>] [-ExportJobStatus <String>] [-ExportUrl <String>] [-Filter <String>]
 [-Format <String>] [-Id <String>] [-Property <String[]>] [-ReportName <String>] [-RequestDateTime <DateTime>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaDeviceManagementVirtualEndpointReportExportJob -BodyParameter <IMicrosoftGraphCloudPcExportJob>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new cloudPcExportJob resource to initiate downloading the entire or specified portion of a report.
Use the GET cloudPcExportJob operation to verify the exportJobStatus property of the cloudPcExportJob resource.
When the property result is completed, the report has finished downloading to the location specified by the exportUrl property.
This API is available in the following national cloud deployments.

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

### -BodyParameter
cloudPcExportJob
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphCloudPcExportJob
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ExpirationDateTime
The date and time when the export job expires.

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

### -ExportJobStatus
cloudPcExportJobStatus

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

### -ExportUrl
The storage account URL of the exported report.
It can be used to download the file.

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

### -Filter
The filter applied on the report.

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

### -Format
The format of the exported report.

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

### -Property
The selected columns of the report.

```yaml
Type: String[]
Parameter Sets: CreateExpanded
Aliases: Select

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReportName
cloudPcReportName

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

### -RequestDateTime
The date and time when the export job was requested.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphCloudPcExportJob
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphCloudPcExportJob
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphCloudPcExportJob\>: cloudPcExportJob
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[ExpirationDateTime \<DateTime?\>\]: The date and time when the export job expires.
  \[ExportJobStatus \<String\>\]: cloudPcExportJobStatus
  \[ExportUrl \<String\>\]: The storage account URL of the exported report.
It can be used to download the file.
  \[Filter \<String\>\]: The filter applied on the report.
  \[Format \<String\>\]: The format of the exported report.
  \[ReportName \<String\>\]: cloudPcReportName
  \[RequestDateTime \<DateTime?\>\]: The date and time when the export job was requested.
  \[Select \<String\[\]\>\]: The selected columns of the report.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.administration/new-mgbetadevicemanagementvirtualendpointreportexportjob](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.administration/new-mgbetadevicemanagementvirtualendpointreportexportjob)



