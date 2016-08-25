---
external help file: RMAzure_Automation.xml
online version: a6dc9902-ad99-47f9-8212-d3d96146b180
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Set-AzureRMAutomationVariable
## XXXXXXXX
Xxxxxxxx xx Xxxxxxxxxx xxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Set-AzureRMAutomationVariable [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Name] <String>
 -Encrypted <Boolean> -Value <Object>
```

### UNNAMED_PARAMETER_SET_2
```
Set-AzureRMAutomationVariable [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Name] <String>
 -Description <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxxxxxx$$ xxxxxx xxxxxxxx xxx xxxxx xx xxxxxxxxxxx xx x xxxxxxxx xx xxxxx$0 Xxxxxxxxxx.
Xx xxxxxxx xxx xxxxxxxx$ xxxxxxx xxx $Xxxxxxxxx$ xxxxxxxxx.
Xxx xxxxxx xxxxxx xxx xxxxxxxxx xxxxx xx x xxxxxxxx xxxxx xxxxxxxx.
Xxxxxxxxxx $Xxxxxxxxx$ xxx xx xxxxxxxx$ xxx$xxxxxxxxx$ xxxxxxxx xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxxx xx x xxxxxxxx
```
PS C:\>Set-AzureRmAutomationVariable -AutomationAccountName "Contoso17" -Name "StringVariable22" -ResourceGroupName "ResourceGroup01" -Value "New Value" -Encrypted $False
```

Xxxx xxxxxxx xxxx x xxx xxxxx xxx xxx xxxxxxxx xxxxx XxxxxxXxxxxxxx00 xx xxx xxxxx$0 Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xx xxxxx xxx xxxxxxxx xx xxxxxx.

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

### -Description
Xxxxxxxxx x xxxxxxxxxxx xxx xxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Encrypted
Xxxxxxxxx xxxxxxx xxxxxx xxxxxxxx xxx xxxxx xx xxx xxxxxxxx xxx xxxxxxx.

```yaml
Type: Boolean
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx xxxx xxxx xxxxxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxxxxxx x xxxxxxxx.

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

### -Value
Xxxxxxxxx x xxxxx xxx xxx xxxxxxxx.

```yaml
Type: Object
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

### Microsoft.Azure.Commands.Automation.Model.Variable

## XXXXX

## XXXXXXX XXXXX

[Get-AzureRmAutomationVariable](a6dc9902-ad99-47f9-8212-d3d96146b180)

[New-AzureRmAutomationVariable](4103a716-9567-4836-b522-d2484452a60e)

[Remove-AzureRmAutomationVariable](c154838a-0b3d-4347-96a5-31ac572b329c)


