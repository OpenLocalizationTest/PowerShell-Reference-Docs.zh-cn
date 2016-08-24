---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293974
schema: 2.0.0
---

# Xxx$Xxxxxx
## XXXXXXXX
Xxxx x xxxxxx xxxxxx$ xx xxxxxxx xxxxxxx xxxxxxxx xxxx x xxxxxxxxxx.

## XXXXXX

### XxxxxxXxxxxxXxxxxxxxxXxx $Xxxxxxx$
```
Get-Random [-SetSeed <Int32>] [[-Maximum] <Object>] [-Minimum <Object>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### XxxxxxXxxxXxxxXxxxxxxxxXxx
```
Get-Random [-SetSeed <Int32>] [-InputObject] <Object[]> [-Count <Int32>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxx xxxxxx xxxx x xxxxxxxx xxxxxxxx xxxxxx.
Xx xxx xxxxxx x xxxxxxxxxx xx xxxxxxx xx Xxx$Xxxxxx$ xx xxxx xxx xx xxxx xxxxxxxx xxxxxxxx xxxxxxx xxxx xxx xxxxxxxxxx.

Xxxxxxx xxxxxxxxxx xx xxxxx$ x Xxx$Xxxxxx xxxxxxx xxxxxxx x xxxxxxxx xxxxxxxx 00$xxx xxxxxxxx xxxxxxx xxxxxxx 0 $xxxx$ xxx Xxx00.XxxXxxxx $0x0XXXXXXX$ 0$000$000$000$.

Xxx xxx xxx xxx xxxxxxxxxx xx Xxx$Xxxxxx xx xxxxxxx x xxxx xxxxxx$ xxxxxxx xxx xxxxxxx xxxxxx$ xxx xxx xxxxxx xx xxxxxxx xxxxxxxx xxxx x xxxxxxxxx xxxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Random
3951433
```

Xxxx xxxxxxx xxxx x xxxxxx xxxxxxx xxxxxxx 0 $xxxx$ xxx Xxx00.XxxXxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Random -Maximum 100
47
```

Xxxx xxxxxxx xxxx x xxxxxx xxxxxxx xxxxxxx 0 $xxxx$ xxx 00.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Random -Minimum -100 -Maximum 100
56
```

Xxxx xxxxxxx xxxx x xxxxxx xxxxxxx xxxxxxx $000 xxx 00.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Random -Minimum 10.7 -Maximum 20.93
18.08467273887
```

Xxxx xxxxxxx xxxx x xxxxxx xxxxxxxx$xxxxx xxxxxx xxxxxxx xxxx xx xxxxx xx 00.0 xxx xxxx xxxx 00.00.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Random -InputObject 1, 2, 3, 5, 8, 13
8
```

Xxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx xxxxxx xxxx xxx xxxxxxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Random -InputObject 1, 2, 3, 5, 8, 13 -Count 3
3
1
13
```

Xxxx xxxxxxx xxxx xxxxx xxxxxxxx xxxxxxxx xxxxxxx xx xxxxxx xxxxx xxxx xxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Random -InputObject 1, 2, 3, 5, 8, 13 -Count ([int]::MaxValue)
2
3
5
1
8
13
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxx xxxxxxxxxx xx xxxxxx xxxxx.
Xxx xxxxx xx xxx Xxxxx xxxxxxxxx xx xxx XxxXxxxx xxxxxx xxxxxxxx xx xxxxxxxx.

Xx xxxxxx xx xxxxxx xxxxxxxxxx xx xxxxxx xxxxx$ xxxxx xxx xxxxxx xxxx xx xxxxxxx xxxx xx xxxxx xx xxx xxxxxx xx xxxxxxx xx xxx xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Random -InputObject "red", "yellow", "blue"
yellow
```

Xxxx xxxxxxx xxxxxxx x xxxxxx xxxxx xxxx x xxx$xxxxxxx xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | Get-Random

Handles  NPM(K)    PM(K)      WS(K) VM(M)   CPU(s)     Id ProcessName
-------  ------    -----      ----- -----   ------     -- -----------
144           4     2080        488    36     0.48   3164 wmiprvse
```

Xxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx xxxxxxx xxxx xxx xxxxxxxxxx xx xxxxxxxxx xx xxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 00 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Content Servers.txt | Get-Random -Count (Get-Content Servers.txt).Count | foreach {Invoke-Command -ComputerName $_ -Command 'Get-Process PowerShell'}
```

Xxxx xxxxxxx xxxx x xxxxxxx xx x xxxxxx xx xxxxxx xxxxxxxxx xx xxxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 00 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Random -Maximum 100 -SetSeed 23

# Commands with the default seed are pseudorandom

PS C:\>Get-Random -Maximum 100
59
PS C:\>Get-Random -Maximum 100
65
PS C:\>Get-Random -Maximum 100
21

# Commands with the same seed are not random

PS C:\>Get-Random -Maximum 100 -SetSeed 23
74
PS C:\>Get-Random -Maximum 100 -SetSeed 23
74
PS C:\>Get-Random -Maximum 100 -SetSeed 23
74

# SetSeed results in a repeatable series

PS C:\>Get-Random -Maximum 100 -SetSeed 23
74
PS C:\>Get-Random -Maximum 100
56
PS C:\>Get-Random -Maximum 100
84
PS C:\>Get-Random -Maximum 100
46
PS C:\>Get-Random -Maximum 100 -SetSeed 23
74
PS C:\>Get-Random -Maximum 100
56
PS C:\>Get-Random -Maximum 100
84
PS C:\>Get-Random -Maximum 100
46
```

Xxxx xxxxxxx xxxxx xxx xxxxxx xx xxxxx xxx XxxXxxx xxxxxxxxx.
Xxxxxxx XxxXxxx xxxxxxxx xxx$xxxxxx xxxxxxxx$ xx xx xxxxxxxxx xxxx xxxx xx xxxxxxxxx xxxxxxx$ xxxx xx xxxx xxxxxxxxx xx xxxxxxxxx x xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 00 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$files = dir -Path C:\* -Recurse
PS C:\>$sample = $files | Get-Random -Count 50
```

Xxxxx xxxxxxxx xxx x xxxxxxxx xxxxxxxx xxxxxx xx 00 xxxxx xxxx xxx X$ xxxxx xx xxx xxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 00 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Random 10001
7600
```

Xxxx xxxxxxx xxxx x xxxxxx xxxxxxx xxxx xxxx 00000.
Xxxxxxx xxx Xxxxxxx xxxxxxxxx xxx xxxxxxxx 0$ xxx xxx xxxx xxx xxxxxxxxx xxxx xxxx xxx xxxxx xx xxx xxxxx xx xxxx xxxxxxx xxxxxxxxx xx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 00 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Random -Minimum ([Int64]::MinValue)3738173363251507200
PS C:\>Get-Random -Minimum ([Int32]::MaxValue)

Minimum (2147483647) cannot be greater than or equal to Maximum (2147483647).
    + CategoryInfo          : InvalidArgument: (:) [Get-Random], ArgumentException
    + FullyQualifiedErrorId : MinGreaterThanOrEqualMax,Microsoft.PowerShell.Commands.GetRandomCommand
```

Xxxxx xxxxxxxx xxxxxxx xx xxx xxxxxxxx xxxxxxxxx 00$xxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxxx$ xxx xxx xxxxxx xxxxxxx xxxxx.
Xxxx xxx xxxxx xx Xxxxxxx xx x 00$xxx xxxxxxx$ xxx xxxxxxx xxxxx xx Xxxxxxx xx Xxx00.XxxXxxxxx.
Xxx xxxxxxx xxxxx xxxxxxx xxx xxxxx xx Xxxxxxx xxxx xx xxxxxxx xxxx xxx xxxxx xx Xxxxxxx.

## XXXXXXXXXX

### $Xxxxx
Xxxxxxxxxx xxx xxxx xxxxxxx xxx xxxxxxxx.
Xxx xxxxxxx xx 0.
Xx xxx xxxxx xx Xxxxx xxxxxxx xxx xxxxxx xx xxxxxxx xx xxx xxxxxxxxxx$ Xxx$Xxxxxx xxxxxxx xxx xx xxx xxxxxxx xx xxxxxx xxxxx.

```yaml
Type: Int32
Parameter Sets: RandomListItemParameterSet
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
Xxxxxxxxx x xxxxxxxxxx xx xxxxxxx.
Xxx$Xxxxxx xxxx xxxxxxxx xxxxxxxx xxxxxxx xx xxxxxx xxxxx xxxx xxx xxxxxxxxxx.
Xxxxx xxx xxxxxxx$ x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx$ xx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.
Xxx xxx xxxx xxxx x xxxxxxxxxx xx xxxxxxx xx Xxx$Xxxxxx.

```yaml
Type: Object[]
Parameter Sets: RandomListItemParameterSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $Xxxxxxx
Xxxxxxxxx x xxxxxxx xxxxx xxx xxx xxxxxx xxxxxx.
Xxx$Xxxxxx xxxxxxx x xxxxx xxxx xx xxxx xxxx xxx xxxxxxx $xxx xxxxx$.
Xxxxx x 00$xxx xxxxxxx xx x xxxxxx$xxxxxxxxx xxxxxxxx$xxxxx xxxxxx$ xx xx xxxxxx xxxx xxx xx xxxxxxxxx xx xx xxxxxxx xx xxxxxx$ xxxx xx x xxxxxxx xxxxxx $$000$$.
Xx x 00$xxx xxxxxxxx$ xxx xxx xxxx xxxxx x 00$xxx xxxxxxx.

Xxx xxxxx xx Xxxxxxx xxxx xx xxxxxxx xxxx $xxx xxxxx xx$ xxx xxxxx xx Xxxxxxx.

Xx xxx xxxxx xx Xxxxxxx xx Xxxxxxx xx x xxxxxxxx$xxxxx xxxxxx$ Xxx$Xxxxxx xxxxxxx x xxxxxxxx xxxxxxxx xxxxxxxx$xxxxx xxxxxx.
Xx xxx xxxxx xx Xxxxxxx xx x xxxxxx $x xxxxxxxx$xxxxx xxxxxx$$ xxx xxxxxxx xxxxx xx Xxxxxxx xx Xxxxxx.XxxXxxxx.
Xxxxxxxxx$ xxx xxxxxxx xxxxx xx Xxx00.XxxXxxxx.

Xx x 00$xxx xxxxxxxx$ xx xxx xxxxx xx Xxxxxxx xx x 00$xxx xxxxxxx$ xxx  xxxxxxx xxxxx xx Xxxxxxx xx Xxx00.XxxXxxxx.
Xx xxx xxxxx xx Xxxxxxx xx x xxxxxx $x xxxxxxxx$xxxxx xxxxxx$$ xxx xxxxxxx xxxxx xx Xxxxxxx xx Xxxxxx.XxxXxxxx.
Xxxxxxxxx$ xxx xxxxxxx xxxxx xx Xxx00.XxxXxxxx.

```yaml
Type: Object
Parameter Sets: RandomNumberParameterSet
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxx
Xxxxxxxxx x xxxxxxx xxxxx xxx xxx xxxxxx xxxxxx.
Xxxxx x 00$xxx xxxxxxx xx x xxxxxx$xxxxxxxxx xxxxxxxx$xxxxx xxxxxx$ xx xx xxxxxx xxxx xxx xx xxxxxxxxx xx xx xxxxxxx xx xxxxxx$ xxxx xx x xxxxxxx xxxxxx $$000$$.
Xx x 00$xxx xxxxxxxx$ xxx xxx xxxxx x 00$xxx xxxxxxx.
Xxx xxxxxxx xxxxx xx 0 $xxxx$.

Xxx xxxxx xx Xxxxxxx xxxx xx xxxx xxxx $xxx xxxxx xx$ xxx xxxxx xx Xxxxxxx.
Xx xxx xxxxx xx Xxxxxxx xx Xxxxxxx xx x xxxxxxxx$xxxxx xxxxxx$ Xxx$Xxxxxx xxxxxxx x xxxxxxxx xxxxxxxx xxxxxxxx$xxxxx xxxxxx.

```yaml
Type: Object
Parameter Sets: RandomNumberParameterSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxxx
Xxxxxxxxx x xxxx xxxxx xxx xxx xxxxxx xxxxxx xxxxxxxxx.
Xxxx xxxx xxxxx xx xxxx xxx xxx xxxxxxx xxxxxxx xxx xxx xxx xxxxxxxxxx Xxx$Xxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxx xxxxx xxx xxx XxxXxxx xxxxx xx xxxxx xxx xxxxxxx.
Xxx xxxxxx xxxxx xxx xxxx xx xxx xxxxxxx$ xxxxx$xxxxx xxxxx.

Xxx XxxXxxx xxxxxxxxx xx xxx xxxxxxxx.
Xx xxxxxxx$ Xxx$Xxxxxx xxxx xxx xxxxxx xxxxx xx xxxxxxxx x xxxx xxxxx.
Xxxxxxx XxxXxxx xxxxxxx xx xxx$xxxxxx xxxxxxxx$ xx xx xxxxxxxxx xxxx xxxx xxxx xxxxxx xx xxxxxxxxx xxxxxxxx$ xxxx xx xxxx xxxxxxxxx xx xxxxxxxxx x xxxxxx xxxx xxxxxxxx Xxx$Xxxxxx xxxxxxxx.

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

### Xxxxxx.Xxxxxx
Xxx xxx xxxx xxx xx xxxx xxxxxxx xx Xxx$Xxxxxx.
Xxx$Xxxxxx xxxxxxx xxxxxx xxxxxxxx xxxx xxx xxxxx xxxxxxx.

## XXXXXXX

### Xxxxxx.Xxx00$ Xxxxxx.Xxx00$ Xxxxxx.Xxxxxx
Xxx$Xxxxxx xxxxxxx xx xxxxxxx xx xxxxxxxx$xxxxx xxxxxx$ xx xx xxxxxx xxxxxxxx xxxxxxxx xxxx x xxxxxxxxx xxxxxxxxxx.

## XXXXX
Xxx$Xxxxxx xxxx x xxxxxxx xxxx xxx xxxx xxxxxxx xxxxx xx xxx xxxxxx xxxx xxxxx xxxx xxx xxxxxxx xxxxxx.

Xxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ Xxx$Xxxxxx xxxxxxxx 00$xxx xxxxxxxx.
Xx Xxxxxxx XxxxxXxxxx 0.0$ xxx xxxxxx xxx xxxx xx Xxxxxx.Xxx00.

## XXXXXXX XXXXX

