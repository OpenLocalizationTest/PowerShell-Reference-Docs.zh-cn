---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294011
schema: 2.0.0
---

# Set-Alias
## XXXXXXXX
Xxxxxxx xx xxxxxxx xx xxxxx $xxxxxxxxx xxxx$ xxx x xxxxxx xx xxxxx xxxxxxx xxxxxxx xx xxx xxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx.

## XXXXXX

```
Set-Alias [-Name] <String> [-Value] <String> [-Description <String>] [-Option <ScopedItemOptions>] [-PassThru]
 [-Scope <String>] [-Force] [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf]
 [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxx xxxxxx xxxxxxx xx xxxxxxx xx xxxxx $xxxxxxxxx xxxx$ xxx x xxxxxx xx xxx x xxxxxxx xxxxxxx$ xxxx xx x xxxxxxxx$ x xxxxxx$ x xxxx$ xx xxxxx xxxxxxxxxx.
Xxx xxx xxxx xxx Xxx$Xxxxx xx xxxxxxxx x xxxxxxx xxxxx xx x xxx xxxxxxx$ xx xx xxxxxx xxx xx xxx xxxxxxxxxx xx xx xxxxx$ xxxx xx xxx xxxxxxxxxxx.
Xxxxxx xxx xxx xxx xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxx$ xxx xxxxxxx xx xx xxxxx xxx xxxx xxxx xxx xxxx xxx xxxxxxx xx xxxxx Xxxxxxx XxxxxXxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-alias -name list -value get-childitem
```

Xxxx xxxxxxx xxxxxxx xxx xxxxx $xxxx$ xxx xxx Xxx$XxxxxXxxx xxxxxx.
Xxxxx xxx xxxxxx xxx xxxxx$ xxx xxx xxx $xxxx$ xx xxxxx xx $Xxx$XxxxxXxxx$ xx xxx xxxxxxx xxxx xxx xx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-alias list get-location
```

Xxxx xxxxxxx xxxxxxxxxx xxx xxxxx $xxxx$ xxxx xxx Xxx$Xxxxxxxx xxxxxx.
Xx $xxxx$ xx xx xxxxx xxx xxxxxxx xxxxxx$ xxxx xxxxxxx xxxxxxx xxx xxxxxxxxxxx xx xxxx xx xxx xx xxx xxxxx xxxx xxx Xxx$Xxxxxxxx.

Xxxx xxxxxxx xxxx xxx xxxx xxxxxx xx xxx xxxxxxx xx xxx xxxxxxxx xxxxxxx$ xxx xx xxxxx xxx xxxxxxxx xxxxxxxxx xxxxx$ $Xxxx xxx $Xxxxx.
Xxxx xxx xxxx xxxxxxxxx xxxxx$ xxx xxxxxx xx xxxxx xxxxxxxxxx xxxx xxxxxx xx xxx xxxxxxxxx xxxxx xx xxx xxxxxxx.
Xx xxxx xxxx$ xxx xxxxx xx $Xxxx $$xxxx$$ xxxx xx xxx xxxxx xxxxxxxxx xxx xxx xxxxx xx $Xxxxx $$xxx$xxxxxxxx$$ xxxx xx xxx xxxxxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-alias scrub remove-item -option readonly -passthru | format-list
```

Xxxx xxxxxxx xxxxxxxxxx xxx xxxxx $xxxxx$ xxxx xxx Xxxxxx$Xxxx xxxxxx.
Xx xxxx xxx $XxxxXxxx$ xxxxxx xx xxxxxxx xxx xxxxx xxxx xxxxx xxxxxxx xx xxxxxxxx xx xxxxxxx xxxxxx.

Xxx XxxxXxxx xxxxxxxxx xxxxxxx Xxxxxxx XxxxxXxxxx xx xxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxx xxxxx xxxxxxx xxx xxxxxxxx xx xxx Xxxxxx$Xxxx xxxxxx.
Xx xxx XxxxXxxx xxxxxxxxx xxxx xxxxxxx$ xxxxx xxxxx xx xx xxxxxx xxxx xxxx xxxxxx xx xxxxxxx $xx x xxxx xx xxxxxxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Set-Alias np c:\windows\notepad.exe
```

Xxxx xxxxxxx xxxxxxxxxx xxx xxxxx$ $xx$$ xxxx xxx xxxxxxxxxx xxxx xxx Xxxxxxx.
Xxxxx xxx xxxxxxx xxxxxxxxx$ xx xxxx Xxxxxxx xxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xxxx$ xxxx xxxx $xx$.

Xxxx xxxxxxx xxxxxxxxxxxx xxxx xxx xxx xxxxxx xxxxxxx xxx xxxxxxxxxx xxxxx xxx xxxxxxxx xxxxx xxxx xxxxxxx.

Xx xxxx xxx xxxxxxx xxxx xxxxxxx$ xxx xxx xxx xxx $Xxxxxx$ xxxxxxxxxxx xxxxxxxx $$$xxx$xxxxxx$$ xx xxxxxxxxx xxx X$Xxxxxxx xxxxxxxxx.
Xxx xxxxxxx xxxxxxx xx xxx xxxxxxx xx $xxx$xxxxx xx $$xxx$xxxxxx$$xxxxxxx.xxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>function CD32 {set-location c:\windows\system32}
PS C:\>set-alias go cd32
```

Xxxxx xxxxxxxx xxxx xxx xx xxxxxx xx xxxxx xx x xxxxxxx xxxx xxxxxxxxxx$ xx xxxx xx x xxxxxxxx xx xxxx xxxxxxxx.

Xxx xxx xxxxxx xx xxxxx xxx x xxxxxx$ xxx xxx xxxxxx xxxxxx xx xxxxx xxx x xxxxxxx xxxx xxxxxxxx xx x xxxxxx xxx xxx xxxxxxxxxx.
Xxxxxxx$ xx xxx xxxxx xxx xxxxxxx xx x xxxxxxxx xx x xxxxxx$ xxxx xxx xxx xxxxxx x xxxxxx xxxxxxxx xx xxxxxx xxxx xxx xxx xxx xxxxxx xxx xx xxxx xxxxxxx xxx xxx xxxxxxxx xx xxxxxx.

Xx xxxx xxxxxxx$ xxx xxxx xxxxx xx xxxxxx xx xxxxx xxx xxx xxxxxxx $xxx$xxxxxxxx x$$xxxxxxx$xxxxxx00$$ xxxxx $xxx$xxxxxxxx$ xx x xxxxxx xxx $X$$Xxxxxxx$Xxxxxx00$ xx xxx xxxxx xx xxx Xxxx xxxxxxxxx.

Xx xx xxxx$ xxx xxxxx xxxxxxx xxxxxxx x xxxxxxxx xxxxxx $XX00$ xxxx xxxxxxxx xxx Xxx$Xxxxxxxx xxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx xxx xxxxx $xx$ xxx xxx XX00 xxxxxxxx.
Xxxx$ xx xxx xxx Xxx$Xxxxxxxx xxxxxxx$ xxx xxxx xxx xxxx xxxxxx $XX00$ xx $xx$.

## XXXXXXXXXX

### -Description
Xxxxxxxxx x xxxxxxxxxxx xx xxx xxxxx.
Xxx xxx xxxx xxx xxxxxx.
Xx xxx xxxxxxxxxxx xxxxxxxx xxxxxx$ xxxxxxx xx xxxxxxxxx xxxxx.

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
Xxxxxx xxx xxxxxx xx xxx x xxxx$xxxx xxxxx.
Xxx xxx Xxxxxx xxxxxxxxx xx xxxxxx x xxxx$xxxx xxxxx.
Xxx Xxxxx xxxxxxxxx xxxxxx xxx x xxxxxxxx xxxxx.

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
Xxxxxxx xx xxxxxx xxxxxxxxxxxx xxx xxxxx.
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
Xxxxxxxxx xxx xxxxx xx xxxxx xxxx xxxxx xx xxxxx.
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
Xxxx xxx xxx xxx XxxxXxxx xxxxxxxxx$ Xxx$Xxxxx xxxxxxxxx x Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XxxxxXxxx xxxxxx xxxxxxxxxxxx xxx xxxxx.
Xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xx xxxxx xx xx xxxxxxxxx xxxx xx xxxxxxxx xxx x xxxxxx xx xxxxxxx xxxxxxx.
Xx xxx xxx xxxxxx$ xxx xxx xxx xxx xxxx xxxx xx xxx xxxxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx.

Xx xxxxxx x xxx xxxxx$ xxx Xxx$Xxxxx xx Xxx$Xxxxx.
Xx xxxxxx xx xxxxx$ xxx Xxxxxx$Xxxx.

X xxxxxx xxx xxxx xxxxxxxx xxxxxxx$ xxx xx xxxxx xxx xxxx xx xxxxxxxxxx xxxx xxx xxxxxx xx x xxxx.
Xx xxx xxx xxx$xxxxx xx xxxxxxxxx xxx xxxxx xxxx x xxxxxxxxx xxxxxx$ xx xx xx xxxxxx xxxxxxxxxx xxxx xxx xxxxxxxx xxxxxx.

Xxx xxx xxxxxx xx xxxxx xxx x xxxxxx$ xxx xxx xxxxxx xxxxxx xx xxxxx xxx x xxxxxxx xxxx xxxxxxxxxx xxx xxxxxx.
Xxx xxxxxxx$ xxx xxx xxxxxx xx xxxxx xxx Xxx$Xxxxxxxx$ xxx xxx xxxxxx xxxxxx xx xxxxx xxx $Xxx$Xxxxxxxx X$$Xxxxxxx$Xxxxxx00$.
Xx xxxxxx xx xxxxx xxx x xxxxxxx$ xxxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx$ xxx xxxx xxxxxx xx xxxxx xx xxx xxxxxxxx.

Xx xxxx xxx xxxxxxx xxxx x xxxxxxx xxx xxx xxxx xx x xxxxxxxxx xxxxxxx$ xxx xxx xxx$xxxxx xxxxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxxxxxxx xx xxx xxxxx xx xxxxxxx.
Xx xxxxxx x xxxxxxx xx xxx xxxx xxxxxx xx xxx $xxxxxxx xxxxxxxx$ xxxx $xxx$xxxx $xxxx xxxx $xxxxx $xxxxxxx$.
Xx xxx xxx xxxxx xx xxx $xxxxxxx xxxxxxxx$ xxxx $$xxxxxxx$.

Xxx xxx xxxx xxxx xxxx xxxxxxx xx xxxxx Xxxxxx$Xxxxx xx xxxx xxx xxxxxxx xxxx xxx xxxxxxx xx x xxxx$ xxx xxxx xxx Xxxxxx$Xxxxx xx xxx xxxx xx xxx xxxxx xxxx xxx x xxx xxxxxxx.

Xxx xxx xxxx xxxxx xx Xxx$Xxxxx xx xxx xxxxx$xx xxxxx$ $xxx$.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx.

## XXXXXXX XXXXX

[Export-Alias]()

[Get-Alias]()

[Import-Alias]()

[New-Alias]()

