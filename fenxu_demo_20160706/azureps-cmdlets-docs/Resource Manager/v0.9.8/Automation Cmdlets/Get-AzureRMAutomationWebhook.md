---
external help file: RMAzure_Automation.xml
online version: cca289e3-4c75-48af-9f25-f99b0c6965c4
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureRMAutomationWebhook
## XXXXXXXX
Xxxx xxxxxxxx xxxx Xxxxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureRMAutomationWebhook [-ResourceGroupName] <String> [-AutomationAccountName] <String>
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureRMAutomationWebhook [-ResourceGroupName] <String> [-AutomationAccountName] <String> -Name <String>
```

### UNNAMED_PARAMETER_SET_3
```
Get-AzureRMAutomationWebhook [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 -RunbookName <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxxxxx$$ xxxxxx xxxx xxxxxxxx.
Xx xxx xxxxxxxx xxxxxxxx$ xxxxxxx x xxxxxxx xxxx xx xxxxxxx xxx xxxx xx xx xxxxx$0 Xxxxxxxxxx xxxxxxx xx xxx xxx xxxxxxxx xxxxxxxxx xx xx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxxxxxx xxx x xxxxxxx
```
PS C:\>Get-AzureRmAutomationWebhook -RunbookName "Runbook03" -ResourceGroup "ResourceGroup01" -AutomationAccountName "AutomationAccount01"
```

Xxxx xxxxxxx xxxx xxx xxxxxxxx xxx x xxxxxxx xxxxx Xxxxxxx00 xx xxx Xxxxxxxxxx xxxxxxx xxxxx XxxxxxxxxxXxxxxxx00 xx xxx xxxxxxxx xxxxx xxxxx XxxxxxxxXxxxx00.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xx Xxxxxxxxxx xxxxxxx xx xxxxx xxxx xxxxxx xxxx x xxxxxxx.

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
Xxxxxxxxx xxx xxxx xx xxx xxxxxxx xxxx xxxx xxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: WebhookName

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxx xxxxxxxx.

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

### -RunbookName
Xxxxxxxxx xxx xxxx xx x xxxxxxx xxx xxxxx xxxx xxxxxx xxxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[New-AzureRmAutomationWebhook](cca289e3-4c75-48af-9f25-f99b0c6965c4)

[Remove-AzureRmAutomationWebhook](8dadbd54-8df1-4b9e-b853-97893e3ad73a)

[Set-AzureRmAutomationWebhook](b2f5cd9e-5886-4ccc-89ea-9e66e5c67818)


