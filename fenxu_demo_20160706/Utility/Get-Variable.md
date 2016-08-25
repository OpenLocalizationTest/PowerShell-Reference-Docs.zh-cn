---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293979
schema: 2.0.0
---

# Get-Variable
## XXXXXXXX
Xxxx xxx xxxxxxxxx xx xxx xxxxxxx xxxxxxx.

## XXXXXX

```
Get-Variable [[-Name] <String[]>] [-ValueOnly] [-Include <String[]>] [-Exclude <String[]>] [-Scope <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxxxx xxxxxx xxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxx xxxxxxxx xxxx xxx xxxxxx xx xxx xxxxxxxxx xx xxxxxxxxxx xxx XxxxxXxxx xxxxxxxxx$ xxx xxx xxx xxxxxx xxx xxxxxxxxx xxxxxxxx xx xxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Variable m*
```

Xxxx xxxxxxx xxxx xxxxxxxxx xxxx xxxxx xxxx xxxxx xxxx xxx xxxxxx $x$.
Xxx xxxxxxx xxxx xxxx xxx xxxxx xx xxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Variable m* -Valueonly
```

Xxxx xxxxxxx xxxx xxxx xxx xxxxxx xx xxx xxxxxxxxx xxxx xxxx xxxxx xxxx xxxxx xxxx $x$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Variable -Include M*,P*
```

Xxxx xxxxxxx xxxx xxxxxxxxxxx xxxxx xxx xxxxxxxxx xxxx xxxxx xxxx xxxxxx xxx xxxxxx $X$ xx xxx xxxxxx $X$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Variable -Scope 0
PS C:\>Compare-Object (Get-Variable -Scope 0) (Get-Variable -Scope 1)
```

Xxx xxxxx xxxxxxx xxxx xxxx xxx xxxxxxxxx xxxx xxx xxxxxxx xx xxx xxxxx xxxxx.
Xx xx xxxxxxxxxx xx $Xxx$Xxxxxxxx $Xxxxx Xxxxx$ xxx xxx xx xxxxxxxxxxx xx $xx $x 0$.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxxx$Xxxxxx xxxxxx xx xxxx xxx xxxxxxxxx xxxx xxx xxxxxxx xx xxx xxxxxx xxxxx $Xxxxx 0$ xxx xxx xxxxxxx xxxx xx xxx xxxxx xxxxx $Xxxxx 0$.

## XXXXXXXXXX

### -Exclude
Xxxxx xxx xxxxxxxxx xxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Include
Xxxxxxxxx xxxx xxx xxxxx xxxx xxxxx xxx xxxxxx xxxx xxx$ xxxxxxxxx xxx xxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

```yaml
Type: String[]
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
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.
Xxx xxx xxxx xxxx x xxxxxxxx xxxx xx Xxx$Xxxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Scope
Xxxx xxxx xxx xxxxxxxxx xx xxx xxxxxxxxx xxxxx.
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

### -ValueOnly
Xxxx xxxx xxx xxxxx xx xxx xxxxxxxx.

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

## XXXXXX

### System.String
Xxx xxx xxxx x xxxxxx xxxx xxxxxxxx xxx xxxxxxxx xxxx xx Xxx$Xxxxxxxx.

## XXXXXXX

### System.Management.Automation.PSVariable
Xxx$Xxxxxxxx xxxxxxx x Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx xxxxxxxx xxxxxx xxx xxxx xxxxxxxx xxxx xx xxxx.
Xxx xxxxxx xxxx xxxxxxx xx xxx xxxxxxxx.

## XXXXX
Xxxx xxxxxx xxxx xxx xxxxxx xxxxxxxxxxx xxxxxxxxx.
Xx xxxxxx xxxxxxxxxxx xxxxxxxxx$ xxx xxx xxx xxx xxxxxxxxxxx xxxxxxxx xxxxxxxx.

## XXXXXXX XXXXX

[Clear-Variable]()

[New-Variable]()

[Remove-Variable]()

[Set-Variable]()

