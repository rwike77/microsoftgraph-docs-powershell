---
external help file: Microsoft.Graph.Beta.Search-help.xml
Module Name: Microsoft.Graph.Beta.Search
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/get-mgbetaexternalconnectionschema
schema: 2.0.0
ms.prod: search
---

# Get-MgBetaExternalConnectionSchema

## SYNOPSIS
Retrieve the properties of a schema for an externalConnection.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgExternalConnectionSchema](/powershell/module/Microsoft.Graph.Search/Get-MgExternalConnectionSchema?view=graph-powershell-1.0)

## SYNTAX

### Get (Default)
```
Get-MgBetaExternalConnectionSchema -ExternalConnectionId <String> [-ExpandProperty <String[]>]
 [-Property <String[]>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaExternalConnectionSchema -InputObject <ISearchIdentity> [-ExpandProperty <String[]>]
 [-Property <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Retrieve the properties of a schema for an externalConnection.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Search

Get-MgBetaExternalConnectionSchema -ExternalConnectionId $externalConnectionId

```
This example shows how to use the Get-MgBetaExternalConnectionSchema Cmdlet.


## PARAMETERS

### -ExpandProperty
Expand related entities

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Expand

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExternalConnectionId
The unique identifier of externalConnection

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
Type: ISearchIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Select

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.ISearchIdentity
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphExternalConnectorsSchema
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<ISearchIdentity\>: Identity Parameter
  \[AcronymId \<String\>\]: The unique identifier of acronym
  \[AuthorizationSystemId \<String\>\]: The unique identifier of authorizationSystem
  \[BookmarkId \<String\>\]: The unique identifier of bookmark
  \[ConnectionOperationId \<String\>\]: The unique identifier of connectionOperation
  \[ExternalActivityId \<String\>\]: The unique identifier of externalActivity
  \[ExternalConnectionId \<String\>\]: The unique identifier of externalConnection
  \[ExternalGroupId \<String\>\]: The unique identifier of externalGroup
  \[ExternalItemId \<String\>\]: The unique identifier of externalItem
  \[IdentityId \<String\>\]: The unique identifier of identity
  \[InboundFlowId \<String\>\]: The unique identifier of inboundFlow
  \[IndustryDataConnectorId \<String\>\]: The unique identifier of industryDataConnector
  \[IndustryDataRunActivityId \<String\>\]: The unique identifier of industryDataRunActivity
  \[IndustryDataRunId \<String\>\]: The unique identifier of industryDataRun
  \[LongRunningOperationId \<String\>\]: The unique identifier of longRunningOperation
  \[QnaId \<String\>\]: The unique identifier of qna
  \[ReferenceDefinitionId \<String\>\]: The unique identifier of referenceDefinition
  \[RoleGroupId \<String\>\]: The unique identifier of roleGroup
  \[SourceSystemDefinitionId \<String\>\]: The unique identifier of sourceSystemDefinition
  \[YearTimePeriodDefinitionId \<String\>\]: The unique identifier of yearTimePeriodDefinition

## RELATED LINKS
[Get-MgExternalConnectionSchema](/powershell/module/Microsoft.Graph.Search/Get-MgExternalConnectionSchema?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/get-mgbetaexternalconnectionschema](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/get-mgbetaexternalconnectionschema)


