---
external help file: Microsoft.Graph.Users-help.xml
Module Name: Microsoft.Graph.Users
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.users/new-mgusertodolisttaskchecklistitem
schema: 2.0.0
ms.prod: outlook
---

# New-MgUserTodoListTaskChecklistItem

## SYNOPSIS
Create a new checklistItem object.
This API is available in the following national cloud deployments.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaUserTodoListTaskChecklistItem](/powershell/module/Microsoft.Graph.Beta.Users/New-MgBetaUserTodoListTaskChecklistItem?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgUserTodoListTaskChecklistItem -TodoTaskId <String> -TodoTaskListId <String> -UserId <String>
 [-AdditionalProperties <Hashtable>] [-CheckedDateTime <DateTime>] [-CreatedDateTime <DateTime>]
 [-DisplayName <String>] [-Id <String>] [-IsChecked] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgUserTodoListTaskChecklistItem -TodoTaskId <String> -TodoTaskListId <String> -UserId <String>
 -BodyParameter <IMicrosoftGraphChecklistItem> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgUserTodoListTaskChecklistItem -InputObject <IUsersIdentity> [-AdditionalProperties <Hashtable>]
 [-CheckedDateTime <DateTime>] [-CreatedDateTime <DateTime>] [-DisplayName <String>] [-Id <String>]
 [-IsChecked] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgUserTodoListTaskChecklistItem -InputObject <IUsersIdentity> -BodyParameter <IMicrosoftGraphChecklistItem>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new checklistItem object.
This API is available in the following national cloud deployments.

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.Users

$params = @{
	displayName = "Final sign-off from the team"
}

# A UPN can also be used as -UserId.
New-MgUserTodoListTaskChecklistItem -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -BodyParameter $params
```
This example shows how to use the New-MgUserTodoListTaskChecklistItem Cmdlet.

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
checklistItem
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphChecklistItem
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CheckedDateTime
The date and time when the checklistItem was finished.

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

### -CreatedDateTime
The date and time when the checklistItem was created.

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
Field indicating the title of checklistItem.

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IUsersIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsChecked
State indicating whether the item is checked off or not.

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

### -TodoTaskId
The unique identifier of todoTask

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

### -TodoTaskListId
The unique identifier of todoTaskList

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphChecklistItem
### Microsoft.Graph.PowerShell.Models.IUsersIdentity
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphChecklistItem
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER \<IMicrosoftGraphChecklistItem\>: checklistItem
  \[(Any) \<Object\>\]: This indicates any property can be added to this object.
  \[Id \<String\>\]: The unique identifier for an entity.
Read-only.
  \[CheckedDateTime \<DateTime?\>\]: The date and time when the checklistItem was finished.
  \[CreatedDateTime \<DateTime?\>\]: The date and time when the checklistItem was created.
  \[DisplayName \<String\>\]: Field indicating the title of checklistItem.
  \[IsChecked \<Boolean?\>\]: State indicating whether the item is checked off or not.

INPUTOBJECT \<IUsersIdentity\>: Identity Parameter
  \[AttachmentBaseId \<String\>\]: The unique identifier of attachmentBase
  \[AttachmentSessionId \<String\>\]: The unique identifier of attachmentSession
  \[ChecklistItemId \<String\>\]: The unique identifier of checklistItem
  \[DirectoryObjectId \<String\>\]: The unique identifier of directoryObject
  \[ExtensionId \<String\>\]: The unique identifier of extension
  \[LicenseDetailsId \<String\>\]: The unique identifier of licenseDetails
  \[LinkedResourceId \<String\>\]: The unique identifier of linkedResource
  \[OAuth2PermissionGrantId \<String\>\]: The unique identifier of oAuth2PermissionGrant
  \[OutlookCategoryId \<String\>\]: The unique identifier of outlookCategory
  \[ProfilePhotoId \<String\>\]: The unique identifier of profilePhoto
  \[TodoTaskId \<String\>\]: The unique identifier of todoTask
  \[TodoTaskListId \<String\>\]: The unique identifier of todoTaskList
  \[UserId \<String\>\]: The unique identifier of user

## RELATED LINKS
[New-MgBetaUserTodoListTaskChecklistItem](/powershell/module/Microsoft.Graph.Beta.Users/New-MgBetaUserTodoListTaskChecklistItem?view=graph-powershell-beta)

[https://learn.microsoft.com/powershell/module/microsoft.graph.users/new-mgusertodolisttaskchecklistitem](https://learn.microsoft.com/powershell/module/microsoft.graph.users/new-mgusertodolisttaskchecklistitem)



