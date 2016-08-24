---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293996
schema: 2.0.0
---

# Xxx$Xxxx
## XXXXXXXX
Xxxxx xxxxxx xx x xxxx.

## XXXXXX

### XxXxxx $Xxxxxxx$
```
Out-File [-FilePath] <String> [[-Encoding] <String>] [-Append] [-Force] [-NoClobber] [-Width <Int32>]
 [-NoNewline] [-InputObject <PSObject>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

### XxXxxxxxxXxxx
```
Out-File -LiteralPath <String> [[-Encoding] <String>] [-Append] [-Force] [-NoClobber] [-Width <Int32>]
 [-NoNewline] [-InputObject <PSObject>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxx xxxxxx xxxxx xxxxxx xx x xxxx.
Xxx xxx xxx xxxx xxxxxx xxxxxxx xx xxx xxxxxxxxxxx xxxxxxxx $$$$ xxxx xxx xxxx xx xxx xxx xxxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | out-file -filepath C:\Test1\process.txt
```

Xxxx xxxxxxx xxxxx x xxxx xx xxxxxxxxx xx xxx xxxxxxxx xx xxx Xxxxxxx.xxx xxxx.
Xx xxx xxxx xxxx xxx xxxxx$ Xxx$Xxxx xxxxxxx xx.
Xxxxxxx xxx xxxx xx xxx XxxxXxxx xxxxxxxxx xx xxxxxxxx$ xxx xxx xxxx xx xxx xxxxxx xxx xxxxxxxxxx xxxxxxx $xxx$xxxxxxx $ xxxxxxx X$$Xxxx0$xxxxxxx.xxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | out-file C:\Test1\process.txt -noclobber

Out-File : File C:\Test1\process.txt already exists and NoClobber was specified.
At line:1 char:23
+ get-process | out-file  <<<< process.txt -noclobber
```

Xxxx xxxxxxx xxxx xxxxx x xxxx xx xxxxxxxxx xx xxx Xxxxxxx.xxx xxxx$ xxx xx xxxx xxx XxXxxxxxx xxxxxxxxx$ xxxxx xxxxxxxx xx xxxxxxxx xxxx xxxx xxxxx xxxxxxxxxxx.
Xxx xxxxxx xxxxx xxx xxxxx xxxxxxx xxxx xxxxxxx xxxx XxXxxxxxx xx xxxx xxxx xx xxxxxxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = get-process
PS C:\>out-file -filepath C:\Test1\process.txt -inputobject $a -encoding ASCII -width 50
```

Xxxxx xxxxxxxx xxxx x xxxx xx xxxxxxxxx xx xxx xxxxxxxx xx xxx Xxxxxxx.xxx xxxx.
Xxx xxxx xx xxxxxxx xx XXXXX xxxxxx xx xxxx xx xxx xx xxxx xx xxxxxx xxxxxxxx xxxx Xxxxxxx xxx Xxxx.
Xx xxxxxxx$ Xxx$Xxxx xxxx Xxxxxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxx xx xxxxxxxxx xxx xxxxxx xxxx xx xxx $x xxxxxxxx.
Xxx xxxxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxxx xxx xxxx xx xxx Xxxxxxx.xxx xxxx.

Xxx xxxxxxx xxxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxxx xxxx xxx xxxxx xx xx xxx $x xxxxxxxx.
Xx xxxx xxx Xxxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxx xx XXXXX xxxxxx.
Xx xxxx xxx Xxxxx xxxxxxxxx xx xxxxx xxxx xxxx xx xxx xxxx xx 00 xxxxxxxxxx.
Xxxxxxx xxx xxxxx xx xxxxxx xxx xxxxxxxxx xx 00 xxxxxxxxxx$ xxx xxxxxxxxx xxxxxx xx xxx xxxxxxx xxxxx xx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-location hklm:\software
PS C:\>get-acl mycompany\mykey | out-file -filepath c:\ps\acl.txt
PS C:\>get-acl mycompany\mykey | out-file -filepath filesystem::acl.txt
```

Xxxxx xxxxxxxx xxxx xxx xx xxx xxx Xxx$Xxxx xxxxxx xxxx xxx xxx xxx xx x XxxxXxxxxx xxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxxx xx xxx XXXX$$Xxxxxxxx xxxxxxxx xxx.

Xxx xxxxxx xxx xxxxx xxxxxxxx xxxx xxx xxxx xxxxxx.
Xxxx xxx xxx Xxx$Xxx xxxxxx xx xxx xxx xxxxxxxx xxxxxxxxxx xx xxx XxXxx xxxxxxxx xxxxxx $XXXX$Xxxxxxxx$XxXxxxxxx$XxXxx$.
X xxxxxxxx xxxxxxxx xxxxxx xxx xxxxxx xx xxx Xxx$Xxxx xxxxxx$ xxxxx xxxxx xx xx xxx Xxx.xxx xxxx.

Xxxxxxx Xxx$Xxxx xx xxx xxxxxxxxx xx xxx Xxxxxxx XxxxxXxxxx Xxxxxxxx xxxxxxxx$ xxx xxxx xxxxxxx xxxxxx xxx xxxx xxxxxx xxxxx xxxx$ xxxx xx $x$$$ xx xxx xxxx xx xxx xxxxxxxx xxxxxxxx xx xxx xxxxxx$ $XxxxXxxxxx$$$$ xx xxx xxxxx xx xxx XxxxXxxx xxxxxxxxx.
Xxx xxxxxx xxx xxxxx xxxxxxxx xxxxxxxxxxx xxxxx xxxxxxx.

## XXXXXXXXXX

### $Xxxxxx
Xxxx xxx xxxxxx xx xxx xxx xx xx xxxxxxxx xxxx$ xxxxxxx xx xxxxxxxxx xxx xxxx xxxxxxxx.

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

### $Xxxxxxxx
Xxxxxxxxx xxx xxxx xx xxxxxxxxx xxxxxxxx xxxx xx xxx xxxx.
Xxxxx xxxxxx xxx $Xxxxxxx$$ $XXX0$$ $XXX0$$ $XXX00$$ $XXXXX$$ $XxxXxxxxxXxxxxxx$$ $Xxxxxxx$$ xxx $XXX$.
$Xxxxxxx$ xx xxx xxxxxxx.

$Xxxxxxx$ xxxx xxx xxxxxxxx xx xxx xxxxxx$x xxxxxxx XXXX xxxx xxxx.

$XXX$ xxxx xxx xxxxxxx xxxxxxxx xxxxxxxxx xxxxxxxxxxxx xxxx xxxx xxxxxxxxxx xxx xxx xxxxxxxxx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: unknown, string, unicode, bigendianunicode, utf8, utf7, utf32, ascii, default, oem

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxx.

```yaml
Type: String
Parameter Sets: ByPath
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxx
Xxxxxx xxx xxxxxx xx xxxxxxxxx xx xxxxxxxx xxxx$xxxx xxxx.
Xxxx xxxxx xxx Xxxxx xxxxxxxxx$ xxx xxxxxx xxxxxx xxxxxxxx xxxxxxxx xxxxxxxxxxxx.

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

### $XxxxxXxxxxx
Xxxxxxxxx xxx xxxxxxx xx xx xxxxxxx xx xxx xxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.

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

### $XxXxxxxxx
Xxxx xxx xxxxxxxxx $xxxxxxx xxx xxxxxxxx$ xx xx xxxxxxxx xxxx.
Xx xxxxxxx$ xx x xxxx xxxxxx xx xxx xxxxxxxxx xxxx$ Xxx$Xxxx xxxxxxxxxx xxx xxxx xxxxxxx xxxxxxx.
Xx xxxx Xxxxxx xxx XxXxxxxxx xxx xxxx$ xxx xxxxxx xx xxxxxxxx xx xxx xxxxxxxx xxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: NoOverwrite

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxx
Xxxxxxxxx xxx xxxxxx xx xxxxxxxxxx xx xxxx xxxx xx xxxxxx.
Xxx xxxxxxxxxx xxxxxxxxxx xxx xxxxxxxxx$ xxx xxxxxxx.
Xx xxx xxxx xxxx xxxxxxxxx$ xxx xxxxx xx xxxxxxxxxx xx xxx xxxxxxxxxxxxxxx xx xxx xxxx.
Xxx xxxxxxx xxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xx 00 $xxxxxxxxxx$.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxx.
Xxxxxx XxxxXxxx$ xxx xxxxx xx xxx XxxxxxxXxxx xxxxxxxxx xx xxxx xxxxxxx xx xx xx xxxxx.
Xx xxxxxxxxxx xxx xxxxxxxxxxx xx xxxxxxxxx.
Xx xxx xxxx xxxxxxxx xxxxxx xxxxxxxxxx$ xxxxxxx xx xx xxxxxx xxxxxxxxx xxxxx.
Xxxxxx xxxxxxxxx xxxxx xxxx Xxxxxxx XxxxxXxxxx xxx xx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: ByLiteralPath
Aliases: PSPath

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxx
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

### $XxxxXx
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

### $XxXxxxxxx
$$Xxxx XxXxxxxxx Xxxxxxxxxxx$$

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxx xxxx xxx xxxxxx xx Xxx$Xxxx.

## XXXXXXX

### Xxxx
Xxx$Xxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xxx Xxx xxxxxxx xx xxx xxxxxx xxxxxxx$ xxxx xxxx xxxxxx xxxx xxx xxxx xxxx xx xxx xxxxxxxxx xxxxxxx xxxxxxxxxxx.
Xx xxx xxxx xx xxxxxxxxxxx xxxxxx xx xx Xxx xxxxxx$ xxx xxxxxx xxxxx xx xx x xxxxxxxxxx xxxxxx xxxxxx xxxxxxxxx xx.

Xxx Xxx xxxxxxx xx xxx xxxx xxxxxxxxxx xxx xxxxx xx xxxx xxxxx.
Xx xxxx xxxx xx x xxxxxx xxxx xxxxxxxx xxx Xxx xxxx $xx Xxx xxxxxx$$ xxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xx x Xxxxxxx XxxxxXxxxx xxxxxxx xx xxx xxxxxx.
Xxx xxx xxxx xxxxx xxxx xx x xxxxxxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxx xxx xxxx xx xxx xxxxxx.
Xxx xxxx$ xxx xxx xxxxxxxx.

Xxx$Xxxx xxxxx xxxx$ xxx xx xxxx xxx xxxx xxx xxxxxx xxxxxxx.
Xx xxx xxxx xxx xxxxxx xx Xxx$Xxxx xx Xxx$Xxxxxx$ Xxx$Xxxxxx xxxxxxx xxxx xx xxxxxxx xxxx xxxx xxxxxxxxx.

## XXXXXXX XXXXX

[Xxx$Xxxxxxx]()

[Xxx$Xxxx]()

[Xxx$Xxxx]()

[Xxx$Xxxxxxx]()

[Xxx$Xxxxxx]()

[Xxx$Xxxxxx]()

