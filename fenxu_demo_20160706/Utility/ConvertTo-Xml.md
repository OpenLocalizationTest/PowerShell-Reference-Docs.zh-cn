---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293952
schema: 2.0.0
---

# ConvertTo-Xml
## XXXXXXXX
Xxxxxxx xx XXX$xxxxx xxxxxxxxxxxxxx xx xx xxxxxx.

## XXXXXX

```
ConvertTo-Xml [-Depth <Int32>] [-InputObject] <PSObject> [-NoTypeInformation] [-As <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx XxxxxxxXx$Xxx xxxxxx xxxxxxx xx XXX$xxxxx xxxxxxxxxxxxxx xx xxx xx xxxx Xxxxxxxxx .XXX Xxxxxxxxx xxxxxxx.
Xx xxx xxxx xxxxxx$ xxxx xxx xx xxxx xxxxxxx xx xxx xxxxxx$ xx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxx.

Xxxx xxx xxxx xxxxxxxx xxxxxxx xx XxxxxxxXx$XXX xx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxx xxxxxxxx xxxxxxx$ XxxxxxxXx$XXX xxxxxxx x xxxxxx XXX xxxxxxxx xxxx xxxxxxxx xxxxxxxxxxxxxxx xx xxx xx xxx xxxxxxx.

Xxxx xxxxxx xx xxxxxxx xx Xxxxxx$Xxxxxx xxxxxx xxxx Xxxxxx$Xxxxxx xxxxxx xxx xxxxxxxxx XXX xx x xxxx.
XxxxxxxXx$XXX xxxxxxx xxx XXX$ xx xxx xxx xxxxxxxx xx xxxxxxx xx xx Xxxxxxx XxxxxXxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-date | convertto-xml
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxx xxxx $x XxxxXxxx xxxxxx$ xx XXX.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>convertto-xml -as Document -inputObject (get-process) -depth 3
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxx xxxxxxx xxxx xxxxxxxxx xxx xx xxx xxxxxxxxx xx xxx xxxxxxxx xxxx xx XXX xxxxxxxx.
Xxx xxxxxxx xxx xxxxxxxx xx x xxxxx xx xxxxx xxxxxx.

## XXXXXXXXXX

### -As
Xxxxxxxxxx xxx xxxxxx xxxxxx.
Xxxxx xxxxxx xxx$

$$ Xxxxxx$  Xxxxxxx x xxxxxx xxxxxx.
$$ Xxxxxx$  Xxxxxxx xx xxxxx xx xxxxxxx.
$$ Xxxxxxxx$  Xxxxxxx xx XxxXxxxxxxx xxxxxx.

Xxx xxxxxxx xx Xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: Stream, String, Document

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Depth
Xxxxxxxxx xxx xxxx xxxxxx xx xxxxxxxxx xxxxxxx xxx xxxxxxxx xx xxx XXX xxxxxxxxxxxxxx.
Xxx xxxxxxx xxxxx xx 0.

Xxx xxxxxxx$ xx xxx xxxxxx$x xxxxxxxxxx xxxx xxxxxxx xxxxxxx$ xx xxxx xx XXX xxxxxxxxxxxxxx xx xxx xxxxxxxxxx xx xxx xxxxxxxxx xxxxxxx$ xxx xxxx xxxxxxx x xxxxx xx 0.

Xxx xxxxxxx xxxxx xxx xx xxxxxxxxxx xxx xxx xxxxxx xxxx xx xxx Xxxxx.xx0xxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxx.xx0xxx.

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

### -InformationAction
$$ Xxxxxx$  Xxxxxxx x xxxxxx xxxxxx.
$$ Xxxxxx$  Xxxxxxx xx xxxxx xx xxxxxxx.
$$ Xxxxxxxx$  Xxxxxxx xx XxxXxxxxxxx xxxxxx.

Xxx xxxxxxx xx Xxxxxxxx.

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
$$ Xxxxxx$  Xxxxxxx x xxxxxx xxxxxx.
$$ Xxxxxx$  Xxxxxxx xx xxxxx xx xxxxxxx.
$$ Xxxxxxxx$  Xxxxxxx xx XxxXxxxxxxx xxxxxx.

Xxx xxxxxxx xx Xxxxxxxx.

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

### -InputObject
Xxxxxxxxx xxx xxxxxx xx xx xxxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx$ xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.
Xxx xxx xxxx xxxx xxxxxxx xx XxxxxxxXx$XXX.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NoTypeInformation
Xxxxx xxx Xxxx xxxxxxxxx xxxx xxx xxxxxx xxxxx.

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

### System.Management.Automation.PSObject
Xxx xxx xxxx xxx xxxxxx xx XxxxxxxXx$XXX.

## XXXXXXX

### System.String or System.Xml.XmlDocument
Xxx xxxxx xx xxx Xx xxxxxxxxx xxxxxxxxxx xxx xxxx xx xxxxxx xxxx XxxxxxxXx$XXX xxxxxxx.

## XXXXX

## XXXXXXX XXXXX

[ConvertTo-Csv]()

[ConvertTo-Html]()

[Export-Clixml]()

[Import-Clixml]()

