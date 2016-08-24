---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294019
schema: 2.0.0
---

# Xxx$Xxxxxx
## XXXXXXXX
Xxxxx xxxxxxx xxxxxx xx x xxxx xx xxxxxxxx xxx xxxx xxxxx xx xxxx xxx xxxxxxxx.

## XXXXXX

### Xxxx $Xxxxxxx$
```
Tee-Object [-InputObject <PSObject>] [-FilePath] <String> [-Append] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### XxxxxxxXxxx
```
Tee-Object [-InputObject <PSObject>] -LiteralPath <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### Xxxxxxxx
```
Tee-Object [-InputObject <PSObject>] -Variable <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxx xxxxxx xxxxxxxxx xxxxxx$ xxxx xx$ xx xxxxx xxx xxxxxx xx x xxxxxxx xx xxx xxxxxxxxxx $xxxx xxx xxxxxx $X$$.
Xx xxxxxx xxx xxxxxx xx x xxxx xx xxxxxxxx xxx xxxx xxxxx xx xxxx xxx xxxxxxxx.
Xx Xxx$Xxxxxx xx xxx xxxx xxxxxxx xx xxx xxxxxxxx$ xxx xxxxxxx xxxxxx xx xxxxxxxxx xx xxx xxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | tee-object -filepath C:\Test1\testfile2.txt

Handles  NPM(K)    PM(K)      WS(K) VM(M)   CPU(s)    Id ProcessName
-------  ------    -----      ----- -----   ------    -- -----------
83       4     2300       4520    39     0.30    4032 00THotkey
272      6     1400       3944    34     0.06    3088 alg
81       3      804       3284    21     2.45     148 ApntEx
81       4     2008       5808    38     0.75    3684 Apoint
...
```

Xxxx xxxxxxx xxxx x xxxx xx xxx xxxxxxxxx xxxxxxx xx xxx xxxxxxxx xxx xxxxx xxx xxxxxx xx x xxxx.
Xxxxxxx x xxxxxx xxxx xx xxx xxxxxxxxx$ xxx xxxxxxxxx xxx xxxx xxxxxxxxx xx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process notepad | tee-object -variable proc | select-object processname,handles

ProcessName                              Handles
-----------                              -------
notepad                                  43
notepad                                  37
notepad                                  38
notepad                                  38
```

Xxxx xxxxxxx xxxx x xxxx xx xxx xxxxxxxxx xxxxxxx xx xxx xxxxxxxx xxx xxxxx xxx xxxxxx xx x xxxxxxxx xxxxx $xxxx$.
Xx xxxx xxxxx xxx xxxxxxxxx xxxxxxx xxxxx xx Xxxxxx$Xxxxxx$ xxxxx xxxxxxx xxx XxxxxxxXxxx xxx Xxxxxxx xxxxxxxx.
Xxxx xxxx xxx $xxxx xxxxxxxx xxxxxxxx xxx xxxxxxx xxxxxxxxxxx xxxxxxxx xx Xxx$Xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-childitem -path D: -file -system -recurse | tee-object -file c:\test\AllSystemFiles.txt -append | out-file c:\test\NewSystemFiles.txt
```

Xxxx xxxxxxx xxxxx x xxxx xx xxxxxx xxxxx xx x xxx xxx xxxxx$ x xxxxxxxxxx xxxx xxx x xxxxxxx xxxx.

Xxx xxxxxxx xxxx xxx Xxx$XxxxxXxxx xxxxxx xx xx x xxxxxxxxx xxxxxx xxx xxxxxx xxxxx xx xxx X$ xxxxx.
X xxxxxxxx xxxxxxxx $$$ xxxxx xxx xxxx xx Xxx$Xxxxxx$ xxxxx xxxxxxx xxx xxxx xx xxx XxxXxxxxxXxxxx.xxx xxxx xxx xxxxxx xxx xxxx xxxx xxx xxxxxxxx xx xxx Xxx$Xxxx xxxxxx$ xxxxx xxxxx xxx xxxx xx xxx XxxXxxxxxXxxxx.xxx xxxx.

## XXXXXXXXXX

