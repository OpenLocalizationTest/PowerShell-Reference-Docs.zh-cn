---
external help file: RMAzure_Automation.xml
online version: 4103a716-9567-4836-b522-d2484452a60e
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureRMAutomationVariable
## XXXXXXXX
Xxxx xx Xxxxxxxxxx xxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureRMAutomationVariable [-ResourceGroupName] <String> [-AutomationAccountName] <String>
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureRMAutomationVariable [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Name] <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxxxxxx$$ xxxxxx xxxx xxx xx xxxx xxxxx$0 Xxxxxxxxxx xxxxxxxxx.
Xx xxx x xxxxxxxx xxxxxxxx$ xxxxxxx xxx xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx x xxxxxxxx
```
PS C:\>$Variable = Get-AzureRmAutomationVariable -AutomationAccountName "Contoso17" -Name "Variable06" -ResourceGroupName "ResourceGroup01"
PS C:\> $Value = $Variable.value
```

Xxx xxxxx xxxxxxx xxxx xx Xxxxxxxxxx xxxxxxxx xxxxx Xxxxxxxx00 xx xxx xxxxxxx xxxxx Xxxxxxx00.
Xxx xxxxxxx xxxxxx xxxx xxxxxx xx xxx $Xxxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxxxxxxx xxx xxxxxxxx xx xxxxx xx xxx $$xxxxx$$ xxxxxxxx xx $Xxxxxxxx.
Xxx xxxxxxx xxxxxx xxx xxxxx xx xxx $xxxxx xxxxxxxx.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xxxx xxxxxxxx xxx xxxxxxxxx xxxx xxxx xxxxxx xxxx.

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

### -Name
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxx xxxx xxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxx xxxxxxxxx.

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

## XXXXXX

## XXXXXXX

### Microsoft.Azure.Commands.Automation.Model.Variable

## XXXXX

## XXXXXXX XXXXX

[New-AzureRmAutomationVariable](4103a716-9567-4836-b522-d2484452a60e)

[Remove-AzureRmAutomationVariable](c154838a-0b3d-4347-96a5-31ac572b329c)

[Set-AzureRmAutomationVariable](3bc5445e-7884-4dab-b00d-3bdfed9f05c5)


