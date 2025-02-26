---
external help file: Microsoft.Graph.People-help.xml
Module Name: Microsoft.Graph.People
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.people/get-mguserusedresourceinsight
schema: 2.0.0
---

# Get-MgUserUsedResourceInsight

## SYNOPSIS
Used for navigating to the item that was used.
For file attachments, the type is fileAttachment.
For linked attachments, the type is driveItem.

## SYNTAX

### Get (Default)
```
Get-MgUserUsedResourceInsight -UsedInsightId <String> -UserId <String> [-ExpandProperty <String[]>]
 [-Property <String[]>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgUserUsedResourceInsight -InputObject <IPeopleIdentity> [-ExpandProperty <String[]>]
 [-Property <String[]>] [<CommonParameters>]
```

## DESCRIPTION
Used for navigating to the item that was used.
For file attachments, the type is fileAttachment.
For linked attachments, the type is driveItem.

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IPeopleIdentity
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

### -UsedInsightId
The unique identifier of usedInsight

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

### -UserId
The unique identifier of user

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IPeopleIdentity
## OUTPUTS

### System.String
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT \<IPeopleIdentity\>: Identity Parameter
  \[PersonId \<String\>\]: The unique identifier of person
  \[SharedInsightId \<String\>\]: The unique identifier of sharedInsight
  \[TrendingId \<String\>\]: The unique identifier of trending
  \[UsedInsightId \<String\>\]: The unique identifier of usedInsight
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.people/get-mguserusedresourceinsight](https://learn.microsoft.com/powershell/module/microsoft.graph.people/get-mguserusedresourceinsight)



