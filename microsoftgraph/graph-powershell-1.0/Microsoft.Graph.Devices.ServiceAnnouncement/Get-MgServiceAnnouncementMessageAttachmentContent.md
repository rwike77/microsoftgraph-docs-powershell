---
external help file: Microsoft.Graph.Devices.ServiceAnnouncement-help.xml
Module Name: Microsoft.Graph.Devices.ServiceAnnouncement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devices.serviceannouncement/get-mgserviceannouncementmessageattachmentcontent
schema: 2.0.0
ms.prod: service-communications
---

# Get-MgServiceAnnouncementMessageAttachmentContent

## SYNOPSIS
The attachment content.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaServiceAnnouncementMessageAttachmentContent](/powershell/module/Microsoft.Graph.Beta.Devices.ServiceAnnouncement/Get-MgBetaServiceAnnouncementMessageAttachmentContent?view=graph-powershell-beta)

## SYNTAX

### Get (Default)
```
Get-MgServiceAnnouncementMessageAttachmentContent -ServiceAnnouncementAttachmentId <String>
 -ServiceUpdateMessageId <String> -OutFile <String> [-PassThru] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgServiceAnnouncementMessageAttachmentContent -InputObject <IDevicesServiceAnnouncementIdentity>
 -OutFile <String> [-PassThru] [<CommonParameters>]
```

## DESCRIPTION
The attachment content.

## EXAMPLES

## PARAMETERS

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IDevicesServiceAnnouncementIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OutFile
Path to write output file to

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
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

### -ServiceAnnouncementAttachmentId
The unique identifier of serviceAnnouncementAttachment

```yaml
Type: String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceUpdateMessageId
The unique identifier of serviceUpdateMessage

```yaml
Type: String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IDevicesServiceAnnouncementIdentity
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IDevicesServiceAnnouncementIdentity\>: Identity Parameter
  \[ServiceAnnouncementAttachmentId \<String\>\]: The unique identifier of serviceAnnouncementAttachment
  \[ServiceHealthId \<String\>\]: The unique identifier of serviceHealth
  \[ServiceHealthIssueId \<String\>\]: The unique identifier of serviceHealthIssue
  \[ServiceUpdateMessageId \<String\>\]: The unique identifier of serviceUpdateMessage

## RELATED LINKS
[Get-MgBetaServiceAnnouncementMessageAttachmentContent](/powershell/module/Microsoft.Graph.Beta.Devices.ServiceAnnouncement/Get-MgBetaServiceAnnouncementMessageAttachmentContent?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.devices.serviceannouncement/get-mgserviceannouncementmessageattachmentcontent](https://learn.microsoft.com/powershell/module/microsoft.graph.devices.serviceannouncement/get-mgserviceannouncementmessageattachmentcontent)


