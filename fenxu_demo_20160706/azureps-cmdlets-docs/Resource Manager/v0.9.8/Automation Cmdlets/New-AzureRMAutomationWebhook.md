---
external help file: RMAzure_Automation.xml
online version: 048bf33a-0bc1-4433-92e0-bd906f6edb8d
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXXXxxxxxxxxxXxxxxxx
## XXXXXXXX
Xxxxxxx x xxxxxxx xxx xx Xxxxxxxxxx xxxxxxx.

## XXXXXX

```
New-AzureRMAutomationWebhook [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-Name] <String>
 [-RunbookName] <String> [-IsEnabled] <Boolean> [-ExpiryTime] <DateTimeOffset> [-Force]
 [-Parameters <IDictionary>] [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxxxxx$$ xxxxxx xxxxxxx x xxxxxxx xxx xx xxxxx$0 Xxxxxxxxxx xxxxxxx.

Xx xxxx xx xxxx xxx xxxxxxx XXX xxxx xxxx xxxxxx xxxxxxx$ xxxxxxx xx xxxxxx xx xxxxxxxxx xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxxx
```
PS C:\>$Webhook = New-AzureRmAutomationWebhook -Name "Webhook06" -IsEnabled $True -ExpiryTime "10/2/2016" -RunbookName "ContosoRunbook" -ResourceGroup "ResourceGroup01" -AutomationAccountName "AutomationAccount01" -Force
```

Xxxx xxxxxxx xxxxxxx x xxxxxxx xxxxx Xxxxxxx00 xxx xxx xxxxxxx xxxxx XxxxxxxXxxxxxx xx xxx Xxxxxxxxxx xxxxxxx xxxxx XxxxxxxxxxXxxxxxx00.
Xxx xxxxxxx xxxxxx xxx xxxxxxx xx xxx $Xxxxxxx xxxxxxxx.
Xxx xxxxxxx xx xxxxxxx.
Xxx xxxxxxx xxxxxxx xx xxx xxxxxxxxx xxxx.
Xxxx xxxxxxx xxxx xxx xxxxxxx xxx xxxxxx xxx xxxxxxx xxxxxxxxxx.
Xxxx xxxxxxx xxxxxxxxx xxx $Xxxxx$ xxxxxxxxx.
Xxxxxxxxx$ xx xxxx xxx xxxxxx xxx xxx xxxxxxxxxxxx.

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxxx xxxxxxxxxx
```
PS C:\>$Params = @{"StringParam"="Hello World";"IntegerParam"=32}
PS C:\> $Webhook = New-AzureRmAutomationWebhook -Name "Webhook11" -Parameters $Params -IsEnabled $True -ExpiryTime "10/2/2016" -RunbookName "ContosoRunbook" -ResourceGroup "ResourceGroup01" -AutomationAccountName "AutomationAccount01" -Force
```

Xxx xxxxx xxxxxxx xxxxxxx x xxxxxxxxxx xx xxxxxxxxxx$ xxx xxxxxx xxxx xx xxx $Xxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx x xxxxxxx xxxxx Xxxxxxx00 xxx xxx xxxxxxx xxxxx XxxxxxxXxxxxxx xx xxx Xxxxxxxxxx xxxxxxx xxxxx XxxxxxxxxxXxxxxxx00.
Xxx xxxxxxx xxxxxxx xxx xxxxxxxxxx xx $Xxxxxx xx xxx xxxxxxx.

## XXXXXXXXXX

### $XxxxxxxxxxXxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xx Xxxxxxxxxx xxxxxxx xx xxxxx xxxx xxxxxx xxxxxxx x xxxxxxx.

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

### $XxxxxxXxxx
Xxxxxxxxx xxx xxxxxx xxxx xxx xxx xxxxxxx xx x $$XxxxXxxxXxxxxx$$ xxxxxx.
Xxx xxx xxxxxxx x xxxxxx xx x $$XxxxXxxx$$ xxxx xxx xx xxxxxxxxx xx x xxxxx $$XxxxXxxxXxxxxx$$.

```yaml
Type: DateTimeOffset
Parameter Sets: (All)
Aliases: 

Required: True
Position: 6
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxx
xx$xxxxx

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

### $XxXxxxxxx
Xxxxxxxxx xxxxxxx xxx xxxxxxx xx xxxxxxx.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: True
Position: 5
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx x xxxx xxx xxx xxxxxxx.

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

### $Xxxxxxxxxx
Xxxxxxxxx x xxxxxxxxxx xx xxx$xxxxx xxxxx.
Xxx xxxx xxx xxx xxxxxxx xxxxxxxxx xxxxx.
Xxx xxxxxx xxx xxx xxxxxxx xxxxxxxxx xxxxxx.
Xxxx xxx xxxxxxx xxxxxx xx xxxxxxxx xx x xxxxxxx$ xxxxx xxxxxxxxxx xxx xxxxxx xx xxx xxxxxxx.

```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxXxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxxxxx x xxxxxxx.

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

### $XxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxx xx xxxxxxxxx xx xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxx
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

### $XxxxXx
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

[Xxx$XxxxxXxXxxxxxxxxxXxxxxxx](048bf33a-0bc1-4433-92e0-bd906f6edb8d)

[Xxxxxx$XxxxxXxXxxxxxxxxxXxxxxxx](8dadbd54-8df1-4b9e-b853-97893e3ad73a)

[Xxx$XxxxxXxXxxxxxxxxxXxxxxxx](b2f5cd9e-5886-4ccc-89ea-9e66e5c67818)


