---
external help file: Microsoft.Graph.Beta.People-help.xml
Module Name: Microsoft.Graph.Beta.People
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.people/new-mgbetauserprofilepublication
schema: 2.0.0
ms.prod: people 
---

# New-MgBetaUserProfilePublication

## SYNOPSIS
Create a new itemPublication object in a user's profile.
This API is available in the following national cloud deployments.

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaUserProfilePublication -UserId <String> [-AdditionalProperties <Hashtable>]
 [-AllowedAudiences <String>] [-CreatedBy <IMicrosoftGraphIdentitySet>] [-CreatedDateTime <DateTime>]
 [-Description <String>] [-DisplayName <String>] [-Id <String>] [-Inference <IMicrosoftGraphInferenceData>]
 [-IsSearchable] [-LastModifiedBy <IMicrosoftGraphIdentitySet>] [-LastModifiedDateTime <DateTime>]
 [-PublishedDate <DateTime>] [-Publisher <String>] [-Source <IMicrosoftGraphPersonDataSources>]
 [-ThumbnailUrl <String>] [-WebUrl <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaUserProfilePublication -UserId <String> -BodyParameter <IMicrosoftGraphItemPublication> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaUserProfilePublication -InputObject <IPeopleIdentity> [-AdditionalProperties <Hashtable>]
 [-AllowedAudiences <String>] [-CreatedBy <IMicrosoftGraphIdentitySet>] [-CreatedDateTime <DateTime>]
 [-Description <String>] [-DisplayName <String>] [-Id <String>] [-Inference <IMicrosoftGraphInferenceData>]
 [-IsSearchable] [-LastModifiedBy <IMicrosoftGraphIdentitySet>] [-LastModifiedDateTime <DateTime>]
 [-PublishedDate <DateTime>] [-Publisher <String>] [-Source <IMicrosoftGraphPersonDataSources>]
 [-ThumbnailUrl <String>] [-WebUrl <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaUserProfilePublication -InputObject <IPeopleIdentity> -BodyParameter <IMicrosoftGraphItemPublication>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new itemPublication object in a user's profile.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Using the New-MgBetaUserProfilePublication Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.People
$params = @{
	Description = "One persons journey to the top of the branding management field."
	DisplayName = "Got Brands? The story of Innocenty Popov and his journey to the top."
	PublishedDate = "Date"
	Publisher = "International Association of Branding Management Publishing"
	ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
	WebUrl = "https://www.iabm.io"
}
# A UPN can also be used as -UserId.
New-MgBetaUserProfilePublication -UserId $userId -BodyParameter $params
```
This example shows how to use the New-MgBetaUserProfilePublication Cmdlet.
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
itemPublication
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphItemPublication
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

### -Description
Description of the publication.

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

### -DisplayName
Title of the publication.

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

### -PublishedDate
The date that the publication was published.

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

### -Publisher
Publication or publisher for the publication.

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

### -ThumbnailUrl
URL referencing a thumbnail of the publication.

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

### -WebUrl
URL referencing the publication.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphItemPublication
### Microsoft.Graph.Beta.PowerShell.Models.IPeopleIdentity
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphItemPublication
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphItemPublication\>: itemPublication
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
  \[Description \<String\>\]: Description of the publication.
  \[DisplayName \<String\>\]: Title of the publication.
  \[PublishedDate \<DateTime?\>\]: The date that the publication was published.
  \[Publisher \<String\>\]: Publication or publisher for the publication.
  \[ThumbnailUrl \<String\>\]: URL referencing a thumbnail of the publication.
  \[WebUrl \<String\>\]: URL referencing the publication.

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

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.people/new-mgbetauserprofilepublication](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.people/new-mgbetauserprofilepublication)


