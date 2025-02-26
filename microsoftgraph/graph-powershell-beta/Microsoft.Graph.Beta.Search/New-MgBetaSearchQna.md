---
external help file: Microsoft.Graph.Beta.Search-help.xml
Module Name: Microsoft.Graph.Beta.Search
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/new-mgbetasearchqna
schema: 2.0.0
ms.prod: search
---

# New-MgBetaSearchQna

## SYNOPSIS
Create a new qna object.
This API is available in the following national cloud deployments.

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaSearchQna [-AdditionalProperties <Hashtable>] [-AvailabilityEndDateTime <DateTime>]
 [-AvailabilityStartDateTime <DateTime>] [-Description <String>] [-DisplayName <String>] [-GroupIds <String[]>]
 [-Id <String>] [-IsSuggested] [-Keywords <IMicrosoftGraphSearchAnswerKeyword>] [-LanguageTags <String[]>]
 [-LastModifiedBy <IMicrosoftGraphSearchIdentitySet>] [-LastModifiedDateTime <DateTime>]
 [-Platforms <DevicePlatformType[]>] [-State <String>]
 [-TargetedVariations <IMicrosoftGraphSearchAnswerVariant[]>] [-WebUrl <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create
```
New-MgBetaSearchQna -BodyParameter <IMicrosoftGraphSearchQna> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new qna object.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Using the New-MgBetaSearchQna Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Search
$params = @{
	DisplayName = "Global Country Holidays"
	WebUrl = "http://www.contoso.com/"
	Description = "The dates that Contoso offices will be closed to observe holidays. These dates may differ from the actual date of the holiday in cases where the holiday falls on a wee​kend.    <table>    <thead>    <tr>    <td><strong>2021 Dates</strong></td>    <td><strong>Holiday</strong></td>    </tr>    </thead>    <tbody>    <tr>        <td>January 1, 2021</td>        <td>New Year's Day</td>    </tr>        <tr>        <td>January 18, 2021</td>        <td>Martin Luther King Day</td>    </tr>        <tr>        <td>February 15, 2021</td>        <td>Presidents Day</td>    </tr>        <tr>        <td>May 31, 2021</td>        <td>Memorial Day</td>    </tr>        <tr>        <td>July 5, 2021</td>        <td>Independence Day</td>    </tr>        <tr>        <td>September 6, 2021</td>        <td>Labor Day</td>    </tr>        <tr>        <td>November 25, 2021 - November 26, 2021</td>        <td>Thanksgiving Day and Day after Thanksgiving</td>    </tr>    <tr>        <td>December 23, 2021 - December 24, 2021</td>        <td>Christmas Eve and Christmas Day</td>    </tr>    </tbody>    </table>"
	Keywords = @{
		Keywords = @(
			"new years day"
			"martin luther king day"
			"presidents day"
			"memorial day"
			"independence day"
			"labor day"
			"thanksgiving"
			"christmas"
		)
		ReservedKeywords = @(
			"holidays"
			"paid days off"
		)
		MatchSimilarKeywords = $true
	}
	AvailabilityStartDateTime = [System.DateTime]::Parse("2020-09-21T20:01:37Z")
	AvailabilityEndDateTime = [System.DateTime]::Parse("2021-12-31T20:01:37Z")
	LanguageTags = @(
		"en-us"
	)
	Platforms = @(
		"ios"
	)
	State = "published"
}
New-MgBetaSearchQna -BodyParameter $params
```
This example shows how to use the New-MgBetaSearchQna Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AvailabilityEndDateTime
Timestamp of when the qna stops to appear as a search result.
Set as null for always available.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AvailabilityStartDateTime
Timestamp of when the qna starts to appear as a search result.
Set as null for always available.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
qna
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSearchQna
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Description
Search answer description shown on search results page.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
Search answer name displayed in search results.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupIds
List of security groups able to view this qna.

```yaml
Type: String[]
Parameter Sets: CreateExpanded
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
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsSuggested
True if a user or Microsoft suggested this qna to the admin.
Read-only.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Keywords
answerKeyword
To construct, see NOTES section for KEYWORDS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSearchAnswerKeyword
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LanguageTags
A list of language names that are geographically specific and that this QnA can be viewed in.
Each language tag value follows the pattern {language}-{region}.
As an example, en-us is English as used in the United States.
For the list of possible values, see supported language tags.

```yaml
Type: String[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedBy
identitySet
To construct, see NOTES section for LASTMODIFIEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphSearchIdentitySet
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
Timestamp of when the search answer is created or edited.
Read-only.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Platforms
List of devices and operating systems able to view this qna.
Possible values are: unknown, android, androidForWork, ios, macOS, windowsPhone81, windowsPhone81AndLater, windows10AndLater, androidWorkProfile, androidASOP.

```yaml
Type: DevicePlatformType[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -State
answerState

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetedVariations
Variations of a qna for different countries or devices.
Use when you need to show different content to users based on their device, country/region, or both.
The date and group settings apply to all variations.
To construct, see NOTES section for TARGETEDVARIATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSearchAnswerVariant[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebUrl
Search answer URL link.
When users click this search answer in search results, they'll go to this URL.

```yaml
Type: String
Parameter Sets: CreateExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSearchQna
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSearchQna
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphSearchQna\>: qna
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Description \<String\>\]: Search answer description shown on search results page.
  \[DisplayName \<String\>\]: Search answer name displayed in search results.
  \[LastModifiedBy \<IMicrosoftGraphSearchIdentitySet\>\]: identitySet
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Application \<IMicrosoftGraphSearchIdentity\>\]: identity
      \[(Any) \<Object\>\]: This indicates any property can be added to this object.
      \[DisplayName \<String\>\]: 
      \[Id \<String\>\]: 
    \[Device \<IMicrosoftGraphSearchIdentity\>\]: identity
    \[User \<IMicrosoftGraphSearchIdentity\>\]: identity
  \[LastModifiedDateTime \<DateTime?\>\]: Timestamp of when the search answer is created or edited.
