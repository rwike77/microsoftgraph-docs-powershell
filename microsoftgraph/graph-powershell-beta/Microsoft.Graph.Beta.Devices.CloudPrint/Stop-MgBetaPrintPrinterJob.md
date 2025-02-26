---
external help file: Microsoft.Graph.Beta.Devices.CloudPrint-help.xml
Module Name: Microsoft.Graph.Beta.Devices.CloudPrint
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.cloudprint/stop-mgbetaprintprinterjob
schema: 2.0.0
ms.prod: cloud-printing
---

# Stop-MgBetaPrintPrinterJob

## SYNOPSIS
Cancel a print job.
Print jobs can be canceled only on behalf of a user, using delegated permissions.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Stop-MgPrintPrinterJob](/powershell/module/Microsoft.Graph.Devices.CloudPrint/Stop-MgPrintPrinterJob?view=graph-powershell-1.0)

## SYNTAX

### Cancel (Default)
```
Stop-MgBetaPrintPrinterJob -PrintJobId <String> -PrinterId <String> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### CancelViaIdentity
```
Stop-MgBetaPrintPrinterJob -InputObject <IDevicesCloudPrintIdentity> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Cancel a print job.
Print jobs can be canceled only on behalf of a user, using delegated permissions.
This API is available in the following national cloud deployments.

## PARAMETERS

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IDevicesCloudPrintIdentity
Parameter Sets: CancelViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -PrinterId
The unique identifier of printer

```yaml
Type: String
Parameter Sets: Cancel
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PrintJobId
The unique identifier of printJob

```yaml
Type: String
Parameter Sets: Cancel
Aliases:

Required: True
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

### Microsoft.Graph.Beta.PowerShell.Models.IDevicesCloudPrintIdentity
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IDevicesCloudPrintIdentity\>: Identity Parameter
  \[GroupId \<String\>\]: The unique identifier of group
  \[PrintConnectorId \<String\>\]: The unique identifier of printConnector
  \[PrintDocumentId \<String\>\]: The unique identifier of printDocument
  \[PrintJobId \<String\>\]: The unique identifier of printJob
  \[PrintOperationId \<String\>\]: The unique identifier of printOperation
  \[PrintServiceEndpointId \<String\>\]: The unique identifier of printServiceEndpoint
  \[PrintServiceId \<String\>\]: The unique identifier of printService
  \[PrintTaskDefinitionId \<String\>\]: The unique identifier of printTaskDefinition
  \[PrintTaskId \<String\>\]: The unique identifier of printTask
  \[PrintTaskTriggerId \<String\>\]: The unique identifier of printTaskTrigger
  \[PrinterId \<String\>\]: The unique identifier of printer
  \[PrinterShareId \<String\>\]: The unique identifier of printerShare
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[Stop-MgPrintPrinterJob](/powershell/module/Microsoft.Graph.Devices.CloudPrint/Stop-MgPrintPrinterJob?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.cloudprint/stop-mgbetaprintprinterjob](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.cloudprint/stop-mgbetaprintprinterjob)



