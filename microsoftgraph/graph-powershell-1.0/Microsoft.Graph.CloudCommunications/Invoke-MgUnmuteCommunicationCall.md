---
external help file: Microsoft.Graph.CloudCommunications-help.xml
Module Name: Microsoft.Graph.CloudCommunications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/invoke-mgunmutecommunicationcall
schema: 2.0.0
ms.prod: cloud-communications
---

# Invoke-MgUnmuteCommunicationCall

## SYNOPSIS
Allow the application to unmute itself.
This is a server unmute, meaning that the server will start sending audio packets for this participant to other participants again.
For more information about how to handle unmute operations, see unmuteParticipantOperation.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [Invoke-MgBetaUnmuteCommunicationCall](/powershell/module/Microsoft.Graph.Beta.CloudCommunications/Invoke-MgBetaUnmuteCommunicationCall?view=graph-powershell-beta)

## SYNTAX

### UnmuteExpanded (Default)
```
Invoke-MgUnmuteCommunicationCall -CallId <String> [-AdditionalProperties <Hashtable>] [-ClientContext <String>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Unmute
```
Invoke-MgUnmuteCommunicationCall -CallId <String>
 -BodyParameter <IPaths1X7BvttCommunicationsCallsCallIdMicrosoftGraphUnmutePostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UnmuteViaIdentityExpanded
```
Invoke-MgUnmuteCommunicationCall -InputObject <ICloudCommunicationsIdentity>
 [-AdditionalProperties <Hashtable>] [-ClientContext <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UnmuteViaIdentity
```
Invoke-MgUnmuteCommunicationCall -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IPaths1X7BvttCommunicationsCallsCallIdMicrosoftGraphUnmutePostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Allow the application to unmute itself.
This is a server unmute, meaning that the server will start sending audio packets for this participant to other participants again.
For more information about how to handle unmute operations, see unmuteParticipantOperation.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	clientContext = "clientContext-value"
}

Invoke-MgUnmuteCommunicationCall -CallId $callId -BodyParameter $params

```
This example shows how to use the Invoke-MgUnmuteCommunicationCall Cmdlet.


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UnmuteExpanded, UnmuteViaIdentityExpanded
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
Type: IPaths1X7BvttCommunicationsCallsCallIdMicrosoftGraphUnmutePostRequestbodyContentApplicationJsonSchema
Parameter Sets: Unmute, UnmuteViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CallId
The unique identifier of call

```yaml
Type: String
Parameter Sets: UnmuteExpanded, Unmute
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClientContext
.

```yaml
Type: String
Parameter Sets: UnmuteExpanded, UnmuteViaIdentityExpanded
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
Type: ICloudCommunicationsIdentity
Parameter Sets: UnmuteViaIdentityExpanded, UnmuteViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### Microsoft.Graph.PowerShell.Models.ICloudCommunicationsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths1X7BvttCommunicationsCallsCallIdMicrosoftGraphUnmutePostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphUnmuteParticipantOperation
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IPaths1X7BvttCommunicationsCallsCallIdMicrosoftGraphUnmutePostRequestbodyContentApplicationJsonSchema\>: .
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[ClientContext \<String\>\]: 

INPUTOBJECT \<ICloudCommunicationsIdentity\>: Identity Parameter
  \[AttendanceRecordId \<String\>\]: The unique identifier of attendanceRecord
  \[AudioRoutingGroupId \<String\>\]: The unique identifier of audioRoutingGroup
  \[CallId \<String\>\]: The unique identifier of call
  \[CallRecordId \<String\>\]: The unique identifier of callRecord
  \[CallTranscriptId \<String\>\]: The unique identifier of callTranscript
  \[CommsOperationId \<String\>\]: The unique identifier of commsOperation
  \[ContentSharingSessionId \<String\>\]: The unique identifier of contentSharingSession
  \[MeetingAttendanceReportId \<String\>\]: The unique identifier of meetingAttendanceReport
  \[OnlineMeetingId \<String\>\]: The unique identifier of onlineMeeting
  \[ParticipantId \<String\>\]: The unique identifier of participant
  \[PresenceId \<String\>\]: The unique identifier of presence
  \[SessionId \<String\>\]: The unique identifier of session
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[Invoke-MgBetaUnmuteCommunicationCall](/powershell/module/Microsoft.Graph.Beta.CloudCommunications/Invoke-MgBetaUnmuteCommunicationCall?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/invoke-mgunmutecommunicationcall](https://learn.microsoft.com/powershell/module/microsoft.graph.cloudcommunications/invoke-mgunmutecommunicationcall)


