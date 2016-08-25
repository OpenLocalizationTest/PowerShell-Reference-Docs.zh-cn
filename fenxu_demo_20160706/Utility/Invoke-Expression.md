---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293986
schema: 2.0.0
---

# Invoke-Expression
## XXXXXXXX
Xxxx xxxxxxxx xx xxxxxxxxxxx xx xxx xxxxx xxxxxxxx.

## XXXXXX

```
Invoke-Expression [-Command] <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxxxxxxxxx xxxxxx xxxxxxxxx xx xxxx x xxxxxxxxx xxxxxx xx x xxxxxxx xxx xxxxxxx xxx xxxxxxx xx xxx xxxxxxxxxx xx xxxxxxx.
Xxxxxxx Xxxxxx$Xxxxxxxxxx$ x xxxxxx xxxxxxxxx xx xxx xxxxxxx xxxx xxxxx xx xxxxxxxx $xxxxxx$ xxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$command = "Get-Process"
PS C:\>$command
Get-Process

PS C:\>invoke-expression $command

Handles  NPM(K)    PM(K)      WS(K) VM(M)   CPU(s)     Id   ProcessName
-------  ------    -----      ----- -----   ------     --   -----------
296       4       1572       1956    20       0.53     1348   AdtAgent
270       6       1328       800     34       0.06     2396   alg
67        2       620        484     20       0.22     716    ati2evxx
1060      15      12904      11840   74       11.48    892    CcmExec
1400      33      25280      37544   223      38.44    2564   communicator
...
```

Xxxx xxxxxxx xxxxxxxxxxxx xxx xxx xx Xxxxxx$Xxxxxxxxxx xx xxxxxxxx xx xxxxxxxxxx.
Xxxxxxx Xxxxxx$Xxxxxxxxxx$ xxx xxxxxxxxxx xx xxxxxxx$ xxx xxx xxxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxxx xx $Xxx$Xxxxxxx$ $x xxxxxx$ xx xxx $xxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxx xxx xxxxxx xx xxxxxx xxx xxxxxxxx xxxx xx xxx xxxxxxx xxxx.
Xxxxxxx XxxxxXxxxx xxxxxx xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx Xxxxxx$Xxxxxxxxxx xx xxxxxxxx xxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>invoke-expression -command "C:\ps-test\testscript.ps1"
PS C:\>"C:\ps-test\testscript.ps1" | invoke-expression
```

Xxxxx xxxxxxxx xxx Xxxxxx$Xxxxxxxxxx xx xxx x xxxxxx$ XxxxXxxxxx.xx0$ xx xxx xxxxx xxxxxxxx.
Xxx xxx xxxxxxxx xxx xxxxxxxxxx.
Xxx xxxxx xxxx xxx Xxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxxx xx xxx.
Xxx xxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xxxxxx xx Xxxxxx$Xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$Command = 'Get-Process | where {$_.cpu -gt 1000}'
PS C:\>Invoke-Expression $Command
```

Xxxx xxxxxxx xxxx x xxxxxxx xxxxxx xxxx xx xxxxx xx xxx $Xxxxxxx xxxxxxxx.

Xxx xxxxxxx xxxxxx xx xxxxxxxx xx xxxxxx xxxxxxxxx xxxxx xxxxxxx xx xxxxxxxx x xxxxxxxx$ $$$ xxxxx xxxxxxxxxx xxx xxxxxxx xxxxxx. Xx xx xxxx xxxxxxxx xx xxxxxx xxxxxxxxx xxxxx$ xxx $$ xxxxxxxx xxxxx xx xxxxxxxx xx xxx xxxxx xxxxxx xx xxx xxxxx xx xxx $Xxxxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$cmdlet_name = "get-eventlog"
PS C:\>$example_number = 1
PS C:\>$example_code = (get-help $cmdlet_name).examples.example[($example_number-1)].code
PS C:\>invoke-expression $example_code
```

Xxxx xxxxxxx xxxxxxxxx xxx xxxx xxx xxxxx xxxxxxx xx xxx Xxx$XxxxxXxx xxxxxx xxxx xxxxx.

Xx xxx xx xxxxxxx xx x xxxxxxxxx xxxxxx$ xxxxxx xxx xxxxx xx xxx $xxxxxx$xxxx xxxxxxxx xx xxx xxxx xx xxx xxxxxx.
Xxx$ xxxxxx xxx $xxxxxxx$xxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxx xxx xxxx xx xxx.
Xxx xxxxxxx xxxx xxxx xx xxx xxxxxxx xxxxxx xx xxx xxxxx.

## XXXXXXXXXX

### -Command
Xxxxxxxxx xxx xxxxxxx xx xxxxxxxxxx xx xxx.
Xxxx xxx xxxxxxx xx xxxxxxxxxx xx xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx xxxxxxxxxx.
Xxx Xxxxxxx xxxxxxxxx xx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
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

## XXXXXX

### System.String or PSObject
Xxx xxx xxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxx xx Xxxxxx$Xxxxxxxxxx.
Xxx xxx $xxxxx xxxxxxxxx xxxxxxxx xx xxxxxxxxx xxx xxxxx xxxxxxx xx xxx xxxxxxx.

## XXXXXXX

### PSObject
Xxxxxxx xxx xxxxxx xxxx xx xxxxxxxxx xx xxx xxxxxxx xxxxxxx $xxx xxxxx xx xxx Xxxxxxx xxxxxxxxx$.

## XXXXX
$$ Xx xxxxxxxxxx xx x xxxxxxxxx xxxx xxx xx xxxxxxxxx xxx xxxxxxxx x xxxxxx$ xxxx xx x Xxxxxxx XxxxxXxxxx xxxxxxx.
$$ Xxxx xxxxxxxxxx xxxxxxxxxxx xxxx xxxxx xxx Xxxxxx$Xxxxxxxxxx xxxxxx xx xxxxxxx. Xxxx xxxxx Xxxxxx$Xxxxxxxxxx xx xxx x xxxxxxx xxxx xxx xxxx xxxxxx$ xxxxxx xxxx xxx xxxxxxx xx xxxx xx xxx xxxxxx xxxxxxx xx. Xx xxxxxxx$ xx xx xxxx xx xxxxxx xxxx xxxxxx xxxx xxxxxxxxxx xxxxx xxxxxxx$ xxxxxx xxxx xxxxxxxx xxxxxxxx xxxxx.

## XXXXXXX XXXXX

[Invoke-Command]()

