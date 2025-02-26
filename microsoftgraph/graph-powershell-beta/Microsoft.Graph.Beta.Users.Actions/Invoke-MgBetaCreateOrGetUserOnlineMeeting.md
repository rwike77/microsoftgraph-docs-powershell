---
external help file: Microsoft.Graph.Beta.Users.Actions-help.xml
Module Name: Microsoft.Graph.Beta.Users.Actions
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/invoke-mgbetacreateorgetuseronlinemeeting
schema: 2.0.0
ms.prod: cloud-communications
---

# Invoke-MgBetaCreateOrGetUserOnlineMeeting

## SYNOPSIS
Create an onlineMeeting object with a custom specified external ID.
If the external ID already exists, this API will return the onlineMeeting object with that external ID.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Invoke-MgCreateOrGetUserOnlineMeeting](/powershell/module/Microsoft.Graph.Users.Actions/Invoke-MgCreateOrGetUserOnlineMeeting?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
Invoke-MgBetaCreateOrGetUserOnlineMeeting -UserId <String> [-AdditionalProperties <Hashtable>]
 [-ChatInfo <IMicrosoftGraphChatInfo>] [-EndDateTime <DateTime>] [-ExternalId <String>]
 [-Participants <IMicrosoftGraphMeetingParticipants>] [-StartDateTime <DateTime>] [-Subject <String>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Create
```
Invoke-MgBetaCreateOrGetUserOnlineMeeting -UserId <String>
 -BodyParameter <IPaths1H47062UsersUserIdOnlinemeetingsMicrosoftGraphCreateorgetPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
Invoke-MgBetaCreateOrGetUserOnlineMeeting -InputObject <IUsersActionsIdentity>
 [-AdditionalProperties <Hashtable>] [-ChatInfo <IMicrosoftGraphChatInfo>] [-EndDateTime <DateTime>]
 [-ExternalId <String>] [-Participants <IMicrosoftGraphMeetingParticipants>] [-StartDateTime <DateTime>]
 [-Subject <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
Invoke-MgBetaCreateOrGetUserOnlineMeeting -InputObject <IUsersActionsIdentity>
 -BodyParameter <IPaths1H47062UsersUserIdOnlinemeetingsMicrosoftGraphCreateorgetPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create an onlineMeeting object with a custom specified external ID.
If the external ID already exists, this API will return the onlineMeeting object with that external ID.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Using the Invoke-MgBetaCreateOrGetUserOnlineMeeting Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Users.Actions
$params = @{
	StartDateTime = [System.DateTime]::Parse("2020-02-06T01:49:21.3524945+00:00")
	EndDateTime = [System.DateTime]::Parse("2020-02-06T02:19:21.3524945+00:00")
	Subject = "Create a meeting with customId provided"
	ExternalId = "7eb8263f-d0e0-4149-bb1c-1f0476083c56"
	Participants = @{
		Attendees = @(
			@{
				Identity = @{
					User = @{
						Id = "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
					}
				}
				Role = "presenter"
				Upn = "test1@contoso.com"
			}
		)
	}
}
# A UPN can also be used as -UserId.
Invoke-MgBetaCreateOrGetUserOnlineMeeting -UserId $userId -BodyParameter $params
```
This example shows how to use the Invoke-MgBetaCreateOrGetUserOnlineMeeting Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).
### Example 2: Using the Invoke-MgBetaCreateOrGetUserOnlineMeeting Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Users.Actions
$params = @{
	ChatInfo = @{
		ThreadId = "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2"
	}
	StartDateTime = [System.DateTime]::Parse("2020-02-06T01:49:21.3524945+00:00")
	EndDateTime = [System.DateTime]::Parse("2020-02-06T02:19:21.3524945+00:00")
	ExternalId = "7eb8263f-d0e0-4149-bb1c-1f0476083c56"
	Participants = @{
		Attendees = @(
			@{
				Identity = @{
					User = @{
						Id = "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
					}
				}
				Upn = "test1@contoso.com"
			}
		)
	}
	Subject = "Create a meeting with customId provided"
}
# A UPN can also be used as -UserId.
Invoke-MgBetaCreateOrGetUserOnlineMeeting -UserId $userId -BodyParameter $params
```
This example shows how to use the Invoke-MgBetaCreateOrGetUserOnlineMeeting Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

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
.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths1H47062UsersUserIdOnlinemeetingsMicrosoftGraphCreateorgetPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChatInfo
chatInfo
To construct, see NOTES section for CHATINFO properties and create a hash table.

```yaml
Type: IMicrosoftGraphChatInfo
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndDateTime
.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExternalId
.

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
Type: IUsersActionsIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Participants
meetingParticipants
To construct, see NOTES section for PARTICIPANTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMeetingParticipants
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartDateTime
.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subject
.

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

### -UserId
The unique identifier of user

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

### Microsoft.Graph.Beta.PowerShell.Models.IPaths1H47062UsersUserIdOnlinemeetingsMicrosoftGraphCreateorgetPostRequestbodyContentApplicationJsonSchema
### Microsoft.Graph.Beta.PowerShell.Models.IUsersActionsIdentity
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphOnlineMeeting
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPaths1H47062UsersUserIdOnlinemeetingsMicrosoftGraphCreateorgetPostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[ChatInfo \<IMicrosoftGraphChatInfo\>\]: chatInfo
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[MessageId \<String\>\]: The unique identifier for a message in a Microsoft Teams channel.
    \[ReplyChainMessageId \<String\>\]: The ID of the reply message.
    \[ThreadId \<String\>\]: The unique identifier for a thread in Microsoft Teams.
  \[EndDateTime \<DateTime?\>\]: 
  \[ExternalId \<String\>\]: 
  \[Participants \<IMicrosoftGraphMeetingParticipants\>\]: meetingParticipants
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Attendees \<IMicrosoftGraphMeetingParticipantInfo\[\]\>\]: Information of the meeting attendees.
      \[Identity \<IMicrosoftGraphIdentitySet\>\]: identitySet
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[Application \<IMicrosoftGraphIdentity\>\]: identity
          \[(Any) \<Object\>\]: This indicates any property can be added to this object.
          \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
          \[Id \<String\>\]: Unique identifier for the identity.
        \[Device \<IMicrosoftGraphIdentity\>\]: identity
        \[User \<IMicrosoftGraphIdentity\>\]: identity
      \[Role \<String\>\]: onlineMeetingRole
      \[Upn \<String\>\]: User principal name of the participant.
    \[Contributors \<IMicrosoftGraphMeetingParticipantInfo\[\]\>\]: 
    \[Organizer \<IMicrosoftGraphMeetingParticipantInfo\>\]: meetingParticipantInfo
    \[Producers \<IMicrosoftGraphMeetingParticipantInfo\[\]\>\]: 
  \[StartDateTime \<DateTime?\>\]: 
  \[Subject \<String\>\]: 

