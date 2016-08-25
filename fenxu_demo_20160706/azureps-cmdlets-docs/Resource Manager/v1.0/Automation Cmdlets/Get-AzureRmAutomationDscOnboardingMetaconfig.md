---
external help file: RMAzure_Automation.xml
online version: a6f623a1-2e69-4ea2-828b-ab63d285a009
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureRmAutomationDscOnboardingMetaconfig
## XXXXXXXX
Xxxxxxx xxxx$xxxxxxxxxxxxx .xxx xxxxx.

## XXXXXX

```
Get-AzureRmAutomationDscOnboardingMetaconfig [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-ComputerName <String[]>] [-Force] [-OutputFolder <String>] [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxXxxxxxxxxxXxxxxxxxxx$$ xxxxxx xxxxxxx XXX Xxxxxxx Xxxxx Xxxxxxxxxxxxx $XXX$ xxxx$xxxxxxxxxxxxx Xxxxxxx Xxxxxx Xxxxxx $XXX$ xxxxx.
Xxxx xxxxxx xxxxxxx x .xxx xxxx xxx xxxx xxxxxxxx xxxx xxxx xxx xxxxxxx.
Xxx xxxxxx xxxxxxx x xxxxxx xxx xxx .xxx xxxxx.
Xxx xxx xxx xxx Xxx$XxxXxxxxXxxxxxxxxxxxxXxxxxxx xxxxxx xxx xxxx xxxxxx xx xxxxxxx xxxxx xxxxxxxxx xxxx xx xxxxx$0 Xxxxxxxxxx xxxxxxx xx XXX xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxxx xxxxxxx xx Xxxxxxxxxx XXX
```
PS C:\>Get-AzureRmAutomationDscOnboardingMetaconfig -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -ComputerName "Server01", "Server02" -OutputFolder "C:\Users\PattiFuller\Desktop" 
PS C:\> Set-DscLocalConfigurationManager -Path "C:\Users\PattiFuller\Desktop\DscMetaConfigs" -ComputerName "Server01", "Server02"
```

Xxx xxxxx xxxxxxx xxxxxxx XXX xxxx$xxxxxxxxxxxxx xxxxx xxx xxx xxxxxxx xxx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.
Xxx xxxxxxx xxxxx xxxxx xxxxx xx x xxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx $$Xxx$XxxXxxxxXxxxxxxxxxxxxXxxxxxx$$ xxxxxx xx xxxxx xxx xxxx$xxxxxxxxxxxxx xx xxx xxxxxxxxx xxxxxxxxx xx xxxxxxx xxxx xx XXX xxxxx.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xx Xxxxxxxxxx xxxxxxx.
Xxx xxx xxxxxxx xxx xxxxxxxxx xxxx xxx $XxxxxxxxXxxx$ xxxxxxxxx xxxxxxxxx xx xxx xxxxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

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

### -ComputerName
Xxxxxxxxx xx xxxxx xx xxxxx xx xxxxxxxxx xxx xxxxx xxxx xxxxxx xxxxxxxxx .xxx xxxxx.
Xx xxx xx xxx xxxxxxx xxxx xxxxxxxxx$ xxx xxxxxx xxxxxxxxx xx .xxx xxxx xxx xxx xxxxxxx xxxxxxxx $xxxxxxxxx$.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Force
Xxxxxx xxx xxxxxxx xx xxx xxxxxxx xxxxxxxxx xxx xxx xxxxxxxxxxxx$ xxx xx xxxxxxx xxxxxxxx .xxx xxxxx xxxx xxxx xxx xxxx xxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutputFolder
Xxxxxxxxx xxx xxxx xx x xxxxxx xxxxx xxxx xxxxxx xxxxxx .xxx xxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx.
Xxxx xxxxxx xxxxxxx .xxx xxxxx xx xxxxxxx xxxxxxxxx xx xxx xxxxxxxx xxxxx xxxx xxxx xxxxxxxxx xxxxxxxxx.

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

### -Confirm
xxxx$xxxxxxxxxxx

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
xxxx$xxxxxxxxxx

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX


