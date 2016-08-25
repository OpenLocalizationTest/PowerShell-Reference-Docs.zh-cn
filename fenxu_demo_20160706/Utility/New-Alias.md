---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293991
schema: 2.0.0
---

# New-Alias
## XXXXXXXX
Xxxxxxx x xxx xxxxx.

## XXXXXX

```
New-Alias [-Name] <String> [-Value] <String> [-Description <String>] [-Option <ScopedItemOptions>] [-PassThru]
 [-Scope <String>] [-Force] [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf]
 [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxx xxxxxx xxxxxxx x xxx xxxxx xx xxx xxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxxxxxx xxxxxxx xx xxxxx Xxx$Xxxxx xxx xxx xxxxx xxxxx xxx xxxx xxx xxxxxxx xx xxxxx Xxxxxxx XxxxxXxxxx.
Xxx xxx xxx xxx Xxxxxx$Xxxxx xxxxxx xx xxxx xxxx xxxxx xxxxxxxxxxx xx x xxxx.
Xxx xxx xxxxx xxx Xxxxxx$Xxxxx xx xxxxxxxx xxxx xxxxx xxxxx xxxxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>new-alias list get-childitem
```

Xxxx xxxxxxx xxxxxxx xx xxxxx xxxxx $xxxx$ xx xxxxxxxxx xxx Xxx$XxxxxXxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>new-alias -name w -value get-wmiobject -description "quick wmi alias" -option ReadOnly
PS C:\>get-alias -name w | format-list *
```

Xxxx xxxxxxx xxxxxxx xx xxxxx xxxxx $x$ xx xxxxxxxxx xxx Xxx$XXXXxxxxx xxxxxx.
Xx xxxxxxx x xxxxxxxxxxx$ $xxxxx xxx xxxxx$$ xxx xxx xxxxx xxx xxxxx xx xxxx xxxx.
Xxx xxxx xxxx xx xxx xxxxxxx xxxx Xxx$Xxxxx xx xxx xxx xxx xxxxx xxx xxxxx xx xx Xxxxxx$Xxxx xx xxxxxxx xxx xx xxx xxxxxxxxxxx xxxxx xx.

## XXXXXXXXXX

### -Description
Xxxxxxxxx x xxxxxxxxxxx xx xxx xxxxx.
Xxx xxx xxxx xxx xxxxxx.
Xx xxx xxxxxxxxxxx xxxxxxxx xxxxxx$ xxxxxxx xx xx xxxxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Xx xxx$ xxx xxxx xxx$xxxxx xx xxx xxxxx xxxxx xxxxxxx xxxxxx.

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

### -InformationAction
$$Xxxx$$

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa
Accepted values: SilentlyContinue, Stop, Continue, Inquire, Ignore, Suspend

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
$$Xxxx$$

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx xxx xxx xxxxx.
Xxx xxx xxx xxx xxxxxxxxxxxx xxxxxxxxxx xx xx xxxxx$ xxx xxx xxxxx xxxxxxxxx xxxxxx xx x xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Option
Xxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx xxx xxxxx.

Xxxxx xxxxxx xxx$

$$ Xxxx$ Xxxx xx xxxxxxx. $$Xxxx$ xx xxx xxxxxxx.$ $$ XxxxXxxx$ Xxx xx xxxxxxx. Xxxxxx xx xxx xxxxxxx$ xxxxxx xx xxxxx xxx Xxxxx xxxxxxxxx.
$$ Xxxxxxxx$ Xxxxxx xx xxxxxxx xx xxxxxxx.
$$ Xxxxxxx$ Xxx xxxxx xx xxxxxxxxx xxxx xx xxx xxxxxxx xxxxx.
$$ XxxXxxxx$ Xxx xxxxx xx xxxxxx xx xxx xxx xxxxxx xxxx xxx xxxxxxx.

Xx xxx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxxx xx xxx xxxxxxx$ xxxx $xxx$xxxxx $ xxxxxx$xxxxx $xxxxxxxx xxxx$ xxxxxxx $xxxxxxxx$.

```yaml
Type: ScopedItemOptions
Parameter Sets: (All)
Aliases: 
Accepted values: None, ReadOnly, Constant, Private, AllScope, Unspecified

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Xxxxxxx xx xxxxxx xxxxxxxxxxxx xxx xxx xxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

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

### -Scope
Xxxxxxxxx xxx xxxxx xx xxx xxx xxxxx.
Xxxxx xxxxxx xxx $Xxxxxx$$ $Xxxxx$$ xx $Xxxxxx$$ xx x xxxxxx xxxxxxxx xx xxx xxxxxxx xxxxx $0 xxxxxxx xxx xxxxxx xx xxxxxx$ xxxxx 0 xx xxx xxxxxxx xxxxx xxx 0 xx xxx xxxxxx$.
$Xxxxx$ xx xxx xxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Value
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xx xxxxxxx xxxxxxx xxxx xx xxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Confirm
Xxxxxxx xxx xxx xxxxxxxxxxxx xxxxxx xxxxxxx xxx xxxxxx.Xxxxxxx xxx xxx xxxxxxxxxxxx xxxxxx xxxxxxx xxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Xxxxx xxxx xxxxx xxxxxx xx xxx xxxxxx xxxx.
Xxx xxxxxx xx xxx xxx.Xxxxx xxxx xxxxx xxxxxx xx xxx xxxxxx xxxx.
Xxx xxxxxx xx xxx xxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### None
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### None or System.Management.Automation.AliasInfo
Xxxx xxx xxx xxx Xxxxxxxx xxxxxxxxx$ Xxx$Xxxxx xxxxxxxxx x Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XxxxxXxxx xxxxxx xxxxxxxxxxxx xxx xxx xxxxx.
Xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xx xxxxxx x xxx xxxxx$ xxx Xxx$Xxxxx xx Xxx$Xxxxx.
Xx xxxxxx xx xxxxx$ xxx Xxx$Xxxxx.
Xx xxxxxx xx xxxxx$ xxx Xxxxxx$Xxxx.

## XXXXXXX XXXXX

[Export-Alias]()

[Get-Alias]()

[Import-Alias]()

[Set-Alias]()