Read-only.
  \[WebUrl \<String\>\]: Search answer URL link.
When users click this search answer in search results, they'll go to this URL.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[AvailabilityEndDateTime \<DateTime?\>\]: Timestamp of when the qna stops to appear as a search result.
Set as null for always available.
  \[AvailabilityStartDateTime \<DateTime?\>\]: Timestamp of when the qna starts to appear as a search result.
Set as null for always available.
  \[GroupIds \<String\[\]\>\]: List of security groups able to view this qna.
  \[IsSuggested \<Boolean?\>\]: True if a user or Microsoft suggested this qna to the admin.
Read-only.
  \[Keywords \<IMicrosoftGraphSearchAnswerKeyword\>\]: answerKeyword
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[Keywords \<String\[\]\>\]: A collection of keywords used to trigger the search answer.
    \[MatchSimilarKeywords \<Boolean?\>\]: If true, indicates that the search term contains similar words to the keywords that should trigger the search answer.
    \[ReservedKeywords \<String\[\]\>\]: Unique keywords that will guarantee the search answer is triggered.
  \[LanguageTags \<String\[\]\>\]: A list of language names that are geographically specific and that this QnA can be viewed in.
Each language tag value follows the pattern {language}-{region}.
As an example, en-us is English as used in the United States.
For the list of possible values, see supported language tags.
  \[Platforms \<DevicePlatformType\[\]\>\]: List of devices and operating systems able to view this qna.
Possible values are: unknown, android, androidForWork, ios, macOS, windowsPhone81, windowsPhone81AndLater, windows10AndLater, androidWorkProfile, androidASOP.
  \[State \<String\>\]: answerState
  \[TargetedVariations \<IMicrosoftGraphSearchAnswerVariant\[\]\>\]: Variations of a qna for different countries or devices.
Use when you need to show different content to users based on their device, country/region, or both.
The date and group settings apply to all variations.
    \[Description \<String\>\]: Answer variation description shown on search results page.
    \[DisplayName \<String\>\]: Answer variation name displayed in search results.
    \[LanguageTag \<String\>\]: 
    \[Platform \<DevicePlatformType?\>\]: Supported platform types.
    \[WebUrl \<String\>\]: Answer variation URL link.
When users click this answer variation in search results, they will go to this URL.

KEYWORDS \<IMicrosoftGraphSearchAnswerKeyword\>: answerKeyword
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Keywords \<String\[\]\>\]: A collection of keywords used to trigger the search answer.
  \[MatchSimilarKeywords \<Boolean?\>\]: If true, indicates that the search term contains similar words to the keywords that should trigger the search answer.
  \[ReservedKeywords \<String\[\]\>\]: Unique keywords that will guarantee the search answer is triggered.

LASTMODIFIEDBY \<IMicrosoftGraphSearchIdentitySet\>: identitySet
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Application \<IMicrosoftGraphSearchIdentity\>\]: identity
    \[(Any) \<Object\>\]: This indicates any property can be added to this object.
    \[DisplayName \<String\>\]: 
    \[Id \<String\>\]: 
  \[Device \<IMicrosoftGraphSearchIdentity\>\]: identity
  \[User \<IMicrosoftGraphSearchIdentity\>\]: identity

TARGETEDVARIATIONS \<IMicrosoftGraphSearchAnswerVariant\[\]\>: Variations of a qna for different countries or devices.
Use when you need to show different content to users based on their device, country/region, or both.
The date and group settings apply to all variations.
  \[Description \<String\>\]: Answer variation description shown on search results page.
  \[DisplayName \<String\>\]: Answer variation name displayed in search results.
  \[LanguageTag \<String\>\]: 
  \[Platform \<DevicePlatformType?\>\]: Supported platform types.
  \[WebUrl \<String\>\]: Answer variation URL link.
When users click this answer variation in search results, they will go to this URL.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/new-mgbetasearchqna](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/new-mgbetasearchqna)

