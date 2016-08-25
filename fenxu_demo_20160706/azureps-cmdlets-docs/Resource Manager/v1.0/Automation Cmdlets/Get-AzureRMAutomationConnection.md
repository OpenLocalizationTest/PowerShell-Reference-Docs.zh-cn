---
external help file: RMAzure_Automation.xml
online version: 7fed73b4-73cf-4642-8e10-167ea6158372
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureRMAutomationConnection
## XXXXXXXX
Xxxx xx Xxxxxxxxxx xxxxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureRMAutomationConnection [-ResourceGroupName] <String> [-AutomationAccountName] <String>
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureRMAutomationConnection [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-Name] <String>
```

### UNNAMED_PARAMETER_SET_3
```
Get-AzureRMAutomationConnection [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-ConnectionTypeName] <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxxxxxxxx$$ xxxxxx xxxx xxx xx xxxx xxxxx$0 Xxxxxxxxxx xxxxxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxxxxxxx xxx xxxxxxxxxxx.
Xxxxxxx xxx xxxx xx x xxxxxxxxxx xx xxx x xxxxxxxx xxxxxxxxxx.
Xxxxxxx xxx xxxxxxxxxx xxxx xxxx xx xxx xxx xxxxxxxxxxx xx x xxxxxxxx xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxxxxxxxxx
```
PS C:\>Get-AzureRmAutomationConnection -ResourceGroupName "ResourceGroup01" -AutomationAccountName "Contoso17"
```

Xxxx xxxxxxx xxxx xxxxxxxx xxx xxx xxxxxxxxxxx xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

### Xxxxxxx 0$ Xxx xxx xxxxxxxxxxx xx x xxxx
```
PS C:\>Get-AzureRmAutomationConnection -ResourceGroupName "ResourceGroup01" -AutomationAccountName "Contoso17" -ConnectionTypeName "SqlServer"
```

Xxxx xxxxxxx xxxx xxxxxxxx xxx xxxxxxxxxxx xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.
Xxxx xxxxxxx xxxx xxxxxxxxxxx xx xxx xxxx XxxXxxxxx.

### Xxxxxxx 0$ Xxx x xxxxxxxxxx
```
PS C:\>Get-AzureRmAutomationConnection -ResourceGroupName "ResourceGroup01" -AutomationAccountName "Contoso17" -Name "ContosoConnection"
```

Xxxx xxxxxxx xxxx xxxxxxxx xxx xxx xxxxxxxxxx xxxxx XxxxxxxXxxxxxxxxx.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xxx xxxxx xxxx xxxxxx xxxx xxxxxxxxxxx.

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

### -ConnectionTypeName
Xxxxxxxxx xxx xxxx xx x xxxxxxxxxx xxxx xxx xxxxx xxxx xxxxxx xxxxxxxxx xxxxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx xxx xxxx xx x xxxxxxxxxx xxxx xxxx xxxxxx xxxxxxxxx.

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
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxx xxxxxxxxxxx.

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

### Microsoft.Azure.Commands.Automation.Model.Connection

## XXXXX

## XXXXXXX XXXXX

[New-AzureRmAutomationConnection](7fed73b4-73cf-4642-8e10-167ea6158372)

[Remove-AzureRmAutomationConnection](76dc3b3d-2dd3-49ad-a28c-afbfc754e020)


