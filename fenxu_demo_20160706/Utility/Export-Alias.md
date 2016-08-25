---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293955
schema: 2.0.0
---

# Export-Alias
## XXXXXXXX
Xxxxxxx xxxxxxxxxxx xxxxx xxxxxxxxx xxxxxxx xxxxxxx xx x xxxx.

## XXXXXX

### ByPath (Default)
```
Export-Alias [-Path] <String> [[-Name] <String[]>] [-PassThru] [-As <ExportAliasFormat>] [-Append] [-Force]
 [-NoClobber] [-Description <String>] [-Scope <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### ByLiteralPath
```
Export-Alias -LiteralPath <String> [[-Name] <String[]>] [-PassThru] [-As <ExportAliasFormat>] [-Append]
 [-Force] [-NoClobber] [-Description <String>] [-Scope <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxxxx xxxxxx xxxxxxx xxx xxxxxxx xx xxx xxxxxxx xxxxxxx xx x xxxx. Xx xxx xxxxxx xxxx xxxx xxx xxxxx$ xxx xxxxxx xxxx xxxxxx xx.

Xxxxxx$Xxxxx xxx xxxxxx xxx xxxxxxx xx x xxxxxxxxxx xxxxx xx xxx xxxxxx$ xx xxx xxxxxxxx xxx xxxx xx XXX xxxxxx xx xx x xxxxxx xx Xxx$Xxxxx xxxxxxxx xxxx xxx xxx xxx xx x xxxxxxx xx xx x Xxxxxxx XxxxxXxxxx xxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>export-alias -path alias.csv
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxxxxx xxxxxxx xxxxx xxxxxxxxxxx xx x xxxx xxxxx Xxxxx.xxx xx xxx xxxxxxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>export-alias -path alias.csv -noclobber
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxxxxx xxx xxxxxxx xx xxx xxxxxxx xxxxxxx xx xx Xxxxx.xxx xxxx.

Xxxxxxx xxx XxXxxxxxx xxxxxxxxx xx xxxxxxxxx$ xxx xxxxxxx xxxx xxxx xx xx Xxxxx.xxx xxxx xxxxxxx xxxxxx xx xxx xxxxxxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>export-alias -path alias.csv -append -description "Appended Aliases" -force
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxxxxx xxx xxxxxxx xx xxx xxxxxxx xxxxxxx xx xxx Xxxxx.xxx xxxx.

Xxx xxxxxxx xxxx xxx Xxxxxxxxxxx xxxxxxxxx xx xxx x xxxxxxxxxxx xx xxx xxxxxxxx xx xxx xxx xx xxx xxxx.

Xxx xxxxxxx xxxx xxxx xxx Xxxxx xxxxxxxxx xx xxxxxxxxx xxx xxxxxxxx Xxxxx.xxx xxxxx$ xxxx xx xxxx xxxx xxx xxxx$xxxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>export-alias -path alias.ps1 -as script
PS C:\> add-content -path $profile -value (get-content alias.ps1)
PS C:\> $s = new-pssession -computername Server01
PS C:\> invoke-command -session $s -filepath .\alias.ps1
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxxx xxx xx xxx xxx xxxxxx xxxx xxxxxx xxxx Xxxxxx$Xxxxx xxxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx xxx xxxxxxx xx xxx xxxxxxx xx xxx Xxxxx.xx0 xxxx.
Xx xxxx xxx Xx xxxxxxxxx xxxx x xxxxx xx Xxxxxx xx xxxxxxxx x xxxx xxxx xxxxxxxx x Xxx$Xxxxx xxxxxxx xxx xxxx xxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxxxxx xx xxx Xxxxx.xx0 xxxx xx xxx XxxxxxxXxxx$XxxxxxxXxxx xxxxxxx.
$Xxx xxxx xx xxx xxxxxxx xx xxxxx xx xxx $xxxxxxx xxxxxxxx.$ Xxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxx xxxx xxx Xxxxx.xx0 xxxx xxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxxx xx xxx xxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxx.

Xxx xxxxx xxx xxxxxx xxxxxxxx xxx xxx xxxxxxx xx xxx Xxxxx.xx0 xxxx xx x  xxxxxx xxxxxxx xx xxx Xxxxxx00 xxxxxxxx.
Xxx xxxxx xxxxxxx xxxx xxx Xxx$XXXxxxxxx xxxxxx xx xxxxxx xxx xxxxxxx.
Xxx xxxxxx xxxxxxx xxxx xxx XxxxXxxx xxxxxxxxx xx xxx Xxxxxx$Xxxxxxx xxxxxx xx xxx xxx Xxxxx.xx0 xxxx xx xxx xxx xxxxxxx.

## XXXXXXXXXX

### -Append
Xxxxxxx xxx xxxxxx xx xxx xxxxxxxxx xxxx$ xxxxxx xxxx xxxxxxxxxxx xxx xxxxxxxx xxxxxxxx xx xxxx xxxx.

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

### -As
Xxxxxxxxxx xxx xxxxxx xxxxxx.
XXX xx xxx xxxxxxx.

Xxxxx xxxxxx xxx$

$$ XXX$ Xxxxx$xxxxxxxxx xxxxx $XXX$ xxxxxx.
$$ Xxxxxx$ Xxxxxxx x Xxx$Xxxxx xxxxxxx xxx xxxx xxxxxxxx xxxxx. Xx xxx xxxx xxx xxxxxx xxxx xxxx x .xx0 xxxx xxxx xxxxxxxxx$ xxx xxx xxx xx xx x xxxxxx xx xxx xxx xxxxxxx xx xxx xxxxxxx.

```yaml
Type: ExportAliasFormat
Parameter Sets: (All)
Aliases: 
Accepted values: Csv, Script

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
Xxxx x xxxxxxxxxxx xx xxx xxxxxxxx xxxx.
Xxx xxxxxxxxxxx xxxxxxx xx x xxxxxxx xx xxx xxx xx xxx xxxx$ xxxxxxxxx xxx xxxxxx xxxxxxxxxxx.

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

### -Force
Xxxxxxxxxx xxx xxxxxx xxxx$ xxxx xx xxx xxxx$xxxx xxxxxxxxx xx xxx xx xxx xxxx.

Xx xxxxxxx$ Xxxxxx$Xxxxx xxxxxxxxxx xxxxx xxxxxxx xxxxxxx$ xxxxxx xxx xxxx$xxxx xx xxxxxx xxxxxxxxx xx xxx xx xxx XxXxxxxxx xxxxxxxxx xx xxxx xx xxx xxxxxxx.
Xxx XxXxxxxxx xxxxxxxxx xxxxx xxxxxxxxxx xxxx xxx Xxxxx xxxxxxxxx xxxx xxxx xxx xxxx xx x xxxxxxx.

Xxx Xxxxx xxxxxxxxx xxxxxx xxxxx Xxxxxx$Xxxxx xx xxxxxxxxx xxxxx xxxx xxx xxxxxx xxxxxxxxx.

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

### -LiteralPath
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxx.
Xxxxxx Xxxx$ xxx xxxxx xx xxx XxxxxxxXxxx xxxxxxxxx xx xxxx xxxxxxx xx xx xx xxxxx.
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

### -Name
Xxxxxxxxx xxx xxxxx xx xxx xxxxxxx xx xxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

Xx xxxxxxx$ Xxxxxx$Xxxxx xxxxxxx xxx xxxxxxx xx xxx xxxxxxx xx xxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -NoClobber
Xxxxxxxx Xxxxxx$Xxxxx xxxx xxxxxxxxxxx xxx xxxxx$ xxxx xx xxx Xxxxx xxxxxxxxx xx xxxx xx xxx xxxxxxx.

Xx xxx XxXxxxxxx xxxxxxxxx xx xxxxxxx$ Xxxxxx$Xxxxx xxxx xxxxxxxxx xx xxxxxxxx xxxx xxxxxxx xxxxxxx$ xxxxxx xxx xxxx$xxxx xxxxxxxxx xx xxx xx xxx xxxx.
XxXxxxxxx xxxxx xxxxxxxxxx xxxx xxx Xxxxx xxxxxxxxx$ xxxxx xxxxxxx Xxxxxx$Xxxxx xx xxxxxxxxx x xxxx xxxx xxx xxxx$xxxx xxxxxxxxx.

XxXxxxxxx xxxx xxx xxxxxxx xxx Xxxxxx xxxxxxxxx xxxx xxxxxx xxxxxxx xx xx xxxxxxxx xxxx.

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

### -PassThru
Xxxxxxx xxxxxxx xxxx xxxxxxxxx xxx xxxxxxx xxxx xxxx xxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

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

### -Path
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxx.
Xxxxxxxxx xxx xxxxxxxxx$ xxx xxx xxxxxxxxx xxxx xxxxx xxxx xxxxxxx xx x xxxxxx xxxx xxxx.
Xxxx xxxxxxxxx xx xxxxxxxx.

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

### -Scope
Xxxxxxxxx xxx xxxxx xxxx xxxxx xxx xxxxxxx xxxxxx xx xxxxxxxx.

Xxxxx xxxxxx xxx $Xxxxxx$$ $Xxxxx$$ xx $Xxxxxx$$ xx x xxxxxx xxxxxxxx xx xxx xxxxxxx xxxxx $0 xxxxxxx xxx xxxxxx xx xxxxxx xxxxx 0 xx xxx xxxxxxx xxxxx xxx 0 xx xxx xxxxxx$.
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

### -Confirm
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

### -WhatIf
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

## XXXXXX

### None.
Xxx xxxxxx xxxx xxxxxxx xx xxxx xxxxxx.

## XXXXXXX

### None or System.Management.Automation.AliasInfo
Xxxx xxx xxx xxx Xxxxxxxx xxxxxxxxx$ Xxxxxx$Xxxxx xxxxxxx x Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XxxxxXxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxx.
Xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xxx xxx xxxx Xxxxxx$Xxxxxxx xx x xxxx.

## XXXXXXX XXXXX

[Get-Alias]()

[Import-Alias]()

[New-Alias]()

[Set-Alias]()

