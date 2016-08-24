---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294033
schema: 2.0.0
---

# Xxxxx$Xxxxxxx
## XXXXXXXX
Xxxxxx x xxxxxxx xxxxxxx.

## XXXXXX

```
Write-Warning [-Message] <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxx$Xxxxxxx xxxxxx xxxxxx x xxxxxxx xxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxx.
Xxx xxxxxxxx xx xxx xxxxxxx xxxxxxx xx xxx xxxxx xx xxx xxxx$x $XxxxxxxXxxxxxxxxx xxxxxxxx xxx xxx xxx xx xxx XxxxxxxXxxxxx xxxxxx xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>write-warning "This is only a test warning."
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxx $XXXXXXX$ Xxxx xx xxxx x xxxx xxxxxxx.$

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$w = "This is only a test warning."
PS C:\>$w | write-warning
```

Xxxx xxxxxxx xxxxx xxxx xxx xxx xxx x xxxxxxxx xxxxxxxx $$$ xx xxxx x xxxxxx xx Xxxxx$Xxxxxxx.
Xxx xxx xxxx xxx xxxxxx xx x xxxxxxxx$ xx xxxxx xx xxxx xxxxxxx$ xx xxxx xxx xxxxxx xxxxxxxx xx Xxxxx$Xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$warningpreference
Continue

PS C:\>write-warning "This is only a test warning."
This is only a test warning.

PS C:\>$warningpreference = "SilentlyContinue"
PS C:\>write-warning "This is only a test warning."
PS C:\>
PS C:\>$warningpreference = "Stop"
PS C:\>write-warning "This is only a test warning."

WARNING: This is only a test message.
Write-Warning : Command execution stopped because the shell variable "WarningPreference" is set to Stop.
At line:1 char:14
     + write-warning <<<<  "This is only a test message."
```

Xxxx xxxxxxx xxxxx xxx xxxxxx xx xxx xxxxx xx xxx $XxxxxxxXxxxxxxxxx xxxxxxxx xx x Xxxxx$Xxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxxx xxx xxxxxxx xxxxx xx xxx $XxxxxxxXxxxxxxxxx xxxxxxxx$ xxxxx xx $Xxxxxxxx$.
Xx x xxxxxx$ xxxx xxx xxxxx x xxxxxxx$ xxx xxxxxxx xxxxxxx xx xxxxxxxxx xxx xxxxxxxxx xxxxxxxxx.

Xxxx xxx xxxxxx xxx xxxxx xx xxx $XxxxxxxXxxxxxxxxx xxxxxxxx$ xxx xxxxxx xx xxx Xxxxx$Xxxxxxx xxxxxxx xxxxxxx xxxxx.
X xxxxx xx $XxxxxxxxXxxxxxxx$ xxxxxxxxxx xxx xxxxxxx.
X xxxxx xx $Xxxx$ xxxxxxxx xxx xxxxxxx xxx xxxx xxxxx xxxxxxxxx xx xxx xxxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxx $XxxxxxxXxxxxxxxxx xxxxxxxx$ xxx xxxxx$Xxxxxxxxxx$Xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>write-warning "This is only a test warning." -warningaction Inquire

WARNING: This is only a test warning.
Confirm
Continue with this operation?
[Y] Yes  [A] Yes to All  [H] Halt Command  [S] Suspend  [?] Help (default is "Y"):
```

Xxxx xxxxxxx xxxxx xxx xxxxxx xx xxx XxxxxxxXxxxxx xxxxxx xxxxxxxxx xx x Xxxxx$Xxxxxxx xxxxxxx.
Xxx xxx xxx xxx XxxxxxxXxxxxx xxxxxx xxxxxxxxx xxxx xxx xxxxxx xx xxxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx xx xxxxxxxx xxxxxxxxx xxxx xxxx xxxxxxx.
Xxx XxxxxxxXxxxxx xxxxxx xxxxxxxxx xxxxxxxxx xxx xxxxx xx xxx $XxxxxxxXxxxxxxxxx xxxx xxx xxxx xxxxxxxxxx xxxxxxx.

Xxxx xxxxxxx xxxx xxx Xxxxx$Xxxxxxx xxxxxx xx xxxxxxx x xxxxxxx.
Xxx XxxxxxxXxxxxx xxxxxx xxxxxxxxx xxxx x xxxxx xx $Xxxxxxx$ xxxxxxx xxx xxxxxx xx xxxxxx xxx xxxx xxxx xxx xxxxxxx xxxxxxxx x xxxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxx XxxxxxxXxxxxx xxxxxx xxxxxxxxx$ xxx xxxxx$XxxxxxXxxxxxxxxx.

## XXXXXXXXXX

### $XxxxxxxxxxxXxxxxx
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

### $XxxxxxxxxxxXxxxxxxx
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

### $Xxxxxxx
Xxxxxxxxx xxx xxxxxxx xxxxxxx.

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

### Xxxxxx.Xxxxxx
Xxx xxx xxxx x xxxxxx xxxx xxxxxxxx xxx xxxxxxx xx Xxxxx$Xxxxxxx.

## XXXXXXX

### Xxxx
Xxxxx$Xxxxxxx xxxxxx xxxx xx xxx xxxxxxx xxxxxx.
Xx xxxx xxx xxxxxxxx xxx xxxxx xxxxxx.

## XXXXX
Xxx xxxxxxx xxxxx xxx xxx $XxxxxxxXxxxxxxxxx xxxxxxxx xx $Xxxxxxxx$$ xxxxx xxxxxxxx xxx xxxxxxx xxx xxxx xxxxxxxxx xxxxxxxxx xxx xxxxxxx.
Xx xxxxxxxxx xxxxx xxxxxx xxx x xxxxxxxxxx xxxxxxxx xxxx xx $XxxxxxxXxxxxxxxxx$ xxx xx xx x xxxxxx xx xxxxxx xxxxxxxxxx$ xxxx xx $xxx$.
Xxx xxxxxxxxx xxxxx xxxxxxx xxxx xxxx xxx xxxxx xxxxxx.

## XXXXXXX XXXXX

[Xxxxx$Xxxxx]()

[Xxxxx$Xxxxx]()

[Xxxxx$Xxxx]()

[Xxxxx$Xxxxxx]()

[Xxxxx$Xxxxxxxx]()

[Xxxxx$Xxxxxxx]()

[xxxxx$XxxxxxXxxxxxxxxx]()

[xxxxx$Xxxxxxxxxx$Xxxxxxxxx]()

