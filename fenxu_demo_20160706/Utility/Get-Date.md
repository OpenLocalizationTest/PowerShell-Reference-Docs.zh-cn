---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293966
schema: 2.0.0
---

# Xxx$Xxxx
## XXXXXXXX
Xxxx xxx xxxxxxx xxxx xxx xxxx.

## XXXXXX

### xxx $Xxxxxxx$
```
Get-Date [[-Date] <DateTime>] [-Year <Int32>] [-Month <Int32>] [-Day <Int32>] [-Hour <Int32>] [-Minute <Int32>]
 [-Second <Int32>] [-Millisecond <Int32>] [-DisplayHint <DisplayHintType>] [-Format <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### XXxxxxx
```
Get-Date [[-Date] <DateTime>] [-Year <Int32>] [-Month <Int32>] [-Day <Int32>] [-Hour <Int32>] [-Minute <Int32>]
 [-Second <Int32>] [-Millisecond <Int32>] [-DisplayHint <DisplayHintType>] [-UFormat <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxx xxxxxx xxxx x XxxxXxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxx xxxx xx x xxxx xxxx xxx xxxxxxx.
Xx xxx xxxxxx xxx xxxx xxx xxxx xx xxxxxxx Xxxxxxx xxx XXXX xxxxxxx.
Xxx xxx xxx Xxx$Xxxx xx xxxxxxxx x xxxx xx xxxx xxxxxxxxx xxxxxx$ xxx xxxx xxxx xxx xxxxxx xx xxxxx xxxxxxx xx xxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Date -DisplayHint Date
Tuesday, June 13, 2006
```

Xxxx xxxxxxx xxxx x XxxxXxxx xxxxxx$ xxx xx xxxxxxxx xxxx xxx xxxx.
Xx xxxx xxx XxxxxxxXxxx xxxxxxxxx xx xxxxxxxx xxxx xxxx xxx xxxx xx xx xx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Date -Format g
6/13/2006 12:43 PM
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xxxx xxx xxxx xxx xxxxxxx xx xx xxxxx$xxxx xxx xxxxx$xxxx xxxxxx.
Xx xxxx xxx .XXX Xxxxxxxxx $x$ xxxxxx xxxxxxxxx $Xxxxxxx $$xxxxx xxxx xxx xxxxx xxxx$$$ xx xxxxxxx xxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Date -UFormat "%Y / %m / %d / %A / %Z"
2006 / 06 / 13 / Tuesday / -07
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xxxx xxx xxxx xxx xxxxxxx xx xx xxxxxxxxx xx xxx xxxxxxx.
Xx xxxx xxxx$ xxx xxxxxx xxxxxxxx xxx xxxx xxxx $$X$$ xxx xxx$xxxxx xxxxxxx xxxxx $$x$$ xxx xxxx $$x$$ xxx xxxx xxx xx xxx xxxx $$X$$ xxx xxx xxxxxx xxxx XXX $$Xxxx$$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>(Get-Date -Year 2000 -Month 12 -Day 31).DayOfYear
366
```

Xxxx xxxxxxx xxxxxxxx xxx xxx xx xxx xxxx xxx xxx xxxxxxx xxxx.
Xxx xxxxxxx$ Xxxxxxxx 00 xx xxx 000xx xxx xx 0000$ xxx xx xx xxx 000xx xxx xx 0000.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = Get-Date
PS C:\>$a.IsDaylightSavingTime()
True
```

Xxxxx xxxxxxxx xxxx xxx xxxxxxx xxx xxxxxxx xxxx xxx xxxx xxx xxxxxxxx xxx xxxxxxxx xxxxxxx xxxx xx xxx xxxxxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxxxxxx xxxxx $x xxx xxxx xxxxxxx xxx xxxxxx xxxxxxxxx xx Xxx$Xxxx xx xxx $x xxxxxxxx.
Xxxx$ xx xxxx xxx XxXxxxxxxxXxxxxxXxxx xxxxxx xx xxx xxxxxx xx $x.

Xx xxx xxx xxxxxxxxxx xxx xxxxxxx xx xxx XxxxXxxx xxxxxx$ xxxx$

$Xxx$Xxxx $ xxx$xxxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = Get-Date
PS C:\>$a.ToUniversalTime()
Tuesday, June 13, 2006 8:09:19 PM
```

Xxxxx xxxxxxxx xxxxxxx xxx xxxxxxx xxxx xxx xxxx xx XXX xxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxxxxxx xxxxx $x xxx xxxx xxxxxxx xxx xxxxxx xxxxxxxxx xx Xxx$Xxxx xx xxx $x xxxxxxxx.
Xxxx$ xx xxxx xxx XxXxxxxxxxxXxxx xxxxxx xx xxx xxxxxx xx $x.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = Get-WmiObject Win32_Bios -Computer Server01
PS C:\>$a | Format-List -Property Name, @{Label="BIOS Age";Expression={(Get-Date) - $_.ConvertToDateTime($_.ReleaseDate)}}
Name     : Default System BIOS
BIOS Age : 1345.17:31:07.1091047
```

Xxxxxxx Xxxxxxxxxx Xxxxxxxxxxxxxxx $XXX$ xxxx x xxxxxxxxx xxxx$xxxx xxxxxx xxxx xxx .XXX Xxxxxxxxx xxxx$xxxx xxxxxx xxxx Xxx$Xxxx xxxxxxx.
Xx xxx xxxx$xxxx xxxxxxxxxxx xxxx XXX xx x xxxxxxx xxxx xxxx$xxxx xxxxxxxxxxx xxxx Xxx$Xxxx$ xxx xxxx xx xxx xxx XxxxxxxXxXxxxXxxx xxxxxx xx xxxxxxx XXX XXX$XXXXXXXX xxxxxxx xx .XXX Xxxxxxxxx XxxxXxxx xxxxxxx.

Xxx xxxxxxxx xx xxxx xxxxxxx xxxxxxx xxx xxxx xxx xxx xx xxx XXXX xx x xxxxxx xxxxxxxx$ Xxxxxx00.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XxxXxxxxx xxxxxx xx xxx xx xxxxxxxx xx xxx Xxx00$XXXX xxxxx xx Xxxxxx00 xxx xxxx xxxxxx xx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxxxxxx xxxxxxxx $$$ xx xxxx xxx XXX xxxxxx xxxxxx xx $x xx xxx Xxxxxx$Xxxx xxxxxx.
Xxx Xxxxxxxx xxxxxxxxx xx Xxxxxx$Xxxx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxxx xx xxx xxxx$ $Xxxx$ xxx $XXXX Xxx$.
Xxx $XXXX Xxx$ xxxxxxxx xx xxxxxxxxx xx x xxxx xxxxx.
Xxx xxxxx xxxxxxxx xxx Xxxxx xxx$ xxxxx xxxxxxxxx xxx xxxx xx xxx xxxxxxxx$ xxx xxx Xxxxxxxxxx xxx$ xxxxx xxxxxxxx xxx xxxxxxxxxx xxxx xxxxxxxxxx xxx XXXX xxx.
Xxx xxxxxxxxxx xxxx xxx XxxxxxxXxXxxxXxxx xxxxxx xx xxxxxxx xxxx xxxxxxxx xx XxxxxxxXxxx xx x .XXX Xxxxxxxxx XxxxXxxx xxxxxx.
Xxxx$ xxx xxxxx xx xxxxxxxxxx xxxx xxx xxxxx xx xxx Xxx$Xxxx xxxxxx$ xxxxx$ xxxxxxx xxxxxxxxxx$ xxxx xxx xxxxxxx xxxx.

Xxx xxxxxxxx xxxxxxxxx $$$$ xx xxx xxxx xxxxxxxxxxxx xxxxxxxxx xx Xxxxxxx XxxxxXxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Date
Tuesday, June 13, 2006 12:43:42 PM
```

Xxxx xxxxxxx xxxx x XxxxXxxx xxxxxx xxx xxxxxxxx xxx xxxxxxx xxxx xxx xxxx xx xxx xxxx xxxx xxx xxxx xxxx xxxxxxx xxx xxx xxxxxx xxxxxx$ xx xxxxxx xxx xxxxx $Xxx$Xxxx $Xxxxxx X$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Date
Tuesday, September 26, 2006 11:25:31 AM

PS C:\>(Get-Date).ToString()
9/26/2006 11:25:31 AM

PS C:\>Get-Date | Add-Content Test.txt

# Adds 9/26/2006 11:25:31 AM

PS C:\>Get-Date -Format F | Add-Content Test.txt

# Adds Tuesday, September 26, 2006 11:25:31 AM
```

Xxxxx xxxxxxxx xxxxxxxxxxx xxx xx xxx Xxx$Xxxx xxxx Xxx$Xxxxxxx xxx xxxxx xxxxxxx xxxx xxxxxxx xxx XxxxXxxx xxxxxx xxxx Xxx$Xxxx xxxxxxxxx xx x xxxxxx.

Xxx xxxxx xxxxxxx xxxxx xxxx xxx xxxxxxx xxxxxxx xxxx x $Xxx$Xxxx$ xxxxxxx xx xx xxxx$xxxx xxx xxxx$xxxx xxxxxx.

Xxx xxxxxx xxxxxxx xxxxx xxxx xxx xxxxxxx xxxxxxx xxxx xxx XxXxxxxx$$ xxxxxx xx xxx XxxxXxxx xxxxxx xx xx xxxxx$xxxx xxx xxxxx$xxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx xx xxxx xxx XxxxXxxx xxxxxx xx xxx Xxx$Xxxxxxx xxxxxx$ xxxxx xxxx xxx xxxxxxx xx xxx Xxxx.xxx xxxx.
Xxxxxxx Xxx$Xxxxxxx xxxx xxx XxXxxxxx$$ xxxxxx xx xxx XxxxXxxx xxxxxx$ xxx xxxx xxxx xx xxxxx xx xx xxxxx$xxxx xxx xxxxx$xxxx xxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx xxxxxxxxx xx Xxx$Xxxx xx xxxxxxx xxx xxxxxx.
Xxxx xxx xxx xxx Xxxxxx xx XXxxxxx xxxxxxxxxx$ Xxx$Xxxx xxxxxxxxx x xxxxxx$ xxx x XxxxXxxx xxxxxx.
Xxxx$ xxxx xxx xxxx xxx xxxxxx xx Xxx$Xxxxxxx$ xx xxxx xxx xxxxxx xx xxx Xxxx.xxx xxxx xxxxxxx xxxxxxxx xx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 00 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command uses the Format parameter with a value of "o" to generate a timestamp string.
PS C:\>Get-Date -Format o
2012-03-08T10:55:55.6083839-08:00

The second command prepares the timestamp to be used in a directory name. The command replaces the colon characters (:) in the string with dots (.) and saves the result in the $timestamp variable. Replacing the colons prevents the characters that precede each colon from being interpreted as a drive name.
PS C:\>$timestamp = Get-Date -Format o | foreach {$_ -replace ":", "."}

The third command uses the Mkdir function to create a directory with the name in the $timestamp variable.
PS C:\>mkdir C:\ps-test\$timestamp
    Directory: C:\ps-test

Mode                LastWriteTime     Length Name
----                -------------     ------ ----
d----          3/8/2012  11:01 AM            2012-03-08T11.00.24.4192623-08.00
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx Xxx$Xxxx xxxxxx xx xxxxxx x xxxxxxxxx xxx xxx xx xxx xxx xxxxxxxxx xx xx xx xxxx xx x xxxxxxxxx xxxx.

## XXXXXXXXXX

### $Xxxx
Xxxxxxxxx x xxxx xxx xxxx.
Xx xxxxxxx$ Xxx$Xxxx xxxx xxx xxxxxxx xxxxxx xxxx xxx xxxx.

Xxxx xxx xxxx xx x xxxxxx xxxx xx xxxxxxxx xxx xxx xxxxxx xxxxxx$ xxxx xx xx$XX$xxxx $Xxxxxx $$Xxxxxxx$$$ xx XX$xx$xxxx $Xxxxxxx $$Xxxxxx Xxxxxx$$$.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: LastWriteTime

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### $Xxx
Xxxxxxxxx xxx xxx xx xxx xxxxx xxxx xx xxxxxxxxx.
Xxxxx x xxxxx xxxx 0 xx 00.
Xxx xxxxxxx xx xxx xxxxxxx xxx.

Xx xxx xxxxxxx x xxxxx xxxx xx xxxxxxx xxxx xxx xxxxxx xx xxxx xx xxx xxxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxxx xx xxxx xx xxx xxxxx xxx xxxxxxxx xxx xxxxxx.
Xxx xxxxxxx$ $Xxx$Xxxx $Xxxxx 0 $Xxx 00$ xxxxxxxx $Xxxxx 0$$ xxx $Xxxxxxxx 00$.

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
Xxxxxxxxxx xxxxx xxxxxxxx xx xxx xxxx xxx xxxx xxx xxxxxxxxx.

Xxxxx xxxxxx xxx$

$$ Xxxx$ xxxxxxxx xxxx xxx xxxx $$ Xxxx$ xxxxxxxx xxxx xxx xxxx $$ XxxxXxxx$ xxxxxxxx xxx xxxx xxx xxxx

XxxxXxxx xx xxx xxxxxxx.
Xxxx xxxxxxxxx xxxx xxx xxxxxx xxx XxxxXxxx xxxxxx xxxx Xxx$Xxxx xxxx.

```yaml
Type: DisplayHintType
Parameter Sets: (All)
Aliases: 
Accepted values: Date, Time, DateTime

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxx
Xxxxxxxx xxx xxxx xxx xxxx xx xxx Xxxxxxxxx .XXX Xxxxxxxxx xxxxxx xxxxxxxxx xx xxx xxxxxx xxxxxxxxx.
Xxxxx x xxxxxx xxxxxxxxx.
Xxx x xxxx xx xxxxxxxxx xxxxxx xxxxxxxxxx$ xxx $XxxxXxxxXxxxxxXxxx Xxxxx$ xx xxx XXXX $Xxxxxxxxx Xxxxxxxxx Xxxxxxx$ xxxxxxx xx xxxx$$$xxxx.xxxxxxxxx.xxx$xxxxxxx$xxxxxx.xxxxxxxxxxxxx.xxxxxxxxxxxxxxxxxx.xxxx.

Xxxx xxx xxx xxx Xxxxxx xxxxxxxxx$ Xxxxxxx XxxxxXxxxx xxxx xxxx xxx xxxxxxxxxx xx xxx XxxxXxxx xxxxxx xxxx xx xxxxx xx xxxxxxx xxx xxxx xx xxx xxxxxx xxxx xxx xxxxxxx.
Xx x xxxxxx$ xxxx xx xxx xxxxxxxxxx xxx xxxxxxx xx XxxxXxxx xxxxxxx xxxxx xxx xx xxxxxxxxx.

Xxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ xxx xxx xxx xxx xxxxxxxxx xxxxxxxxxx xxxxxxx xx xxxxxx xxx xxx Xxxxxx xxxxxxxxx.

$$ XxxxXxxx $ X xxxx xx xxxx$xxxxxxxx xxxxxxxxxxxxxx xx xxx xxxxxxx xxxx xx xxxxx xxxx. Xx xx xx xxx xxxx xx xxxxxxxx $ xxxxx 0 xxxxxx$ 0 xxxxxx$ xxx 0 xxxxxx$. Xx xxxxxxx xx xxxxxxx xxxx xxx xxx xxxx xxxxxx xx 00000000.
$$ XxxxXxxxXxxxxxxxx $ X xxxx xx xxxx$xxxxxxxx xxxxxxxxxxxxxx xx xxx xxxxxxx xxxx xx xxxxxxxxx xxxx. Xx xx xx xxx xxxx xx xxxxxxxx $ $X$ $xxxxx 0 xxxxxx$ 0 xxxxxx$ xxx 0 xxxxxx$. Xx xxxxxxx xx xxxxxxx xxxx xxx xxx xxxx xxxxxx xx 00000000X.
$$ XxxxXxxxXxxx $ X xxxx xx xxxx$xxxxxxxx xxxxxxxxxxxxxx xx xxx xxxxxxx xxxx xxx xxxx xx xxxxx xxxx$ xx 00$xxxx xxxxxx. Xx xx xx xxx xxxx xx xxxxxxxx $ $X$ $ xxxxxxxxxx$ xxxxx xxxx xx x xxxx$xxxxxxxxx xxxxxxxxxxxxxx xx xxxxxxxxxxxx. Xx xxxxxxx xx xxxxxxx xxxx xxx xxx xxxx xxxxxx xx 00000000X0000000000.
$$ XxxxXxxxXxxxXxxxxxxxx $ X xxxx xx xxxx$xxxxxxxx xxxxxxxxxxxxxx xx xxx xxxxxxx xxxx xxx xxxx xx xxxxxxxxx xxxx$ xx 00$xxxx xxxxxx. Xx xx xx xxx xxxx xx xxxxxxxx $ $X$ $ xxxxxxxxxx$ xxxxx xxxx xx x xxxx$xxxxxxxxx xxxxxxxxxxxxxx xx xxxxxxxxxxxx$ $ $X$. Xx xxxxxxx xx xxxxxxx xxxx xxx xxx xxxx xxxxxx xx 00000000X0000000000X.

```yaml
Type: String
Parameter Sets: net
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx xxx xxxx xxxx xx xxxxxxxxx.
Xxxxx x xxxxx xxxx 0 xx 00.
Xxx xxxxxxx xx xxx xxxxxxx xxxx.

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

### $XxxxxxxxxxxXxxxxx
Xxxx xxx xxxx xx x xxxxxx xxxx xx xxxxxxxx xxx xxx xxxxxx xxxxxx$ xxxx xx xx$XX$xxxx $Xxxxxx $$Xxxxxxx$$$ xx XX$xx$xxxx $Xxxxxxx $$Xxxxxx Xxxxxx$$$.

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
Xxxx xxx xxxx xx x xxxxxx xxxx xx xxxxxxxx xxx xxx xxxxxx xxxxxx$ xxxx xx xx$XX$xxxx $Xxxxxx $$Xxxxxxx$$$ xx XX$xx$xxxx $Xxxxxxx $$Xxxxxx Xxxxxx$$$.

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

### $Xxxxxxxxxxx
Xxxxxxxxx xxx xxxxxxxxxxxx xx xxx xxxx.
Xxxxx x xxxxx xxxx 0 xx 000.
Xxx xxxxxxx xx xxx xxxxxxx xxxxxx xx xxxxxxxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

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

### $Xxxxxx
Xxxxxxxxx xxx xxxxxx xxxx xx xxxxxxxxx.
Xxxxx x xxxxx xxxx 0 xx 00.
Xxx xxxxxxx xxxxx xx xxx xxxxxxx xxxxxxx.

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

### $Xxxxx
Xxxxxxxxx xxx xxxxx xxxx xx xxxxxxxxx.
Xxxxx x xxxxx xxxx 0 xx 00.
Xxx xxxxxxx xx xxx xxxxxxx xxxxx.

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

### $Xxxxxx
Xxxxxxxxx xxx xxxxxx xxxx xx xxxxxxxxx.
Xxxxx x xxxxx xxxx 0 xx 00.
Xxx xxxxxxx xx xxx xxxxxxx xxxxxx.

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

### $XXxxxxx
Xxxxxxxx xxx xxxx xxx xxxx xx XXXX xxxxxx.
Xxx x xxxx xx xxx xxxxxx xxxxxxxxxx$ xxx xxx Xxxxx xxxxxxx.

Xxxx xxx xxx xxx XXxxxxx xxxxxxxxx$ Xxxxxxx XxxxxXxxxx xxxx xxxx xxx xxxxxxxxxx xx xxx XxxxXxxx xxxxxx xxxx xx xxxxx xx xxxxxxx xxx xxxx xx xxx xxxxxx xxxx xxx xxxxxxx.
Xx x xxxxxx$ xxxx xx xxx xxxxxxxxxx xxx xxxxxxx xx XxxxXxxx xxxxxxx xxxxx xxx xx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UFormat
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx xxx xxxx xxxx xx xxxxxxxxx.
Xxxxx x xxxxx xxxx 0 xx 0000.
Xxx xxxxxxx xx xxx xxxxxxx xxxx.

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

## XXXXXX

### Xxxx
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### Xxxxxx.XxxxXxxx xx Xxxxxx.Xxxxxx
Xxxx xxx xxx xxx Xxxxxx xx XXxxxxx xxxxxxxxxx$ Xxx$Xxxx xxxxxxx x xxxxxx.
Xxxxxxxxx$ xx xxxxxxx x XxxxXxxx xxxxxx.

## XXXXX
Xx xxxxxxx$ xxx xxxx$xxxx xx xxxxxxxxx xx xxxx$xxxx xxx xxxx$xxxx xxxxxxx xxx xxx xxxxxx xxxxxx.

Xxxx xxx xxxx x xxxx xx xxxxxxx xxxx xxxxxx xxxxxx xxxxx$ xxxx xx xxx Xxx$Xxxxxxx xxxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxxx xxx XxxxXxxx xxxxxx xx x xxxxxx xxxxxx xxxxxx xx xx xxx xxxx.
Xxx xxxxxxx XxXxxxxx$$ xxxxxx xx xxxxx xxxx xxx xxxx xxxx.
Xx xxxxxxx xx xxxxxxxxx xxxxxx$ xxx xxx Xxxxxx xx XXxxxxx xxxxxxxxxx xx Xxx$Xxxx.

Xxxxxxx Xxxxxx$

Xxx xxxxxxxxx xxx xxx xxxxxx xx xxx XXxxxxx xxxxxxxxx.
Xxx xxxxxx xxx xxx xxxxxxx xx$

Xxx$Xxxx $XXxxxxx $$$xxxxx\>

Xxx xxxxxxx$

Xxx$Xxxx $XXxxxxx $x

Xxxx$Xxxx$

Xxxx xxx xxxx $ xxxx

$xxxxxxx$ $Xxxxxx$ Xxxx 00$ 0000 00$00$00 XX$

x     Xxxx xxx xxxx $ xxxxxxxxxxx $Xxx Xxx 00 00$00$00 0000$

Xxxx$

X    Xxxx xx xx$xx$xx xxxxxx $00$00$00$

x    Xxxx xx xxxxxxxx xxxxxx xxx xxxxxx $00$00$00 xxx Xxxxxxx$XX$

Xxxx$

X   Xxxxxxx $00 xxx 0000$

X   Xxxx xx 0$xxxxx xxxxxx $0000$

x   Xxxx xx 0$xxxxx xxxxxx $00$

X   Xxxx xx $X$

x   Xxxx xx $x$

Xxxxx$

x   Xxxxx xxxx $ xxxxxxxxxxx $Xxx$

X   Xxxxx xxxx $ xxxx $Xxxxxxx$

x   Xxxx xx $x$

x   Xxxxx xxxxxx $00$

Xxxx$

X  Xxxx xx xxx xxxx $00$00$

X   Xxxx xx xxx xxxx $00$00$

X   Xxxx xx $X$

Xxx$

x   Xxx xx xxx xxxx $ xxxxxxxxxxx xxxx $Xxx$

X   Xxx xx xxx xxxx $ xxxx xxxx $Xxxxxx$

x   Xxx xx xxx xxxx $ xxxxxx $Xxxxxx $ 0$

x   Xxx xx xxx xxxxx $ 0 xxxxxx $00$

x   Xxx xx xxx xxxxx $ xxxxx xxxxxxxx xx x xxxxx $ 0$

x    Xxx xx xxx xxxx $ $0$000$

x   Xxxx xx $x$

Xxxx$

x   XX xx XX

x   Xxxx xx 00$xxxx xxxxxx $00$00$00 XX$

X   Xxxx xx 00$xxxx xxxxxx $ xx xxxxxxx $00$00$

X   Xxxx xx 00 xxxx xxxxxx $00$00$00$

X   Xxxx xx $X$

X   Xxxx xxxx xxxxxx xxxx Xxxxxxxxx Xxxx Xxxxxxxxxx $XXX$ $$00$

Xxxx$

X   Xxxx xx 00$xxxx xxxxxx $00$

X    Xxxx xx 00 xxxx xxxxxx $00$

x   Xxxx xx $X$

x    Xxxx xx $X$ $Xxxxx$xxxx X $ Xxxxx$xxxx X$

Xxxxxxx $ Xxxxxxx$

X   Xxxxxxx $00$

X   Xxxxxxx $00$

x   Xxxxxxx xxxxxxx xxxxx Xxxxxxx 0$ 0000 00$00$00 $0000000000.00000$

Xxxxxxx Xxxxxxxxxx$

x   xxxxxxx xxxxxxxxx $$x$

x   Xxx xxxxxxxxx $$x$

## XXXXXXX XXXXX

[Xxx$XxxxXxxx]()

[Xxx$Xxxx]()

