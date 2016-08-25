---
external help file: RMAzure_Automation.xml
online version: a6f623a1-2e69-4ea2-828b-ab63d285a009
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureRmAutomationDscNode
## XXXXXXXX
Xxxx XXX xxxxx xxxx Xxxxxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureRmAutomationDscNode [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Status]
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureRmAutomationDscNode [-ResourceGroupName] <String> [-AutomationAccountName] <String> -Id <Guid>
```

### UNNAMED_PARAMETER_SET_3
```
Get-AzureRmAutomationDscNode [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Status]
 -NodeConfigurationName <String>
```

### UNNAMED_PARAMETER_SET_4
```
Get-AzureRmAutomationDscNode [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Status]
 -Name <String>
```

### UNNAMED_PARAMETER_SET_5
```
Get-AzureRmAutomationDscNode [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 -ConfigurationName <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxXxxx$$ xxxxxx xxxx XXX Xxxxxxx Xxxxx Xxxxxxxxxxxxx $XXX$ xxxxx xxxx xxxxx$0 Xxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx XXX xxxxx
```
PS C:\>Get-AzureRmAutomationDscNode -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17"
```

Xxxx xxxxxxx xxxx xxxxxxxx xxx xxx XXX xxxxx xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

### Xxxxxxx 0$ Xxx xxx XXX xxxxx xxx x XXX xxxxxxxxxxxxx
```
PS C:\>Get-AzureRmAutomationDscNode -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -ConfigurationName "ContosoConfiguration"
```

Xxxx xxxxxxx xxxx xxxxxxxx xxx xxx XXX xxxxx xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00 xxxx xxx xxxxxx xx x XXX xxxx xxxxxxxxxxxxx xxxxx xxx xxxxxxxxx xx XXX xxxxxxxxxxxxx XxxxxxxXxxxxxxxxxxxx.

### Xxxxxxx 0$ Xxx x XXX xxxx xx XX
```
PS C:\>Get-AzureRmAutomationDscNode -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -Id c0a1718e-d8be-4fa3-91b6-82e1d3a36298
```

Xxxx xxxxxxx xxxx xxxxxxxx xx x XXX xxxx xxxx xxx xxxxxxxxx XX xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

### Xxxxxxx 0$ Xxx x XXX xxxx xx xxxx
```
PS C:\>Get-AzureRmAutomationDscNode -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -Name "Computer14"
```

Xxxx xxxxxxx xxxx xxxxxxxx xx x XXX xxxx xxxx xxx xxxx Xxxxxxxx00 xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

### Xxxxxxx 0$ Xxx xxx XXX xxxxx xxxxxx xx x XXX xxxx xxxxxxxxxxxxx
```
PS C:\>Get-AzureRmAutomationDscNode -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -NodeConfigurationName "ContosoConfiguration.webserver"
```

Xxxx xxxxxxx xxxx xxxxxxxx xx xxx XXX xxxxx xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00 xxxx xxx xxxxxx xx x XXX xxxx xxxxxxxxxxxxx xxxxx XxxxxxxXxxxxxxxxxxxx.xxxxxxxxx.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xxxx xxxxxxxx xxx XXX xxxxx xxxx xxxx xxxxxx xxxx.

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

### -ConfigurationName
Xxxxxxxxx xxx xxxx xx x XXX xxxxxxxxxxxxx.
Xxxx xxxxxx xxxx XXX xxxxx xxxx xxxxx xxx xxxx xxxxxxxxxxxxxx xxxxxxxxx xxxx xxx xxxxxxxxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_5
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Xxxxxxxxx xxx xxxxxx XX xx xxx XXX xxxx xxxx xxxx xxxxxx xxxx.

```yaml
Type: Guid
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: NodeId

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx xxx xxxx xx x XXX xxxx xxxx xxxx xxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_4
Aliases: NodeName

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -NodeConfigurationName
Xxxxxxxxx xxx xxxx xx x xxxx xxxxxxxxxxxxx xxxx xxxx xxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx xx xxxxx xxxx xxxxxx xxxx XXX xxxxx.

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

### -Status
Xxxxxxxxx xxx xxxxxx xx xxx XXX xxxxx xxxx xxxx xxxxxx xxxx.
Xxxxx xxxxxx xxx$ 

$$ Xxxxxxxxx $$ XxxXxxxxxxxx $$ Xxxxxx $$ Xxxxxxx $$ Xxxxxxxx $$ Xxxxxxxxxxxx

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4
Aliases: 
Accepted values: Compliant, NotCompliant, Failed, Pending, Received, Unresponsive

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Register-AzureRmAutomationDscNode](a6f623a1-2e69-4ea2-828b-ab63d285a009)

[Set-AzureRmAutomationDscNode](68da8fba-38df-4255-91e8-513635163d57)

[Unregister-AzureRmAutomationDscNode](159d4e1d-b8db-4544-9807-c09e63fbd5dd)


