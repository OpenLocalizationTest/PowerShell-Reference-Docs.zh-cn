---
external help file: RMAzure_Automation.xml
online version: 091cd841-4aaf-45de-a8f2-6f973fb9c91b
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Import-AzureRmAutomationDscNodeConfiguration
## XXXXXXXX
Xxxxxxx x XXX xxxxxxxx xx x XXX xxxx xxxxxxxxxxxxx xx Xxxxxxxxxx.

## XXXXXX

```
Import-AzureRmAutomationDscNodeConfiguration [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-Force] -ConfigurationName <String> -Path <String> [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxxxxx$XxxxxXxXxxxxxxxxxXxxXxxxxxxxxxxxx$$ xxxxxx xxxxxxx x Xxxxxxx Xxxxxx Xxxxxx $XXX$ xxxxxxxxxxxxx xxxxxxxx xxxx xxxxx$0 Xxxxxxxxxx xx x Xxxxxxx Xxxxx Xxxxxxxxxxxxx $XXX$ xxxx xxxxxxxxxxxxx.
Xxxxxxx xxx xxxx xx x .xxx xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x XXX xxxx xxxxxxxxxxxxx xxxx Xxxxxxxxxx
```
PS C:\>Import-AzureRmAutomationDscConfiguration -AutomationAccountName "Contoso17" -ResourceGroupName "ResourceGroup01" -ConfigurationName "ContosoConfiguration" -Path "C:\DSC\webserver.mof" -Force
```

Xxxx xxxxxxx xxxxxxx x XXX xxxx xxxxxxxxxxxxx xxxx xxx xxxx xxxxx xxxxxxxxx.xxx xxxx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00$ xxxxx xxx XXX xxxxxxxxxxxxx XxxxxxxXxxxxxxxxxxxx.
Xxx xxxxxxx xxxxxxxxx xxx $Xxxxx$ xxxxxxxxx.
Xx xxxxx xx xx xxxxxxxx XXX xxxx xxxxxxxxxxxxx xxxxx XxxxxxxXxxxxxxxxxxxx.xxxxxxxxx$ xxxx xxxxxxx xxxxxxxx xx.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xxxx xxxxx xxxx xxxxxx xxxxxxx x XXX xxxx xxxxxxxxxxxxx.

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
Xxxxxxxxx xxx xxxx xx x XXX xxxxxxxxxxxxx xx Xxxxxxxxxx xx xxx xx xxx xxxxxxxxx xxx xxxxxxxxx xxx xxx xxxx xxxxxxxxxxxxx xx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Force
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxxx xx xxxxxxxx XXX xxxx xxxxxxxxxxxxx xx Xxxxxxxxxx.

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

### -Path
Xxxxxxxxx xxx xxxx xx xxx XXX xxxxxxxxxxxxx xxxxxxxx xxxx xxxx xxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx x xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxxxxx x XXX xxxx xxxxxxxxxxxxx.

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

[Export-AzureRmAutomationDscConfiguration](091cd841-4aaf-45de-a8f2-6f973fb9c91b)

[Get-AzureRmAutomationDscConfiguration](cd411497-be17-46f7-8708-519f02312553)


