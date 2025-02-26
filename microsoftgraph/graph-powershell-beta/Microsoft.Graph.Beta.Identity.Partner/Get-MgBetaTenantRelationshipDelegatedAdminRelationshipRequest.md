---
external help file: Microsoft.Graph.Beta.Identity.Partner-help.xml
Module Name: Microsoft.Graph.Beta.Identity.Partner
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.partner/get-mgbetatenantrelationshipdelegatedadminrelationshiprequest
schema: 2.0.0
ms.prod: partner-customer-administration
ms.prod: partner-customer-administration
---

# Get-MgBetaTenantRelationshipDelegatedAdminRelationshipRequest

## SYNOPSIS
Read the properties and relationships of a delegatedAdminRelationshipRequest object.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgTenantRelationshipDelegatedAdminRelationshipRequest](/powershell/module/Microsoft.Graph.Identity.Partner/Get-MgTenantRelationshipDelegatedAdminRelationshipRequest?view=graph-powershell-1.0)

## SYNTAX

### List (Default)
```
Get-MgBetaTenantRelationshipDelegatedAdminRelationshipRequest -DelegatedAdminRelationshipId <String>
 [-ExpandProperty <String[]>] [-Property <String[]>] [-Filter <String>] [-Search <String>] [-Skip <Int32>]
 [-Sort <String[]>] [-Top <Int32>] [-PageSize <Int32>] [-All] [-CountVariable <String>] [<CommonParameters>]
```

### Get
```
Get-MgBetaTenantRelationshipDelegatedAdminRelationshipRequest -DelegatedAdminRelationshipId <String>
 -DelegatedAdminRelationshipRequestId <String> [-ExpandProperty <String[]>] [-Property <String[]>]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaTenantRelationshipDelegatedAdminRelationshipRequest -InputObject <IIdentityPartnerIdentity>
 [-ExpandProperty <String[]>] [-Property <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Read the properties and relationships of a delegatedAdminRelationshipRequest object.
This API is available in the following national cloud deployments.

## PARAMETERS

### -All
List all pages.

```yaml
Type: SwitchParameter
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CountVariable
Specifies a count of the total number of items in a collection.
By default, this variable will be set in the global scope.

```yaml
Type: String
Parameter Sets: List
Aliases: CV

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DelegatedAdminRelationshipId
The unique identifier of delegatedAdminRelationship

```yaml
Type: String
Parameter Sets: List, Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DelegatedAdminRelationshipRequestId
The unique identifier of delegatedAdminRelationshipRequest

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

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: List
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
Type: IIdentityPartnerIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PageSize
Sets the page size of results.

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
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

### -Search
Search items by search phrases

```yaml
Type: String
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Sort
Order items by property values

```yaml
Type: String[]
Parameter Sets: List
Aliases: OrderBy

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Top
Show only the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases: Limit

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Skip
Skip the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IIdentityPartnerIdentity
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDelegatedAdminRelationshipRequest
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IIdentityPartnerIdentity\>: Identity Parameter
  \[DelegatedAdminAccessAssignmentId \<String\>\]: The unique identifier of delegatedAdminAccessAssignment
  \[DelegatedAdminCustomerId \<String\>\]: The unique identifier of delegatedAdminCustomer
  \[DelegatedAdminRelationshipId \<String\>\]: The unique identifier of delegatedAdminRelationship
  \[DelegatedAdminRelationshipOperationId \<String\>\]: The unique identifier of delegatedAdminRelationshipOperation
  \[DelegatedAdminRelationshipRequestId \<String\>\]: The unique identifier of delegatedAdminRelationshipRequest
  \[DelegatedAdminServiceManagementDetailId \<String\>\]: The unique identifier of delegatedAdminServiceManagementDetail

## RELATED LINKS
[Get-MgTenantRelationshipDelegatedAdminRelationshipRequest](/powershell/module/Microsoft.Graph.Identity.Partner/Get-MgTenantRelationshipDelegatedAdminRelationshipRequest?view=graph-powershell-1.0)

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.partner/get-mgbetatenantrelationshipdelegatedadminrelationshiprequest](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.partner/get-mgbetatenantrelationshipdelegatedadminrelationshiprequest)



