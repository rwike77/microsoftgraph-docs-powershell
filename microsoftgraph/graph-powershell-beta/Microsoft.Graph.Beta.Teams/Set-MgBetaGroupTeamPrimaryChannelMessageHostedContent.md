---
external help file: Microsoft.Graph.Beta.Teams-help.xml
Module Name: Microsoft.Graph.Beta.Teams
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/set-mgbetagroupteamprimarychannelmessagehostedcontent
schema: 2.0.0
---

# Set-MgBetaGroupTeamPrimaryChannelMessageHostedContent

## SYNOPSIS
Update media content for the navigation property hostedContents in groups

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Set-MgGroupTeamPrimaryChannelMessageHostedContent](/powershell/module/Microsoft.Graph.Teams/Set-MgGroupTeamPrimaryChannelMessageHostedContent?view=graph-powershell-1.0)

## SYNTAX

### Set (Default)
```
Set-MgBetaGroupTeamPrimaryChannelMessageHostedContent -ChatMessageHostedContentId <String>
 -ChatMessageId <String> -GroupId <String> [-Data <Stream>] -InFile <String> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### SetViaIdentity
```
Set-MgBetaGroupTeamPrimaryChannelMessageHostedContent -InputObject <ITeamsIdentity> [-Data <Stream>]
 -InFile <String> [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update media content for the navigation property hostedContents in groups

## PARAMETERS

### -ChatMessageHostedContentId
The unique identifier of chatMessageHostedContent

```yaml
Type: String
Parameter Sets: Set
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ChatMessageId
The unique identifier of chatMessage

```yaml
Type: String
Parameter Sets: Set
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Data
.

```yaml
Type: Stream
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -GroupId
The unique identifier of group

```yaml
Type: String
Parameter Sets: Set
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InFile
The path to the file to upload.
This should include a path and file name.
If you omit the path, the current location will be used.

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: ITeamsIdentity
Parameter Sets: SetViaIdentity
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

### Microsoft.Graph.Beta.PowerShell.Models.ITeamsIdentity
### System.IO.Stream
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<ITeamsIdentity\>: Identity Parameter
  \[AssociatedTeamInfoId \<String\>\]: The unique identifier of associatedTeamInfo
  \[ChannelId \<String\>\]: The unique identifier of channel
  \[ChatId \<String\>\]: The unique identifier of chat
  \[ChatMessageHostedContentId \<String\>\]: The unique identifier of chatMessageHostedContent
  \[ChatMessageId \<String\>\]: The unique identifier of chatMessage
  \[ChatMessageId1 \<String\>\]: The unique identifier of chatMessage
  \[ConversationMemberId \<String\>\]: The unique identifier of conversationMember
  \[DeletedChatId \<String\>\]: The unique identifier of deletedChat
  \[DeletedTeamId \<String\>\]: The unique identifier of deletedTeam
  \[GroupId \<String\>\]: The unique identifier of group
  \[OfferShiftRequestId \<String\>\]: The unique identifier of offerShiftRequest
  \[OpenShiftChangeRequestId \<String\>\]: The unique identifier of openShiftChangeRequest
  \[OpenShiftId \<String\>\]: The unique identifier of openShift
  \[PinnedChatMessageInfoId \<String\>\]: The unique identifier of pinnedChatMessageInfo
  \[ResourceSpecificPermissionGrantId \<String\>\]: The unique identifier of resourceSpecificPermissionGrant
  \[SchedulingGroupId \<String\>\]: The unique identifier of schedulingGroup
  \[SharedWithChannelTeamInfoId \<String\>\]: The unique identifier of sharedWithChannelTeamInfo
  \[ShiftId \<String\>\]: The unique identifier of shift
  \[SwapShiftsChangeRequestId \<String\>\]: The unique identifier of swapShiftsChangeRequest
  \[TeamId \<String\>\]: The unique identifier of team
  \[TeamTemplateDefinitionId \<String\>\]: The unique identifier of teamTemplateDefinition
  \[TeamTemplateId \<String\>\]: The unique identifier of teamTemplate
  \[TeamsAppDefinitionId \<String\>\]: The unique identifier of teamsAppDefinition
  \[TeamsAppId \<String\>\]: The unique identifier of teamsApp
  \[TeamsAppInstallationId \<String\>\]: The unique identifier of teamsAppInstallation
  \[TeamsAsyncOperationId \<String\>\]: The unique identifier of teamsAsyncOperation
  \[TeamsTabId \<String\>\]: The unique identifier of teamsTab
  \[TeamworkDeviceId \<String\>\]: The unique identifier of teamworkDevice
  \[TeamworkDeviceOperationId \<String\>\]: The unique identifier of teamworkDeviceOperation
  \[TeamworkTagId \<String\>\]: The unique identifier of teamworkTag
  \[TeamworkTagMemberId \<String\>\]: The unique identifier of teamworkTagMember
  \[TimeCardId \<String\>\]: The unique identifier of timeCard
  \[TimeOffId \<String\>\]: The unique identifier of timeOff
  \[TimeOffReasonId \<String\>\]: The unique identifier of timeOffReason
  \[TimeOffRequestId \<String\>\]: The unique identifier of timeOffRequest
  \[UserId \<String\>\]: The unique identifier of user
  \[UserScopeTeamsAppInstallationId \<String\>\]: The unique identifier of userScopeTeamsAppInstallation
  \[WorkforceIntegrationId \<String\>\]: The unique identifier of workforceIntegration

## RELATED LINKS
[Set-MgGroupTeamPrimaryChannelMessageHostedContent](/powershell/module/Microsoft.Graph.Teams/Set-MgGroupTeamPrimaryChannelMessageHostedContent?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/set-mgbetagroupteamprimarychannelmessagehostedcontent](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/set-mgbetagroupteamprimarychannelmessagehostedcontent)



