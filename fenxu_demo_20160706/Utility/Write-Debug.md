---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294027
schema: 2.0.0
---

# Write-Debug
## XXXXXXXX
Xxxxxx x xxxxx xxxxxxx xx xxx xxxxxxx.

## XXXXXX

```
Write-Debug [-Message] <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxx$Xxxxx xxxxxx xxxxxx xxxxx xxxxxxxx xx xxx xxxxxxx xxxx x xxxxxx xx xxxxxxx.

Xx xxxxxxx$ xxxxx xxxxxxxx xxx xxx xxxxxxxxx xx xxx xxxxxxx$ xxx xxx xxx xxxxxxx xxxx xx xxxxx xxx Xxxxx xxxxxxxxx xx xxx $XxxxxXxxxxxxxxx xxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Write-Debug "Cannot open file."
```

Xxxx xxxxxxx xxxxxx x xxxxx xxxxxxx.
Xxxxxxx xxx xxxxx xx $XxxxxXxxxxxxxxx xx $XxxxxxxxXxxxxxxx$$ xxx xxxxxxx xx xxx xxxxxxxxx xx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$DebugPreference
SilentlyContinue
PS C:\>Write-Debug "Cannot open file."
PS C:\>
PS C:\>Write-Debug "Cannot open file." -debug
DEBUG: Cannot open file.
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx Xxxxx xxxxxx xxxxxxxxx xx xxxxxxxx xxx xxxxx xx xxx $XxxxxXxxxxxxxxx xxxxxxxx xxx x xxxxxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxxx xxx xxxxx xx xxx $XxxxxXxxxxxxxxx xxxxxxxx$ xxxxx xx $XxxxxxxxXxxxxxxx$$ xxx xxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxx x xxxxx xxxxxxx xxx$ xxxxxxx xx xxx xxxxx xx $XxxxxXxxxxxxxxx$ xxx xxxxxxx xxxx xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxxxx x xxxxx xxxxxxx.
Xx xxxx xxx Xxxxx xxxxxx xxxxxxxxx xx xxxxxxxx xxx xxxxx xx $XxxxxXxxxxxxxxx xxx xx xxxxxxx xxx xxxxx xxxxxxxx xxxxxxxxx xxxx xxxx xxxxxxx.

Xx x xxxxxx$ xxxx xxxxxx xxx xxxxx xx $XxxxxXxxxxxxxxx xx $XxxxxxxxXxxxxxxx$$ xxx xxxxx xxxxxxx xxxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxx Xxxxx xxxxxx xxxxxxxxx$ xxx xxxxx$XxxxxxXxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$DebugPreference
SilentlyContinue
PS C:\>Write-Debug "Cannot open file."
PS C:\>
PS C:\>$DebugPreference = "Continue"
PS C:\>Write-Debug "Cannot open file."
DEBUG: Cannot open file.
```

Xxxx xxxxxxx xxxxx xxx xxxxxx xx xxxxxxxx xxx xxxxx xx xxx $XxxxxXxxxxxxxxx xxxxxxxx xx xxx xxxxxxx xx xxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxxx xxx xxxxx xx xxx $XxxxxXxxxxxxxxx xxxxxxxx$ xxxxx xx $XxxxxxxxXxxxxxxx$$ xxx xxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxx x xxxxx xxxxxxx xxx$ xxxxxxx xx xxx xxxxx xx $XxxxxXxxxxxxxxx$ xxx xxxxxxx xxxx xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxxx xx $Xxxxxxxx$ xx xxx $XxxxxXxxxxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxx x xxxxx xxxxxxx$ xxxxx xxxxxxx xx xxx xxxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx $XxxxxXxxxxxxxxx$ xxx xxxxx$Xxxxxxxxxx$Xxxxxxxxx.

## XXXXXXXXXX

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

### -Message
Xxxxxxxxx xxx xxxxx xxxxxxx xx xxxx xx xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Msg

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## XXXXXX

### System.String
Xxx xxx xxxx x xxxxxx xxxx xxxxxxxx x xxxxx xxxxxxx xx Xxxxx$Xxxxx.

## XXXXXXX

### None
Xxxxx$Xxxxx xxxxxx xxxx xx xxx xxxxx xxxxxx.
Xx xxxx xxx xxxxxx xxx xxxxxx.

## XXXXX

## XXXXXXX XXXXX

[Write-Error]()

[Write-Host]()

[Write-Output]()

[Write-Progress]()

[Write-Verbose]()

[Write-Warning]()

