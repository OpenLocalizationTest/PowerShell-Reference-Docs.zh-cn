---
external help file: RMAzure_Automation.xml
online version: 19472f94-5827-4878-a17a-d7bb10932861
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxXxxxxxxxxxXxxXxxxXxxxxx
## XXXXXXXX
Xxxx xxxxxxx xxxx xxxx x XXX xxxx xx Xxxxxxxxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
Get-AzureRmAutomationDscNodeReport [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-EndTime <DateTimeOffset]>] [-StartTime <DateTimeOffset]>] -NodeId <Guid>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Get-AzureRmAutomationDscNodeReport [-ResourceGroupName] <String> [-AutomationAccountName] <String> -Id <Guid>
 -NodeId <Guid>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Get-AzureRmAutomationDscNodeReport [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Latest]
 -NodeId <Guid>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxXxxxXxxxxx$$ xxxxxx xxxx xxxxxxx xxxx xxxx xx XXX Xxxxxxx Xxxxx Xxxxxxxxxxxxx $XXX$ xxxx xx xxxxx$0 Xxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxxxxx xxx x XXX xxxx
```
PS C:\>$Node = Get-AzureRmAutomationDscNode -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -Name "Computer14"
PS C:\> Get-AzureRmAutomationDscNodeReport -ResourceGroupName "ResourceGroup14" -AutomationAccountName "Contoso17" -NodeId $Node.Id
```

Xxx xxxxx xxxxxxx xxxx xxx XXX xxxx xxx xxx xxxxxxxx xxxxx Xxxxxxxx00 xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.
Xxx xxxxxxx xxxxxx xxxx xxxxxx xx xxx $Xxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxxxxxxx xxx xxx xxxxxxx xxxx xxxx xxx XXX xxxx xxxxx Xxxxxxxx00 xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.
Xxx xxxxxxx xxxxxxxxx xxx xxxx xx xxxxx xxx $$Xx$$ xxxxxxxx xx xxx $Xxxx xxxxxx.

### Xxxxxxx 0$ Xxx x xxxxxx xxx x XXX xxxx xx xxxxxx XX
```
PS C:\>$Node = Get-AzureRmAutomationDscNode -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -Name "Computer14"
PS C:\> Get-AzureRmAutomationDscNodeReport -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -NodeId $Node.Id -Id c0a1718e-d8be-4fa3-91b6-82e1d3a36298
```

Xxx xxxxx xxxxxxx xxxx xxx XXX xxxx xxx xxx xxxxxxxx xxxxx Xxxxxxxx00 xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.
Xxx xxxxxxx xxxxxx xxxx xxxxxx xx xxx $Xxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxxxxxxx xxx xxx xxxxxx xxxxxxxxxx xx xxx xxxxxxxxx XX xxxx xxxx xxx XXX xxxx xxxxx Xxxxxxxx00 xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

### Xxxxxxx 0$ Xxx xxx xxxxxx xxxxxx xxx x XXX xxxx
```
PS C:\>$Node = Get-AzureRmAutomationDscNode -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -Name "Computer14"
PS C:\> Get-AzureRmAutomationDscNodeReport -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -NodeId $Node.Id -Latest
```

Xxx xxxxx xxxxxxx xxxx xxx XXX xxxx xxx xxx xxxxxxxx xxxxx Xxxxxxxx00 xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.
Xxx xxxxxxx xxxxxx xxxx xxxxxx xx xxx $Xxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxxxxxxx xxx xxx xxxxxx xxxxxx xxxx xxxx xxx XXX xxxx xxxxx Xxxxxxxx00 xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

## XXXXXXXXXX

### $XxxxxxxxxxXxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xx Xxxxxxxxxx xxxxxxx.
Xxxx xxxxxx xxxxxxx xxxxxxx xxx x XXX xxxx xxxx xxxxxxx xx xxx xxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxXxxx
Xxxxxxxxx xx xxx xxxx.
Xxxx xxxxxx xxxx xxxxxxx xxxx Xxxxxxxxxx xxxxxxxx xxxxxx xxxx xxxx.

```yaml
Type: DateTimeOffset]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xx
Xxxxxxxxx xxx xxxxxx XX xx xxx XXX xxxx xxxxxx xxx xxxx xxxxxx xx xxx.

```yaml
Type: Guid
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: ReportId

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxx
Xxxxxxxxx xxxx xxxx xxxxxx xxxx xxx xxxxxx XXX xxxxxx xxx xxx xxxxxxxxx xxxx xxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXx
Xxxxxxxxx xxx xxxxxx XX xx xxx XXX xxxx xxx xxxxx xxxx xxxxxx xxxx xxxxxxx.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxxxxXxxxxXxxx
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx xxxx xxxxxxxx xxx XXX xxxx xxx xxxxx xxxx xxxxxx xxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxx
Xxxxxxxxx x xxxxx xxxx.
Xxxx xxxxxx xxxx xxxxxxx xxxx Xxxxxxxxxx xxxxxxxx xxxxx xxxx xxxx.

```yaml
Type: DateTimeOffset]
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Xxx$XxxxxXxXxxxxxxxxxXxxXxxx](19472f94-5827-4878-a17a-d7bb10932861)

[Xxxxxx$XxxxxXxXxxxxxxxxxXxxXxxxXxxxxxXxxxxxx](0bfb6a70-3a4a-4e58-a0b9-e41eb52a90ef)


