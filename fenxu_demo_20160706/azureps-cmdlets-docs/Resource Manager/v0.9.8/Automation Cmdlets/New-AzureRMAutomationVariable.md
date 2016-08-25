---
external help file: RMAzure_Automation.xml
online version: a6dc9902-ad99-47f9-8212-d3d96146b180
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# New-AzureRMAutomationVariable
## XXXXXXXX
Xxxxxxx xx Xxxxxxxxxx xxxxxxxx.

## XXXXXX

```
New-AzureRMAutomationVariable [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Name] <String>
 [-Description <String>] [-Value <Object>] -Encrypted <Boolean>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxxxxxx$$ xxxxxx xxxxxxx x xxxxxxxx xx xxxxx$0 Xxxxxxxxxx.
Xx xxxxxxx xxx xxxxxxxx$ xxxxxxx xxx $Xxxxxxxxx$ xxxxxxxxx.
Xxx xxxxxx xxxxxx xxx xxxxxxxxx xxxxx xx x xxxxxxxx xxxxx xxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxxxx xxxx x xxxxxx xxxxx
```
PS C:\>New-AzureRmAutomationVariable -AutomationAccountName "Contoso17" -Name "StringVariable22" -Encrypted $False -Value "My String" -ResourceGroupName "ResourceGroup01"
```

Xxxx xxxxxxx xxxxxxx x xxxxxxxx xxxxx XxxxxxXxxxxxxx00 xxxx x xxxxxx xxxxx xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.

### Xxxxxxx 0$ Xxxxxx x xxxxxxxx xxxx x xxxxxxx xxxxx
```
PS C:\>$VirtualMachine = Get-AzureVM -ServiceName "VirtualMachine" -Name "VirtualMachine03"
PS C:\> New-AzureRmAutomationVariable -AutomationAccountName "Contoso17" -Name "ComplexVariable01" -Encrypted $False -Value $VirtualMachine -ResourceGroupName "ResourceGroup01"
```

Xxx xxxxx xxxxxxx xxxx x xxxxxxx xxxxxxx xx xxxxx xxx Xxx$XxxxxXX xxxxxx.
Xxx xxxxxxx xxxxxx xx xx xxx $XxxxxxxXxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx x xxxxxxxx xxxxx XxxxxxxXxxxxxxx00 xx xxx Xxxxxxxxxx xxxxxxx xxxxx Xxxxxxx00.
Xxxx xxxxxxx xxxx x xxxxxxx xxxxxx xxx xxx xxxxx$ xx xxxx xxxx$ xxx xxxxxxx xxxxxxx xx $XxxxxxxXxxxxxx.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xx xxxxx xx xxxxx xxx xxxxxxxx.

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
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Encrypted
Xxxxxxxxx xxxxxxx xxxx xxxxxx xxxxxxxx xxx xxxxx xx xxx xxxxxxxx xxx xxxxxxx.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx x xxxx xxx xxx xxxxxxxx.

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
Xxxxxxxxx xxx xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxxxxx x xxxxxxxx.

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
Parameter Sets: (All)
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

[Get-AzureRmAutomationVariable](a6dc9902-ad99-47f9-8212-d3d96146b180)

[Remove-AzureRmAutomationVariable](c154838a-0b3d-4347-96a5-31ac572b329c)

[Set-AzureRmAutomationVariable](3bc5445e-7884-4dab-b00d-3bdfed9f05c5)