CHATINFO \<IMicrosoftGraphChatInfo\>: chatInfo
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[MessageId \<String\>\]: The unique identifier for a message in a Microsoft Teams channel.
  \[ReplyChainMessageId \<String\>\]: The ID of the reply message.
  \[ThreadId \<String\>\]: The unique identifier for a thread in Microsoft Teams.

INPUTOBJECT \<IUsersActionsIdentity\>: Identity Parameter
  \[AccessReviewInstanceId \<String\>\]: The unique identifier of accessReviewInstance
  \[AccessReviewStageId \<String\>\]: The unique identifier of accessReviewStage
  \[AppLogCollectionRequestId \<String\>\]: The unique identifier of appLogCollectionRequest
  \[AuthenticationMethodId \<String\>\]: The unique identifier of authenticationMethod
  \[CalendarId \<String\>\]: The unique identifier of calendar
  \[ChatId \<String\>\]: The unique identifier of chat
  \[ChatMessageId \<String\>\]: The unique identifier of chatMessage
  \[ChatMessageId1 \<String\>\]: The unique identifier of chatMessage
  \[CloudPcId \<String\>\]: The unique identifier of cloudPC
  \[ContentTypeId \<String\>\]: The unique identifier of contentType
  \[DeviceEnrollmentConfigurationId \<String\>\]: The unique identifier of deviceEnrollmentConfiguration
  \[DeviceLogCollectionResponseId \<String\>\]: The unique identifier of deviceLogCollectionResponse
  \[DocumentSetVersionId \<String\>\]: The unique identifier of documentSetVersion
  \[DriveId \<String\>\]: The unique identifier of drive
  \[DriveItemId \<String\>\]: The unique identifier of driveItem
  \[DriveItemVersionId \<String\>\]: The unique identifier of driveItemVersion
  \[EventId \<String\>\]: The unique identifier of event
  \[EventId1 \<String\>\]: The unique identifier of event
  \[ListItemId \<String\>\]: The unique identifier of listItem
  \[ListItemVersionId \<String\>\]: The unique identifier of listItemVersion
  \[MailFolderId \<String\>\]: The unique identifier of mailFolder
  \[MailFolderId1 \<String\>\]: The unique identifier of mailFolder
  \[ManagedDeviceId \<String\>\]: The unique identifier of managedDevice
  \[MessageId \<String\>\]: The unique identifier of message
  \[MobileAppTroubleshootingEventId \<String\>\]: The unique identifier of mobileAppTroubleshootingEvent
  \[NotebookId \<String\>\]: The unique identifier of notebook
  \[OnenotePageId \<String\>\]: The unique identifier of onenotePage
  \[OnenoteSectionId \<String\>\]: The unique identifier of onenoteSection
  \[OutlookTaskFolderId \<String\>\]: The unique identifier of outlookTaskFolder
  \[OutlookTaskGroupId \<String\>\]: The unique identifier of outlookTaskGroup
  \[OutlookTaskId \<String\>\]: The unique identifier of outlookTask
  \[PermissionId \<String\>\]: The unique identifier of permission
  \[PlannerPlanId \<String\>\]: The unique identifier of plannerPlan
  \[SensitivityLabelId \<String\>\]: The unique identifier of sensitivityLabel
  \[SubscriptionId \<String\>\]: The unique identifier of subscription
  \[TeamsAppInstallationId \<String\>\]: The unique identifier of teamsAppInstallation
  \[TodoTaskId \<String\>\]: The unique identifier of todoTask
  \[TodoTaskListId \<String\>\]: The unique identifier of todoTaskList
  \[UserId \<String\>\]: The unique identifier of user

