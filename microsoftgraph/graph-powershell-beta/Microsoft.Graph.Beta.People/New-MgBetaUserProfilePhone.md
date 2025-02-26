---
external help file: Microsoft.Graph.Beta.People-help.xml
Module Name: Microsoft.Graph.Beta.People
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.people/new-mgbetauserprofilephone
schema: 2.0.0
ms.prod: people
---

# New-MgBetaUserProfilePhone

## SYNOPSIS
Use this API to create a new itemPhone object in a user's profile.
This API is available in the following national cloud deployments.

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaUserProfilePhone -UserId <String> [-AdditionalProperties <Hashtable>] [-AllowedAudiences <String>]
 [-CreatedBy <IMicrosoftGraphIdentitySet>] [-CreatedDateTime <DateTime>] [-DisplayName <String>] [-Id <String>]
 [-Inference <IMicrosoftGraphInferenceData>] [-IsSearchable] [-LastModifiedBy <IMicrosoftGraphIdentitySet>]
 [-LastModifiedDateTime <DateTime>] [-Number <String>] [-Source <IMicrosoftGraphPersonDataSources>]
 [-Type <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaUserProfilePhone -UserId <String> -BodyParameter <IMicrosoftGraphItemPhone> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaUserProfilePhone -InputObject <IPeopleIdentity> [-AdditionalProperties <Hashtable>]
 [-AllowedAudiences <String>] [-CreatedBy <IMicrosoftGraphIdentitySet>] [-CreatedDateTime <DateTime>]
 [-DisplayName <String>] [-Id <String>] [-Inference <IMicrosoftGraphInferenceData>] [-IsSearchable]
 [-LastModifiedBy <IMicrosoftGraphIdentitySet>] [-LastModifiedDateTime <DateTime>] [-Number <String>]
 [-Source <IMicrosoftGraphPersonDataSources>] [-Type <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaUserProfilePhone -InputObject <IPeopleIdentity> -BodyParameter <IMicrosoftGraphItemPhone> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Use this API to create a new itemPhone object in a user's profile.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Using the New-MgBetaUserProfilePhone Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.People
$params = @{
	DisplayName = "Car Phone"
	Number = "+7 499 342 22 13"
}
# A UPN can also be used as -UserId.
New-MgBetaUserProfilePhone -UserId $userId -BodyParameter $params
```
This example shows how to use the New-MgBetaUserProfilePhone Cmdlet.
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

### -AllowedAudiences
allowedAudiences

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

### -BodyParameter
itemPhone
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphItemPhone
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CreatedBy
identitySet
To construct, see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
Provides the dateTimeOffset for when the entity was created.

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

### -DisplayName
Friendly name the user has assigned this phone number.

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

### -Inference
inferenceData
To construct, see NOTES section for INFERENCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphInferenceData
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
Type: IPeopleIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsSearchable
.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedBy
identitySet
To construct, see NOTES section for LASTMODIFIEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
Provides the dateTimeOffset for when the entity was created.

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

### -Number
Phone number provided by the user.

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

### -Source
personDataSources
To construct, see NOTES section for SOURCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphPersonDataSources
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Type
phoneType

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphItemPhone
### Microsoft.Graph.Beta.PowerShell.Models.IPeopleIdentity
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphItemPhone
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphItemPhone\>: itemPhone
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[AllowedAudiences \<String\>\]: allowedAudiences
  \[CreatedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Application \<IMicrosoftGraphIdentity\>\]: identity
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[DisplayName \<String\>\]: The display name of the identity.
This property is read-only.
      \[Id \<String\>\]: The identifier of the identity.
This property is read-only.
    \[Device \<IMicrosoftGraphIdentity\>\]: identity
    \[User \<IMicrosoftGraphIdentity\>\]: identity
  \[CreatedDateTime \<DateTime?\>\]: Provides the dateTimeOffset for when the entity was created.
  \[Inference \<IMicrosoftGraphInferenceData\>\]: inferenceData
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[ConfidenceScore \<Double?\>\]: Confidence score reflecting the accuracy of the data inferred about the user.
    \[UserHasVerifiedAccuracy \<Boolean?\>\]: Records if the user has confirmed this inference as being True or False.
  \[IsSearchable \<Boolean?\>\]: 
  \[LastModifiedBy \<IMicrosoftGraphIdentitySet\>\]: identitySet
  \[LastModifiedDateTime \<DateTime?\>\]: Provides the dateTimeOffset for when the entity was created.
  \[Source \<IMicrosoftGraphPersonDataSources\>\]: personDataSources
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Type \<String\[\]\>\]: 
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[DisplayName \<String\>\]: Friendly name the user has assigned this phone number.
  \[Number \<String\>\]: Phone number provided by the user.
  \[Type \<String\>\]: phoneType

CREATEDBY \<IMicrosoftGraphIdentitySet\>: identitySet
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Application \<IMicrosoftGraphIdentity\>\]: identity
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[DisplayName \<String\>\]: The display name of the identity.
This property is read-only.
    \[Id \<String\>\]: The identifier of the identity.
This property is read-only.
  \[Device \<IMicrosoftGraphIdentity\>\]: identity
  \[User \<IMicrosoftGraphIdentity\>\]: identity

INFERENCE \<IMicrosoftGraphInferenceData\>: inferenceData
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[ConfidenceScore \<Double?\>\]: Confidence score reflecting the accuracy of the data inferred about the user.
  \[UserHasVerifiedAccuracy \<Boolean?\>\]: Records if the user has confirmed this inference as being True or False.

INPUTOBJECT \<IPeopleIdentity\>: Identity Parameter
  \[ActivityStatisticsId \<String\>\]: The unique identifier of activityStatistics
  \[EducationalActivityId \<String\>\]: The unique identifier of educationalActivity
  \[ItemAddressId \<String\>\]: The unique identifier of itemAddress
  \[ItemEmailId \<String\>\]: The unique identifier of itemEmail
  \[ItemPatentId \<String\>\]: The unique identifier of itemPatent
  \[ItemPhoneId \<String\>\]: The unique identifier of itemPhone
  \[ItemPublicationId \<String\>\]: The unique identifier of itemPublication
  \[LanguageProficiencyId \<String\>\]: The unique identifier of languageProficiency
  \[PersonAnnotationId \<String\>\]: The unique identifier of personAnnotation
  \[PersonAnnualEventId \<String\>\]: The unique identifier of personAnnualEvent
  \[PersonAwardId \<String\>\]: The unique identifier of personAward
  \[PersonCertificationId \<String\>\]: The unique identifier of personCertification
  \[PersonId \<String\>\]: The unique identifier of person
  \[PersonInterestId \<String\>\]: The unique identifier of personInterest
  \[PersonNameId \<String\>\]: The unique identifier of personName
  \[PersonWebsiteId \<String\>\]: The unique identifier of personWebsite
  \[ProjectParticipationId \<String\>\]: The unique identifier of projectParticipation
  \[SkillProficiencyId \<String\>\]: The unique identifier of skillProficiency
  \[UserAccountInformationId \<String\>\]: The unique identifier of userAccountInformation
  \[UserId \<String\>\]: The unique identifier of user
  \[WebAccountId \<String\>\]: The unique identifier of webAccount
  \[WorkPositionId \<String\>\]: The unique identifier of workPosition

LASTMODIFIEDBY \<IMicrosoftGraphIdentitySet\>: identitySet
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Application \<IMicrosoftGraphIdentity\>\]: identity
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[DisplayName \<String\>\]: The display name of the identity.
This property is read-only.
    \[Id \<String\>\]: The identifier of the identity.
This property is read-only.
  \[Device \<IMicrosoftGraphIdentity\>\]: identity
  \[User \<IMicrosoftGraphIdentity\>\]: identity

SOURCE \<IMicrosoftGraphPersonDataSources\>: personDataSources
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Type \<String\[\]\>\]:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.people/new-mgbetauserprofilephone](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.people/new-mgbetauserprofilephone)


