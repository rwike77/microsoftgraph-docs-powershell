---
external help file: Microsoft.Graph.Calendar-help.xml
Module Name: Microsoft.Graph.Calendar
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.calendar/get-mggroupeventattachmentcount
schema: 2.0.0
---

# Get-MgGroupEventAttachmentCount

## SYNOPSIS
Get the number of the resource

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaGroupEventAttachmentCount](/powershell/module/Microsoft.Graph.Beta.Calendar/Get-MgBetaGroupEventAttachmentCount?view=graph-powershell-beta)

## SYNTAX

### Get (Default)
```
Get-MgGroupEventAttachmentCount -EventId <String> -GroupId <String> [-Filter <String>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgGroupEventAttachmentCount -InputObject <ICalendarIdentity> [-Filter <String>] [<CommonParameters>]
```

## DESCRIPTION
Get the number of the resource

## PARAMETERS

### -EventId
The unique identifier of event

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

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupId
The unique identifier of group

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: ICalendarIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.ICalendarIdentity
## OUTPUTS

### System.Int32
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<ICalendarIdentity\>: Identity Parameter
  \[AttachmentId \<String\>\]: The unique identifier of attachment
  \[CalendarGroupId \<String\>\]: The unique identifier of calendarGroup
  \[CalendarId \<String\>\]: The unique identifier of calendar
  \[CalendarPermissionId \<String\>\]: The unique identifier of calendarPermission
  \[EventId \<String\>\]: The unique identifier of event
  \[EventId1 \<String\>\]: The unique identifier of event
  \[ExtensionId \<String\>\]: The unique identifier of extension
  \[GroupId \<String\>\]: The unique identifier of group
  \[PlaceId \<String\>\]: The unique identifier of place
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[Get-MgBetaGroupEventAttachmentCount](/powershell/module/Microsoft.Graph.Beta.Calendar/Get-MgBetaGroupEventAttachmentCount?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.calendar/get-mggroupeventattachmentcount](https://learn.microsoft.com/powershell/module/microsoft.graph.calendar/get-mggroupeventattachmentcount)