PARTICIPANTS \<IMicrosoftGraphMeetingParticipants\>: meetingParticipants
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Attendees \<IMicrosoftGraphMeetingParticipantInfo\[\]\>\]: Information of the meeting attendees.
    \[Identity \<IMicrosoftGraphIdentitySet\>\]: identitySet
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[Application \<IMicrosoftGraphIdentity\>\]: identity
        \[(Any) \<Object\>\]: This indicates any property can be added to this object.
        \[DisplayName \<String\>\]: The display name of the identity.
This might not always be available or up to date.
For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
        \[Id \<String\>\]: Unique identifier for the identity.
      \[Device \<IMicrosoftGraphIdentity\>\]: identity
      \[User \<IMicrosoftGraphIdentity\>\]: identity
    \[Role \<String\>\]: onlineMeetingRole
    \[Upn \<String\>\]: User principal name of the participant.
  \[Contributors \<IMicrosoftGraphMeetingParticipantInfo\[\]\>\]: 
  \[Organizer \<IMicrosoftGraphMeetingParticipantInfo\>\]: meetingParticipantInfo
  \[Producers \<IMicrosoftGraphMeetingParticipantInfo\[\]\>\]:

## RELATED LINKS
[Invoke-MgCreateOrGetUserOnlineMeeting](/powershell/module/Microsoft.Graph.Users.Actions/Invoke-MgCreateOrGetUserOnlineMeeting?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/invoke-mgbetacreateorgetuseronlinemeeting](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.users.actions/invoke-mgbetacreateorgetuseronlinemeeting)