### $Xxxxxx
Xxxxxxx xxx xxxxxx xx xxx xxxxxxxxx xxxx.
Xxxxxxx xxxx xxxxxxxxx$ xxx xxx xxxxxxx xxxxxxxx xxx xxxxxxxx xxxxxxx xx xxx xxxx xxxxxxx xxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: SwitchParameter
Parameter Sets: File
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxxx xxx xxxxxx xx xxx xxxxxxxxx xxxx.
Xxxxxxxx xxxxxxxxxx xxx xxxxxxxxx$ xxx xxxx xxxxxxx xx x xxxxxx xxxx.

```yaml
Type: String
Parameter Sets: File
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxxxXxxxxx
Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

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
Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

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

### $XxxxxXxxxxx
Xxxxxxxxx xxx xxxxxx xx xx xxxxx xxx xxxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.
Xxx xxx xxxx xxxx xx xxxxxx xx Xxx$Xxxxxx.

Xxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xxxx Xxx$Xxxxxx$ xxxxxxx xx xxxxxx xxxxxxx xxxxxxx xx Xxx$Xxxxxx$ xxx XxxxxXxxxxx xxxxx$xxxx xx xxx xxxxx xx x xxxxxxxxxx xxxx xx xxx xxxxxx xx x xxxxxxx$ xxxx xx $XxxxxXxxxxx $Xxx$Xxxxxxx$$xx xxxxxxx xx x xxxxxx xxxxxx.
Xxxxxxx XxxxxXxxxxx xxxxxx xxxxxx xxxxxxxxxx xxxxxxxxxx xxxx xx xxxxx xx xxxxxxxxxx xx xxxxxxx$ xx xx xxxxxxxxxxx xxxx xx xxx xxx Xxx$Xxxxxx xx xxxxxxx xxxxxxxxxx xx x xxxxxxxxxx xx xxxxxxx xxx xxxxx xxxxxxx xxxx xxxx xxxxxxxx xxxxxx xx xxxxxxx xxxxxxxxxx$ xxx xxx Xxx$Xxxxxx xx xxx xxxxxxxx$ xx xxxxx xx xxx xxxxxxxx xx xxxx xxxxx.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $Xxxxxxxx
Xxxxx xxx xxxxxx xx xxx xxxxxxxxx xxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxx xxx xxxxxxxxx xxxxxx xxxx $$$.

```yaml
Type: String
Parameter Sets: Variable
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxx
Xxxxx xxx xxxxxx xx xxx xxxxxxxxx xxxx.
Xxxxxx XxxxXxxx$ xxx xxxxx xx xxx XxxxxxxXxxx xxxxxxxxx xx xxxx xxxxxxx xx xx xx xxxxx.
Xx xxxxxxxxxx xxx xxxxxxxxxxx xx xxxxxxxxx.
Xx xxx xxxx xxxxxxxx xxxxxx xxxxxxxxxx$ xxxxxxx xx xx xxxxxx xxxxxxxxx xxxxx.
Xxxxxx xxxxxxxxx xxxxx xxxx Xxxxxxx XxxxxXxxxx xxx xx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: LiteralFile
Aliases: PSPath

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxx xxxx xxxxxxx xx Xxx$Xxxxxx.

## XXXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx$Xxxxxx xxxxxxx xxx xxxxxx xxxx xx xxxxxxxxx.

## XXXXX
Xxx xxx xxxx xxx xxx Xxx$Xxxx xxxxxx xx xxx xxxxxxxxxxx xxxxxxxx$ xxxx xx xxxxx xxxx xxx xxxxxx xx x xxxx xxx xx xxx xxxx xx xxxx xxx xxxxxxxx.

Xxx$Xxxxxx xxxx Xxxxxxx xxxxxxxx xxxx xx xxxxxx xx xxxxx.
Xx x xxxxxx$ xxx xxxxxx xxxxx xxx xx xxxxxxxxx xxxxxxxx xx xxxxx xxxx x xxxxxxxxx xxxxxxxx.
Xx xxxxxxx xxx xxxxxxxx$ xxx xxx Xxx$Xxxx xxxxxx.

## XXXXXXX XXXXX

[Xxxxxx$Xxxxxx]()

[xxxxx$Xxxxxxxxxxx]()

