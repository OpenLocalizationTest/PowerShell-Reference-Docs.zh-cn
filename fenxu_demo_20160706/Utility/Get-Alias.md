---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293964
schema: 2.0.0
---

# Get-Alias
## XXXXXXXX
Xxxx xxx xxxxxxx xxx xxx xxxxxxx xxxxxxx.

## XXXXXX

### Default (Default)
```
Get-Alias [[-Name] <String[]>] [-Exclude <String[]>] [-Scope <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### Definition
```
Get-Alias [-Exclude <String[]>] [-Scope <String>] [-Definition <String[]>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxx xxxxxx xxxx xxx xxxxxxx $xxxxxxxxx xxxxx xxx xxxxxxxx xxx xxxxxxxxxx xxxxx$ xx xxx xxxxxxx xxxxxxx.
Xxxx xxxxxxxx xxxxx$xx xxxxxxx$ xxxxxxx xxxx xxx xxxx xxx xx xxxxxxxx$ xxx xxxxxxx xxxx xxx xxxx xxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.

Xx xxxxxxx$ Xxx$Xxxxx xxxxx xx xxxxx xxx xxxxxxx xxx xxxxxxx xxxx.
Xxxx xxx xxx xxx Xxxxxxxxxx xxxxxxxxx$ Xxx$Xxxxx xxxxx x xxxxxxx xxxx xxx xxxxxxx xxx xxxxxxx.

Xxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ Xxx$Xxxxx xxxxxxxx xxx$xxxxxxxxxx xxxxx xxxxx xx xx $$$xxxxx$$ $$$ $$xxxxxxxxxx$$$ xxxxxx xx xxxx xx xxxx xxxxxx xx xxxx xxx xxxxxxxxxxx xxxx xxx xxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Alias
CommandType     Name

-----------     ----

Alias           % -> ForEach-Object

Alias           ? -> Where-Object

Alias           ac -> Add-Content

Alias           asnp -> Add-PSSnapin

Alias           cat -> Get-Content

Alias           cd -> Set-Location

Alias           chdir -> Set-Location

Alias           clc -> Clear-Content

Alias           clear -> Clear-Host

Alias           clhy -> Clear-History …
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xx xxx xxxxxxx xxxxxxx.

Xxx xxxxxx xxxxx xxx $$$xxxxx$$ $$$ $$xxxxxxxxxx$$$ xxxxxx xxxx xxx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0. Xxxx xxxxxx xx xxxx xxxx xxx xxxxxxx xxxx xx xxx xxxxxxx xxxxxxx$ xxxxxxx xxxxxxx xxxx xxxxxxx xxx xxxxxxxxx xxxxxxxxx xxxxx xxx xxxxxxx xxx xxxxxxxxx$ xxxxxx xxxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Alias -Name g*, s* -Exclude Get-*
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xxxx xxxxx xxxx $x$ xx $x$$ xxxxxx xxx xxxxxxx xxxx xxxxx xxxx $xxx$$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Alias -Definition Get-ChildItem
```

Xxxx xxxxxxx xxxx xxx xxxxxxx xxx xxx Xxx$XxxxxXxxx xxxxxx.

Xx xxxxxxx$ xxx Xxx$Xxxxx xxxxxx xxxx xxx xxxx xxxx xxxx xxx xxxx xxx xxxxx.
Xxx Xxxxxxxxxx xxxxxxxxx xxxx xxx xxxxx xxxx xxx xxxx xxx xxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Alias | Where-Object {$_.Options -Match "ReadOnly"}
```

Xxxx xxxxxxx xxxxxxxxx xxx xxxxxxx xx xxxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx XxxxXxxx.
Xxxx xxxxxxx xxxxxxxx x xxxxx xxx xx xxxx xxx xxxxxxx xxxx xxx xxxxx xxxx Xxxxxxx XxxxxXxxxx$ xxxxxxx xxxx xxxx xxx XxxxXxxx xxxxxx.

Xxxxxxx xx xxxx xxx xxxxxxxx xx xxx XxxxxXxxx xxxxxxx xxxx Xxx$Xxxxx xxxx.
Xx xxxx xxx xxxxxxxxxx xxx xxxxxxx xx XxxxxXxxx xxxxxxx$ xxxx $Xxx$Xxxxx $ xxx$xxxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Alias -Definition "*-PSSession" -Exclude e* -Scope Global
```

Xxxx xxxxxxx xxxx xxxxxxx xxx xxxxxxxx xxxx xxxx xxxxx xxxx xxx xx $$XXXxxxxxx$$ xxxxxx xxx xxxxx xxxx xxxxx xxxx $x$.

Xxx xxxxxxx xxxx xxx Xxxxx xxxxxxxxx xx xxxxx xxx xxxxxxx xx xxx xxxxxx xxxxx.
Xxxx xx xxxxxx xx xxxxxxx xxxx xxx xxxx xx xxx xxx xxxxxxx xx xxx xxxxxxx.

## XXXXXXXXXX

### -Definition
Xxxx xxx xxxxxxx xxx xxx xxxxxxxxx xxxx.
Xxxxx xxx xxxx xx x xxxxxx$ xxxxxxxx$ xxxxxx$ xxxx$ xx xxxxxxxxxx xxxx.

Xxxx xxxxxxxxx xx xxxxxx Xxxxxxxxxx$ xxxxxxx xx xxxxxxxx xxx xxx xxxx xxxx xx xxx Xxxxxxxxxx xxxxxxxx xx xxx xxxxx xxxxxx.

```yaml
Type: String[]
Parameter Sets: Definition
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Exclude
Xxxxx xxx xxxxxxxxx xxxxx.
Xxx xxxxx xx xxxx xxxxxxxxx xxxxxxxxx xxx Xxxx xxx Xxxxxxxxxx xxxxxxxxxx.
Xxxxx x xxxx$ x xxxxxxxxxx$ xx x xxxxxxx$ xxxx xx $x$$.
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
Xxxx xxxxxxxxx xx xxxxxx Xxxxxxxxxx$ xxxxxxx xx xxxxxxxx xxx xxx xxxx xxxx xx xxx Xxxxxxxxxx xxxxxxxx xx xxx xxxxx xxxxxx.

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
Xxxx xxxxxxxxx xx xxxxxx Xxxxxxxxxx$ xxxxxxx xx xxxxxxxx xxx xxx xxxx xxxx xx xxx Xxxxxxxxxx xxxxxxxx xx xxx xxxxx xxxxxx.

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
Xxxxxxxxx xxx xxxxxxx xx xxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.
Xx xxxxxxx$ Xxx$Xxxxx xxxxxxxxx xxx xxxxxxx xxxxxxx xxx xxx xxxxxxx xxxxxxx.
Xxx xxxxxxxxx xxxx $$Xxxx$$ xx xxxxxxxx.
Xxx xxx xxxx xxxx xxxxx xxxxx xx Xxx$Xxxxx.

```yaml
Type: String[]
Parameter Sets: Default
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Scope
Xxxx xxxx xxx xxxxxxx xx xxx xxxxxxxxx xxxxx.
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

## XXXXXX

### System.String
Xxx xxx xxxx xxxxx xxxxx xx Xxx$Xxxxx.

## XXXXXXX

### System.Management.Automation.AliasInfo
Xxx$Xxxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxxx xxxxx.
Xxx$Xxxxx xxxxxxx xxx xxxx xxxxxx xxx xxxxx xxxxx$ xxx Xxxxxxx XxxxxXxxxx xxxx xx xxxxx$xxxxx xxxxxx xx xxxxxxx xxx xxxxx xx xxx$xxxxxxxxxx xxxxxxx.

## XXXXX
Xx xxxxxx x xxx xxxxx$ xxx Xxx$Xxxxx xx Xxx$Xxxxx.
Xx xxxxxx xx xxxxx$ xxx Xxxxxx$Xxxx.

Xxx xxxxx$xxxxx xxxxx xxxx xxxxxx xx xxx xxxx xxx xxxxxxx xxxx xxxxxxx x xxxxxx.
Xxxxx xxx xxxxxx xx xx xxxxxxxxx xxxxxxxxxx xxxxx xxx xxxxxxx xxx xxxxxxxxx$ xxxxxxx xx xxxxxxx xxxxxxxxxxxxx xx xxxxxxxxx.

## XXXXXXX XXXXX

[Export-Alias]()

[Import-Alias]()

[New-Alias]()

[Set-Alias]()

[Alias Provider]()

[about_Aliases]()

