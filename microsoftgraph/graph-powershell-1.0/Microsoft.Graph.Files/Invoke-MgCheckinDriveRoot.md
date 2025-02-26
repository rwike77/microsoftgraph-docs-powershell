---
external help file: Microsoft.Graph.Files-help.xml
Module Name: Microsoft.Graph.Files
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.files/invoke-mgcheckindriveroot
schema: 2.0.0
ms.prod: sharepoint
---

# Invoke-MgCheckinDriveRoot

## SYNOPSIS
Check in a checked out driveItem resource, which makes the version of the document available to others.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [Invoke-MgBetaCheckinDriveRoot](/powershell/module/Microsoft.Graph.Beta.Files/Invoke-MgBetaCheckinDriveRoot?view=graph-powershell-beta)

## SYNTAX

### CheckinExpanded (Default)
```
Invoke-MgCheckinDriveRoot -DriveId <String> [-AdditionalProperties <Hashtable>] [-CheckInAs <String>]
 [-Comment <String>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Checkin
```
Invoke-MgCheckinDriveRoot -DriveId <String>
 -Body <IPathsW65Kj4DrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CheckinViaIdentityExpanded
```
Invoke-MgCheckinDriveRoot -InputObject <IFilesIdentity> [-AdditionalProperties <Hashtable>]
 [-CheckInAs <String>] [-Comment <String>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CheckinViaIdentity
```
Invoke-MgCheckinDriveRoot -InputObject <IFilesIdentity>
 -BodyParameter <IPathsW65Kj4DrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Check in a checked out driveItem resource, which makes the version of the document available to others.
This API is available in the following national cloud deployments.

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CheckinExpanded, CheckinViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Body
.
To construct, see NOTES section for BODY properties and create a hash table.

```yaml
Type: IPathsW65Kj4DrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Checkin
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPathsW65Kj4DrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema
Parameter Sets: CheckinViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CheckInAs
.

```yaml
Type: String
Parameter Sets: CheckinExpanded, CheckinViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Comment
.

```yaml
Type: String
Parameter Sets: CheckinExpanded, CheckinViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DriveId
The unique identifier of drive

```yaml
Type: String
Parameter Sets: CheckinExpanded, Checkin
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
Type: IFilesIdentity
Parameter Sets: CheckinViaIdentityExpanded, CheckinViaIdentity
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

### Microsoft.Graph.PowerShell.Models.IFilesIdentity
### Microsoft.Graph.PowerShell.Models.IPathsW65Kj4DrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODY \<IPathsW65Kj4DrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[CheckInAs \<String\>\]: 
  \[Comment \<String\>\]: 

BODYPARAMETER \<IPathsW65Kj4DrivesDriveIdRootMicrosoftGraphCheckinPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[CheckInAs \<String\>\]: 
  \[Comment \<String\>\]: 

INPUTOBJECT \<IFilesIdentity\>: Identity Parameter
  \[ColumnDefinitionId \<String\>\]: The unique identifier of columnDefinition
  \[ColumnLinkId \<String\>\]: The unique identifier of columnLink
  \[ContentTypeId \<String\>\]: The unique identifier of contentType
  \[ContentTypeId1 \<String\>\]: The unique identifier of contentType
  \[DocumentSetVersionId \<String\>\]: The unique identifier of documentSetVersion
  \[DriveId \<String\>\]: The unique identifier of drive
  \[DriveItemId \<String\>\]: The unique identifier of driveItem
  \[DriveItemId1 \<String\>\]: The unique identifier of driveItem
  \[DriveItemVersionId \<String\>\]: The unique identifier of driveItemVersion
  \[EndDateTime \<String\>\]: Usage: endDateTime='{endDateTime}'
  \[GroupId \<String\>\]: The unique identifier of group
  \[Interval \<String\>\]: Usage: interval='{interval}'
  \[ItemActivityStatId \<String\>\]: The unique identifier of itemActivityStat
  \[ListItemId \<String\>\]: The unique identifier of listItem
  \[ListItemVersionId \<String\>\]: The unique identifier of listItemVersion
  \[PermissionId \<String\>\]: The unique identifier of permission
  \[Q \<String\>\]: Usage: q='{q}'
  \[RichLongRunningOperationId \<String\>\]: The unique identifier of richLongRunningOperation
  \[SharedDriveItemId \<String\>\]: The unique identifier of sharedDriveItem
  \[StartDateTime \<String\>\]: Usage: startDateTime='{startDateTime}'
  \[SubscriptionId \<String\>\]: The unique identifier of subscription
  \[ThumbnailSetId \<String\>\]: The unique identifier of thumbnailSet
  \[Token \<String\>\]: Usage: token='{token}'
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[Invoke-MgBetaCheckinDriveRoot](/powershell/module/Microsoft.Graph.Beta.Files/Invoke-MgBetaCheckinDriveRoot?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.files/invoke-mgcheckindriveroot](https://learn.microsoft.com/powershell/module/microsoft.graph.files/invoke-mgcheckindriveroot)



