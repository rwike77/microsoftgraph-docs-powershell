---
external help file: Microsoft.Graph.Beta.Teams-help.xml
Module Name: Microsoft.Graph.Beta.Teams
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/new-mgbetateaminstalledapp
schema: 2.0.0
---

# New-MgBetaTeamInstalledApp

## SYNOPSIS
Install an app to the specified team.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgTeamInstalledApp](/powershell/module/Microsoft.Graph.Teams/New-MgTeamInstalledApp?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaTeamInstalledApp -TeamId <String> [-AdditionalProperties <Hashtable>]
 [-ConsentedPermissionSet <IMicrosoftGraphTeamsAppPermissionSet>] [-Id <String>]
 [-TeamsApp <IMicrosoftGraphTeamsApp>] [-TeamsAppDefinition <IMicrosoftGraphTeamsAppDefinition>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaTeamInstalledApp -TeamId <String> -BodyParameter <IMicrosoftGraphTeamsAppInstallation> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaTeamInstalledApp -InputObject <ITeamsIdentity> [-AdditionalProperties <Hashtable>]
 [-ConsentedPermissionSet <IMicrosoftGraphTeamsAppPermissionSet>] [-Id <String>]
 [-TeamsApp <IMicrosoftGraphTeamsApp>] [-TeamsAppDefinition <IMicrosoftGraphTeamsAppDefinition>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaTeamInstalledApp -InputObject <ITeamsIdentity> -BodyParameter <IMicrosoftGraphTeamsAppInstallation>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Install an app to the specified team.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Install app in a chat

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	"teamsApp@odata.bind" = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}

New-MgBetaTeamInstalledApp -TeamId $teamId -BodyParameter $params

```
This example will install app in a chat

### Example 2: Install app in a team and consent to the resource-specific permissions required by the app

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	"teamsApp@odata.bind" = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/7023576d-9e40-47ca-9cf2-daae6838e785"
	consentedPermissionSet = @{
		resourceSpecificPermissions = @(
			@{
				permissionValue = "OnlineMeeting.ReadBasic.Chat"
				permissionType = "delegated"
			}
			@{
				permissionValue = "ChatMessage.Read.Chat"
				permissionType = "application"
			}
		)
	}
}

New-MgBetaTeamInstalledApp -TeamId $teamId -BodyParameter $params

```
This example will install app in a team and consent to the resource-specific permissions required by the app


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
teamsAppInstallation
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamsAppInstallation
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ConsentedPermissionSet
teamsAppPermissionSet
To construct, see NOTES section for CONSENTEDPERMISSIONSET properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamsAppPermissionSet
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
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
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -TeamId
The unique identifier of team

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TeamsApp
teamsApp
To construct, see NOTES section for TEAMSAPP properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamsApp
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TeamsAppDefinition
teamsAppDefinition
To construct, see NOTES section for TEAMSAPPDEFINITION properties and create a hash table.

```yaml
Type: IMicrosoftGraphTeamsAppDefinition
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphTeamsAppInstallation
### Microsoft.Graph.Beta.PowerShell.Models.ITeamsIdentity
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphTeamsAppInstallation
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphTeamsAppInstallation\>: teamsAppInstallation
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[ConsentedPermissionSet \<IMicrosoftGraphTeamsAppPermissionSet\>\]: teamsAppPermissionSet
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[ResourceSpecificPermissions \<IMicrosoftGraphTeamsAppResourceSpecificPermission\[\]\>\]: A collection of resource-specific permissions.
      \[PermissionType \<String\>\]: teamsAppResourceSpecificPermissionType
      \[PermissionValue \<String\>\]: The name of the resource-specific permission.
  \[TeamsApp \<IMicrosoftGraphTeamsApp\>\]: teamsApp
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[AppDefinitions \<IMicrosoftGraphTeamsAppDefinition\[\]\>\]: The details for each version of the app.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[AllowedInstallationScopes \<String\>\]: teamsAppInstallationScopes
      \[Authorization \<IMicrosoftGraphTeamsAppAuthorization\>\]: teamsAppAuthorization
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[RequiredPermissionSet \<IMicrosoftGraphTeamsAppPermissionSet\>\]: teamsAppPermissionSet
      \[AzureAdAppId \<String\>\]: The WebApplicationInfo.Id from the Teams app manifest.
      \[Bot \<IMicrosoftGraphTeamworkBot\>\]: teamworkBot
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[ColorIcon \<IMicrosoftGraphTeamsAppIcon\>\]: teamsAppIcon
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
        \[HostedContent \<IMicrosoftGraphTeamworkHostedContent\>\]: teamworkHostedContent
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
          \[ContentBytes \<Byte\[\]\>\]: Write only.
Bytes for the hosted content (such as images).
          \[ContentType \<String\>\]: Write only.
Content type, such as image/png, image/jpg.
        \[WebUrl \<String\>\]: The web URL that can be used for downloading the image.
      \[CreatedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Application \<IMicrosoftGraphIdentity\>\]: identity
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
          \[Id \<String\>\]: Unique identifier for the identity.
        \[Device \<IMicrosoftGraphIdentity\>\]: identity
        \[User \<IMicrosoftGraphIdentity\>\]: identity
      \[Description \<String\>\]: 
      \[DisplayName \<String\>\]: The name of the app provided by the app developer.
      \[LastModifiedDateTime \<DateTime?\>\]: 
      \[OutlineIcon \<IMicrosoftGraphTeamsAppIcon\>\]: teamsAppIcon
      \[PublishingState \<String\>\]: teamsAppPublishingState
      \[Shortdescription \<String\>\]: 
      \[TeamsAppId \<String\>\]: The ID from the Teams app manifest.
      \[Version \<String\>\]: The version number of the application.
    \[DisplayName \<String\>\]: The name of the catalog app provided by the app developer in the Microsoft Teams zip app package.
    \[DistributionMethod \<String\>\]: teamsAppDistributionMethod
    \[ExternalId \<String\>\]: The ID of the catalog provided by the app developer in the Microsoft Teams zip app package.
  \[TeamsAppDefinition \<IMicrosoftGraphTeamsAppDefinition\>\]: teamsAppDefinition

CONSENTEDPERMISSIONSET \<IMicrosoftGraphTeamsAppPermissionSet\>: teamsAppPermissionSet
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[ResourceSpecificPermissions \<IMicrosoftGraphTeamsAppResourceSpecificPermission\[\]\>\]: A collection of resource-specific permissions.
    \[PermissionType \<String\>\]: teamsAppResourceSpecificPermissionType
    \[PermissionValue \<String\>\]: The name of the resource-specific permission.

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

TEAMSAPP \<IMicrosoftGraphTeamsApp\>: teamsApp
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AppDefinitions \<IMicrosoftGraphTeamsAppDefinition\[\]\>\]: The details for each version of the app.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[AllowedInstallationScopes \<String\>\]: teamsAppInstallationScopes
    \[Authorization \<IMicrosoftGraphTeamsAppAuthorization\>\]: teamsAppAuthorization
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[RequiredPermissionSet \<IMicrosoftGraphTeamsAppPermissionSet\>\]: teamsAppPermissionSet
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[ResourceSpecificPermissions \<IMicrosoftGraphTeamsAppResourceSpecificPermission\[\]\>\]: A collection of resource-specific permissions.
          \[PermissionType \<String\>\]: teamsAppResourceSpecificPermissionType
          \[PermissionValue \<String\>\]: The name of the resource-specific permission.
    \[AzureAdAppId \<String\>\]: The WebApplicationInfo.Id from the Teams app manifest.
    \[Bot \<IMicrosoftGraphTeamworkBot\>\]: teamworkBot
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[ColorIcon \<IMicrosoftGraphTeamsAppIcon\>\]: teamsAppIcon
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[HostedContent \<IMicrosoftGraphTeamworkHostedContent\>\]: teamworkHostedContent
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
        \[ContentBytes \<Byte\[\]\>\]: Write only.
Bytes for the hosted content (such as images).
        \[ContentType \<String\>\]: Write only.
Content type, such as image/png, image/jpg.
      \[WebUrl \<String\>\]: The web URL that can be used for downloading the image.
    \[CreatedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Application \<IMicrosoftGraphIdentity\>\]: identity
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
        \[Id \<String\>\]: Unique identifier for the identity.
      \[Device \<IMicrosoftGraphIdentity\>\]: identity
      \[User \<IMicrosoftGraphIdentity\>\]: identity
    \[Description \<String\>\]: 
    \[DisplayName \<String\>\]: The name of the app provided by the app developer.
    \[LastModifiedDateTime \<DateTime?\>\]: 
    \[OutlineIcon \<IMicrosoftGraphTeamsAppIcon\>\]: teamsAppIcon
    \[PublishingState \<String\>\]: teamsAppPublishingState
    \[Shortdescription \<String\>\]: 
    \[TeamsAppId \<String\>\]: The ID from the Teams app manifest.
    \[Version \<String\>\]: The version number of the application.
  \[DisplayName \<String\>\]: The name of the catalog app provided by the app developer in the Microsoft Teams zip app package.
  \[DistributionMethod \<String\>\]: teamsAppDistributionMethod
  \[ExternalId \<String\>\]: The ID of the catalog provided by the app developer in the Microsoft Teams zip app package.

TEAMSAPPDEFINITION \<IMicrosoftGraphTeamsAppDefinition\>: teamsAppDefinition
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AllowedInstallationScopes \<String\>\]: teamsAppInstallationScopes
  \[Authorization \<IMicrosoftGraphTeamsAppAuthorization\>\]: teamsAppAuthorization
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[RequiredPermissionSet \<IMicrosoftGraphTeamsAppPermissionSet\>\]: teamsAppPermissionSet
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[ResourceSpecificPermissions \<IMicrosoftGraphTeamsAppResourceSpecificPermission\[\]\>\]: A collection of resource-specific permissions.
        \[PermissionType \<String\>\]: teamsAppResourceSpecificPermissionType
        \[PermissionValue \<String\>\]: The name of the resource-specific permission.
  \[AzureAdAppId \<String\>\]: The WebApplicationInfo.Id from the Teams app manifest.
  \[Bot \<IMicrosoftGraphTeamworkBot\>\]: teamworkBot
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[ColorIcon \<IMicrosoftGraphTeamsAppIcon\>\]: teamsAppIcon
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
    \[HostedContent \<IMicrosoftGraphTeamworkHostedContent\>\]: teamworkHostedContent
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
      \[ContentBytes \<Byte\[\]\>\]: Write only.
Bytes for the hosted content (such as images).
      \[ContentType \<String\>\]: Write only.
Content type, such as image/png, image/jpg.
    \[WebUrl \<String\>\]: The web URL that can be used for downloading the image.
  \[CreatedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Application \<IMicrosoftGraphIdentity\>\]: identity
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      \[Id \<String\>\]: Unique identifier for the identity.
    \[Device \<IMicrosoftGraphIdentity\>\]: identity
    \[User \<IMicrosoftGraphIdentity\>\]: identity
  \[Description \<String\>\]: 
  \[DisplayName \<String\>\]: The name of the app provided by the app developer.
  \[LastModifiedDateTime \<DateTime?\>\]: 
  \[OutlineIcon \<IMicrosoftGraphTeamsAppIcon\>\]: teamsAppIcon
  \[PublishingState \<String\>\]: teamsAppPublishingState
  \[Shortdescription \<String\>\]: 
  \[TeamsAppId \<String\>\]: The ID from the Teams app manifest.
  \[Version \<String\>\]: The version number of the application.

## RELATED LINKS
[New-MgTeamInstalledApp](/powershell/module/Microsoft.Graph.Teams/New-MgTeamInstalledApp?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/new-mgbetateaminstalledapp](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.teams/new-mgbetateaminstalledapp)


