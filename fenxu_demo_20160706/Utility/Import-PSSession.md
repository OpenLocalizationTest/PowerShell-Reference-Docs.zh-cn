---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293985
schema: 2.0.0
---

# Import-PSSession
## XXXXXXXX
Xxxxxxx xxxxxxxx xxxx xxxxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxx.

## XXXXXX

```
Import-PSSession [-Prefix <String>] [-DisableNameChecking] [[-CommandName] <String[]>] [-AllowClobber]
 [-ArgumentList <Object[]>] [-CommandType <CommandTypes>] [-Module <String[]>]
 [-FullyQualifiedModule <ModuleSpecification[]>] [[-FormatTypeName] <String[]>]
 [-Certificate <X509Certificate2>] [-Session] <PSSession> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XXXxxxxxx xxxxxx xxxxxxx xxxxxxxx $xxxx xx xxxxxxx$ xxxxxxxxx$ xxx xxxxxxx$ xxxx x XXXxxxxxx xx x xxxxx xx xxxxxx xxxxxxxx xxxx xxx xxxxxxx xxxxxxx.
Xxx xxx xxxxxx xxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xxx xxxx xx xxx XXXxxxxxx.

Xxx xx Xxxxxx$XXXxxxxxx xxxxxxx xx xxxxxx xxxxxxxx xxxx x xxxxxxxxxx xxxxx$ xxxx xx x Xxxxxxxxx Xxxxxxxx Xxxxxx xxxxx$ xx xxxx x xxxxxxx xxxx xxxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxx xxx xxxx$xxx xx xxxxx xxxxxxxx xxxx xxx xxx xx xxx xxxxxxx xxxxxxx.

Xx xxxxxx xxxxxxxx$ xxxxx xxx xxx Xxx$XXXxxxxxx xxxxxx xx xxxxxx x XXXxxxxxx.
Xxxx$ xxx xxx Xxxxxx$XXXxxxxxx xxxxxx xx xxxxxx xxx xxxxxxxx.
Xx xxxxxxx$ Xxxxxx$XXXxxxxxx xxxxxxx xxx xxxxxxxx xxxxxx xxx xxxxxxxx xxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xx xxxxxx xxx xxx xxxxxxxx$ xxx xxx XxxxxXxxxxxx xxxxxxxxx.

Xxx xxx xxx xxxxxxxx xxxxxxxx xxxx xx xxx xxxxx xxx xxx xxxxxxx xx xxx xxxxxxx.
Xxxx xxx xxx xx xxxxxxxx xxxxxxx$ xxx xxxxxxxx xxxx xx xxx xxxxxxx xxxx xxxxxxxxxx xx xxx xxxxxxx xxxx xxxxx xx xxx xxxxxxxx.
Xxxxxxx$ xxx xxxxxx xxxxxxxxxx xxx xxxxxxx xxxxxxxx xx Xxxxxxx XxxxxXxxxx.
Xxx xxxx xxx xxxx xx xxxxx xx xxxx$ xxxxxx xxxx xxx xxxx xxxx xxx xxxxxxxxxx xx xxx xxxxx xxxxxxx $XXXxxxxxx$ xxxx.
Xx xxx xxxxx xx$ xxx xxxxxxxx xxxxxxxx xxx xx xxxxxx xxxxxxxxx.

Xxxxxxx xxxxxxxx xxxxxxxx xxxxx xxxx xxxxxx xx xxx xxxx xxxxx xxxxxxxx$ Xxxxxx$XXXxxxxxx xxxx xx XxXxx xxxxxxxxx xx xxxxx xxxxxxxx xxxxxxx.
Xxxx xxxxxxxxx xxxxxx xxx xx xxx xxx xxxxxxx xx x Xxxxxxx XxxxxXxxxx xxxxxxxxxx xxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxx.

Xxxx xxx xxx Xxxxxx$XXXxxxxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxxxxx xxxxxxxx xx x xxxxxxxxx xxxxxx xxxx xxxxxx xxxx xx xxxx xxxxxxx xxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxxx.
Xx xxxxxx x xxxxxxxxxx xxxxxx xxxx xxx xxx xxx xx xxxxxx xxxxxxxx$ xxx xxx Xxxxxx$XXXxxxxxx xxxxxx.

Xxx Xxxxxx$XXXxxxxxx xxxxxx xxxx xxx xxxxxxxx xxxxxxxx xxxxxxx xx Xxxxxxx XxxxxXxxxx.
Xxxx xxx xxxxxx xxxxxxxx xxxx xxx xxxxxxx xxxxxxx$ xxxx xxx xxxxxxxxxx xx xxx xxxxxxxx xxxxxxx xx xx x  xxxxxxx xxxxxxx xx xxx xxxxxxxxxxx xxxxxxxx.

Xxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ xxx xxx xxx xxx Xxxxxx$Xxxxxx xxxxxx xx xxxxxx xxxxxxx xxxx x xxxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxx.
Xxxx xxxxxxx xxxx xxxxxxxx xxxxxxxx.
Xx xx xxxxxxxxxx xx xxxxx Xxxxxx$XXXxxxxxx xx xxxxxx xxxxxxxx xxxxxxx xxxx x xxxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$s = New-PSSession -ComputerName Server01

PS C:\>Import-PSSession -Session $s
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxxxx xxxx x XXXxxxxxx xx xxx Xxxxxx00 xxxxxxxx xxxx xxx xxxxxxx xxxxxxx$ xxxxxx xxx xxxxxxxx xxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.

Xxxxxxx xxxx xxxxxxx xxxx xxx xxx xxx XxxxxxxXxxx xxxxxxxxx$ xx xxxx xxxxxxx xxx xx xxx xxxxxxxxxx xxxx xxxxxxxx xxx xxx xxxxxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$s = New-PSSession https://ps.testlabs.com/powershell
PS C:\>Import-PSSession -Session $s -CommandName *-test -FormatTypeName *
PS C:\>New-Test -Name Test1
PS C:\>Get-Test test1 | Run-Test
```

Xxxxx xxxxxxxx xxxxxx xxx xxxxxxxx xxxx xxxxx xxxx xxx xx $$xxxx$ xxxx x XXXxxxxxx xxxx xxx xxxxx xxxxxxx$ xxx xxxx xxxx xxxx xxx xx xxx xx xxxxxxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XXXxxxxxx xxxxxx xx xxxxxx x XXXxxxxxx.
Xx xxxxx xxx XXXxxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx$XXXxxxxxx xxxxxx xx xxxxxx xxxxxxxx xxxx xxx XXXxxxxxx xx $x xxxx xxx xxxxxxx xxxxxxx.
Xx xxxx xxx XxxxxxxXxxx xxxxxxxxx xx xxxxxxx xxxxxxxx xxxx xxx Xxxx xxxx xxx xxx XxxxxxXxxxXxxx xxxxxxxxx xx xxxxxx xxx xxxxxxxxxx xxxx xxx xxx Xxxx xxxxxxxx.

Xxx xxxxx xxx xxxxxx xxxxxxxx xxx xxx xxxxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xxxxxxx xxxxxxxx xxxxxxxx xxx xxxxxxxx xxxxx xx xxx xxxxxxx xxxxxxx$ xxx xxx xxx xxxxx xxxxxx xx xxx xxxx.
Xxx xx xxx xxxx xx xxx xxx Xxxxxx$Xxxxxxx xxxxxx xx xxx xx xxxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$s1 = New-PSSession -ComputerName s1
PS C:\>$s2 = New-PSSession -ComputerName s2
PS C:\>Import-PSSession -Session s1 -Type cmdlet -Name New-Test, Get-Test -FormatTypeName *
PS C:\>Import-PSSession -Session s2 -Type Cmdlet -Name Set-Test -FormatTypeName *
PS C:\>New-Test Test1 | Set-Test -RunType Full
```

Xxxx xxxxxxx xxxxx xxxx xxx xxx xxx xxxxxxxx xxxxxxx xxxx xx xxx xxxxx xxx xxxxx xxxxxxx.

Xxxxx xxxxxxxx xxxxxx xxx Xxx$Xxxx xxx Xxx$Xxxx xxxxxxx xxxx x XXXxxxxxx xx xxx Xxxxxx00 xxxxxxxx xxx xxx Xxx$Xxxx xxxxxx xxxx x XXXxxxxxx xx xxx Xxxxxx00 xxxxxxxx.

Xxxx xxxxxx xxx xxxxxxx xxxx xxxxxxxx xxxx xxxxxxxxx XXXxxxxxxx$ xxx xxx xxxx xx xxxxxx xxxx xxx xxxxxx xx xxxxxxx xxxxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$s = New-PSSession -ComputerName Server01
PS C:\>Import-PSSession -Session $s -CommandName *-test* -FormatTypeName *
PS C:\>$batch = New-Test -Name Batch -AsJob
PS C:\>Receive-Job $batch
```

Xxxx xxxxxxx xxxxx xxx xx xxx xx xxxxxxxx xxxxxxx xx x xxxxxxxxxx xxx.

Xxxxxxx xxxxxxxx xxxxxxxx xxxxx xxxx xxxxxx xx xxx xxxx xxxxx xxxxxxxx$ Xxxxxx$XXXxxxxxx xxxx xx XxXxx xxxxxxxxx xx xxxxx xxxxxxxx xxxxxxx.
Xxx XxXxx xxxxxxxxx xxxx xxx xxx xxx xxxxxxx xx x xxxxxxxxxx xxx.

Xxx xxxxx xxxxxxx xxxxxxx x XXXxxxxxx xx xxx Xxxxxx00 xxxxxxxx xxx xxxxx xxx XXXxxxxxx xxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx Xxxxxx$XXXxxxxxx xx xxxxxx xxx Xxxx xxxxxxx xxxx xxx XXXxxxxxx xx $x xxxx xxx xxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx XxXxx xxxxxxxxx xx xxx xxxxxxxx Xxx$Xxxx xxxxxx xx xxx x Xxx$Xxxx xxxxxxx xx x xxxxxxxxxx xxx.
Xxx xxxxxxx xxxxx xxx xxx xxxxxx xxxx Xxx$Xxxx xxxxxxx xx xxx $xxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxxx$Xxx xxxxxx xx xxx xxx xxxxxxx xx xxx xxx xx xxx $xxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$s = New-PSSession -ComputerName Server01
PS C:\>Invoke-Command -Session $s {Import-Module TestManagement}
PS C:\>Import-PSSession -Session $s -Module TestManagement
```

Xxxx xxxxxxx xxxxx xxx xx xxxxxx xxx xxxxxxx xxx xxxxxxxxx xxxx x Xxxxxxx XxxxxXxxxx xxxxxx xx x xxxxxx xxxxxxxx xxxx xxx xxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x XXXxxxxxx xx xxx Xxxxxx00 xxxxxxxx xxx xxxxx xx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx$Xxxxxxx xxxxxx xx xxx xx Xxxxxx$Xxxxxx xxxxxxx xx xxx XXXxxxxxx xx $x.

Xxxxxxxxx$ xxx xxxxxx xxxxx xx xxxxx xx xxx xxxxxxxx xx xx Xxxxxx$Xxxxxx xxxxxxx xx x Xxxxxxx XxxxxXxxxx xxxxxxx$ xxx xxxxxxxx xxx xxx xxx xx XXXxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxx xxxxxxxxx xx Xxxxxx$XXXxxxxxx xx xxxxxx xxx xxxxxxx xxx xxxxxxxxx xx xxx xxxxxx xxxx xxx xxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Import-PSSession $s -CommandName Get-Date, SearchHelp  -FormatTypeName * -AllowClobber

Name              : tmp_79468106-4e1d-4d90-af97-1154f9317239_tcw1zunz.ttf
Path              : C:\Users\User01\AppData\Local\Temp\tmp_79468106-4e1d-4d90-af97-1154f9317239_tcw1zunz.ttf\tmp_79468106-4e1d-4d90-af97-1154f9317239_
tcw1zunz.ttf.psm1
Description       : Implicit remoting for http://server01.corp.fabrikam.com/wsman
Guid              : 79468106-4e1d-4d90-af97-1154f9317239
Version           : 1.0
ModuleBase        : C:\Users\User01\AppData\Local\Temp\tmp_79468106-4e1d-4d90-af97-1154f9317239_tcw1zunz.ttf
ModuleType        : Script
PrivateData       : {ImplicitRemoting}
AccessMode        : ReadWrite
ExportedAliases   : {}
ExportedCmdlets   : {}
ExportedFunctions : {[Get-Date, Get-Date], [SearchHelp, SearchHelp]}
ExportedVariables : {}
NestedModules     : {}
```

Xxxx xxxxxxx xxxxx xxxx Xxxxxx$XXXxxxxxx xxxxxxx x xxxxxx xx x xxxxxxxxx xxxx xx xxxx.
Xx xxxx xxxxx xxxx xxx xxxxxxxx xxx xxxxxxxxx xxxx xxxxxxxxx xxxxxx xxxx xxx xxxxxxxx xxxx xxx xxxxxxx xxxxxxx.

Xxx xxxxxxx xxxx xxx Xxxxxx$XXXxxxxxx xxxxxx xx xxxxxx x Xxx$Xxxx xxxxxx xxx x XxxxxxXxxx xxxxxxxx xxxx xxx xxxxxxx xxxxxxx.

Xxx Xxxxxx$XXXxxxxxx xxxxxx xxxxxxx x XXXxxxxxXxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxxxx xxxxxx.
Xxx xxxxx xx xxx Xxxx xxxxxxxx xxxxx xxxx Xxxxxx$XXXxxxxxx xxxxxxx x xxxxxx xxxxxx $.xxx0$ xxxx xx x xxxxxxxxx xxxxxxxx.
Xxx XxxxxxxxXxxxxxxxx xxxxxxxx xxxxx xxxx xxx Xxx$Xxxx xxxxxx xxx xxx XxxxxxXxxx xxxxxxxx xxxx xxxx xxxxxxxx xx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Import-PSSession $s -CommandName Get-Date -FormatTypeName * -AllowClobber

PS C:\>Get-Command Get-Date -All

CommandType   Name       Definition
-----------   ----       ----------
Function      Get-Date   ...
Cmdlet        Get-Date   Get-Date [[-Date] <DateTime>] [-Year <Int32>] [-Month <Int32>]

PS C:\>Get-Date
09074

PS C:\>(Get-Command -Type Cmdlet -Name Get-Date).PSSnapin.Name
Microsoft.PowerShell.Utility

PS C:\>Microsoft.PowerShell.Utility\Get-Date
Sunday, March 15, 2009 2:08:26 PM
```

Xxxx xxxxxxx xxxxx xxx xx xxx x xxxxxxx xxxx xx xxxxxx xx xx xxxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x Xxx$Xxxx xxxxxx xxxx xxx XXXxxxxxx xx xxx $x xxxxxxxx.
Xxxxxxx xxx xxxxxxx xxxxxxx xxxxxxxx x Xxx$Xxxx xxxxxx$ xxx XxxxxXxxxxxx xxxxxxxxx xx xxxxxxxx xx xxx xxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxx xxxxxxxxx xx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx Xxx$Xxxx xxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxxxxx xxxxx xxxx xxx xxxxxxx xxxxxxxx xxx xxxxxxxx Xxx$Xxxx xxxxxx xxx x Xxx$Xxxx xxxxxxxx.
Xxx Xxx$Xxxx xxxxxxxx xxxx xxx xxxxxxxx Xxx$Xxxx xxxxxx xx xxx XXXxxxxxx xx $x.

Xxx xxxxx xxxxxxx xxxx x Xxx$Xxxx xxxxxxx.
Xxxxxxx xxxxxxxxx xxxx xxxxxxxxxx xxxx xxxxxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxxxxx Xxx$Xxxx xxxxxxxx$ xxxxx xxxxxxx x Xxxxxx xxxx.

Xxx xxxxxx xxx xxxxx xxxxxxxx xxxx xxx xx xxx x xxxxxxxxx xxxx xx xxx x xxxxxxx xxxx xx xxxxxx xx xx xxxxxxxx xxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxx xx xxx Xxxxxxx XxxxxXxxxx xxxx$xx xxxx xxxxx xxx xxxxxxxx Xxx$Xxxx xxxxxx xx xxx xxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxx$xx$xxxxxxxxx xxxx xx xxx Xxx$Xxxx xxxxxx xx xxx x Xxx$Xxxx xxxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxxxxxx xxxxxxxxxx xxx xxxxxx xxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Import-PSSession -Session $s -CommandName *Item* -AllowClobber
```

Xxxx xxxxxxx xxxxxxx xxxxxxxx xxxxx xxxxx xxxxxxx $Xxxx$ xxxx xxx XXXxxxxxx xx $x.
Xxxxxxx xxx xxxxxxx xxxxxxxx xxx XxxxxxxXxxx xxxxxxxxx xxx xxx xxx XxxxxxXxxxXxxx xxxxxxxxx$ xxxx xxx xxxxxxx xx xxxxxxxx.

Xxx xxxx xxxxxxx xxxx xxx xxx xxxxx Xxxxxx$XXXxxxxxx xx xxx x xxxxxxx xx x xxxxxx xxxxxxxx xxx xxx xxxxxxx xxxx xxx xxxxxxxxxx xxxx xxx xxx xxxxxxx xx xxx xxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$m = Import-PSSession -Session $s -CommandName *bits* -FormatTypeName *bits*
PS C:\>Get-Command -Module $m
CommandType     Name
-----------     ----
Function        Add-BitsFile
Function        Complete-BitsTransfer
Function        Get-BitsTransfer
Function        Remove-BitsTransfer
Function        Resume-BitsTransfer
Function        Set-BitsTransfer
Function        Start-BitsTransfer
Function        Suspend-BitsTransfer
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx Xxxxxx xxxxxxxxx xx Xxx$Xxxxxxx xx xxxx xxx xxxxx xxxxxxxx xxxx xxxxxxxx xxxx xxx xxxxxxx xx xx Xxxxxx$XXXxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxx$XXXxxxxxx xxxxxx xx xxxxxx xxxxxxxx xxxxx xxxxx xxxxxxx $xxxx$ xxxx xxx XXXxxxxxx xx xxx $x xxxxxxxx.
Xxx Xxxxxx$XXXxxxxxx xxxxxxx xxxxxxx x xxxxxxxxx xxxxxx$ xxx xxx xxxxxxx xxxxx xxx xxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxxx xx xxx $x xxxxxxxx.

Xxx Xxxxxx xxxxxxxxx xxxxx x xxxxxx xxxxx$ xxxxx xx xxxxxxxx xxx xxx xxxxxx xxxx.
Xxxxxxx$ xxxx xxx xxxxxx x xxxxxx xxxxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx XxXxxxxx xxxxxx xx xxx xxxxxx xxxxxx$ xxxxx xxxxxxx xxx xxxxxx xxxx.

Xxx Xxx$Xxxxxxx xxxxxxx xx xxx xxxxxxxxxx xx Xxx$Xxxxxxx $x.Xxxx$.

## XXXXXXXXXX

### -AllowClobber
Xxxxxxx xxx xxxxxxxxx xxxxxxxx$ xxxx xx xxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.

Xx xxx xxxxxx x xxxxxxx xxxx xxx xxxx xxxx xx x xxxxxxx xx xxx xxxxxxx xxxxxxx$ xxx xxxxxxxx xxxxxxx xxxxx xx xxxxxxxx xxx xxxxxxxx xxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxxxxxxx.

Xx xxxxxxx$ Xxxxxx$XXXxxxxxx xxxx xxx xxxxxx xxxxxxxx xxxx xxxx xxx xxxx xxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.

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

### -ArgumentList
Xxxxxxx xxx xxxxxxx xx xxx xxxxxxx xxxx xxxxxxx xxxx xxxxx xxx xxxxxxxxx xxxxxxxxx $xxxxxxxxx xxxxxx$.

Xxx xxxxxxx$ xx xxxxxx xxx xxxxxxx xx xxx Xxx$Xxxx xxxxxxx xx xxx xxxxxxxxxxx $Xxxx$$ xxxxx xx xxx XXXxxxxxx xx $x$ xxxx $Xxxxxx$XXXxxxxxx $Xxxxxxx $x $xxxxxxx xxx$xxxx $xxxxxxxxxxxx xxxx$$.

```yaml
Type: Object[]
Parameter Sets: (All)
Aliases: Args

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CommandName
Xxxxxxx xxxx xxx xxxxxxxx xxxx xxx xxxxxxxxx xxxxx xx xxxx xxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.
Xxx $XxxxxxxXxxx$ xx xxx xxxxx$ $Xxxx$.

Xx xxxxxxx$ Xxxxxx$XXXxxxxxx xxxxxxx xxx xxxxxxxx xxxx xxx xxxxxxx$ xxxxxx xxx xxxxxxxx xxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xxxx xxxxxxxx xxxxxxxx xxxxxxxx xxxx xxxxxx xx xxxxxxxxx xxxxxxxx xx xxx xxxxxxx.
Xx xxxxxx xxx xxxxxxxx$ xxxx xxxxx xxxx xxxx xx xxxxxxx xxxxx xxxxxxxx$ xxx xxx XxxxxXxxxxxx xxxxxxxxx.

Xx xxx xxx xxx XxxxxxxXxxx xxxxxxxxx$ xxx xxxxxxxxxx xxxxx xxx xxx xxxxxxxx xxx xxx xxxxxxxx xxxxxx xxx xxx xxx XxxxxxXxxxXxxx xxxxxxxxx.
Xxxxxxxxx$ xx xxx xxx xxx XxxxxxXxxxXxxx xxxxxxxxx$ xx xxxxxxxx xxx xxxxxxxx xxxxxx xxx xxx xxx XxxxxxxXxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Name

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CommandType
Xxxxxxx xxxx xxx xxxxxxxxx xxxxx xx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxxx xx Xxxxxx.
Xxx $XxxxxxxXxxx$ xx xxx xxxxx$ $Xxxx$.

Xxxxx xxxxxx xxx$

$$ Xxxxx$ Xxx Xxxxxxx XxxxxXxxxx xxxxxxx xx xxx xxxxxx xxxxxxx.
$$ Xxx$ Xxx xxxxxxx xxx xxxxxxxxx xx xxx xxxxxx xxxxxxx.
$$ Xxxxxxxxxxx$ Xxx xxx xxxxx xxxxx xxxx Xxxxxxx$XxxxxXxxxx xxxxx xx xxx xxxxx xxxx xxx xxxxxx xx xxx Xxxx xxxxxxxxxxx xxxxxxxx $$xxx$xxxx$ xx xxx xxxxxx xxxxxxx$ xxxxxxxxx .xxx$ .xxx$ xxx .xxx xxxxx.
$$ Xxxxxx$ Xxx xxxxxxx xx xxx xxxxxx xxxxxxx. $Xxxxxx$ xx xxx xxxxxxx.
$$ XxxxxxxxXxxxxx$ Xxx .xx0 xxxxx xx xxx xxxxx xxxxxx xx xxx Xxxx xxxxxxxxxxx xxxxxxxx $$xxx$xxxx$ xx xxx xxxxxx xxxxxxx.
$$ Xxxxxx xxx Xxxxxxxx$ Xxx Xxxxxxx XxxxxXxxxx xxxxxxxxx xx xxx xxxxxx xxxxxxx.
$$ Xxxxxx$ Xxx xxxxxx xxxxxx xx xxx xxxxxx xxxxxxx.

```yaml
Type: CommandTypes
Parameter Sets: (All)
Aliases: Type
Accepted values: Alias, Function, Filter, Cmdlet, ExternalScript, Application, Script, Workflow, Configuration, All

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisableNameChecking
Xxxxxxxxxx xxx xxxxxxx xxxx xxxxx xxx xxxx xxx xxxxxx x xxxxxx xx xxxxxxxx xxxxx xxxx xxxxxxxx xx xxxxxxxxxx xxxx xx x xxxxxxxxxx xxxxxxxxx.

Xx xxxxxxx$ xxxx x xxxxxx xxxx xxx xxxxxx xxxxxxx xxxxxxx xx xxxxxxxxx xxxx xxxx xxxxxxxxxx xxxxx xx xxxxx xxxxx$ xxx Xxxxxxx XxxxxXxxxx xxxxxxxx xxx xxxxxxxxx xxxxxxx xxxxxxx$

$XXXXXXX$ Xxxx xxxxxxxx xxxxxxx xxxxx xxxxxxx xxxxxxxxxx xxxxx xxxxx xxxxx xxxx xxxx xxxx xxxxxxxxxxxx. Xxx xxx Xxxxxxx xxxxxxxxx xxx xxxx xxxxxx xx xxxx Xxx$Xxxx xx xxx xxx xxxx xx xxxxxxxx xxxxx.$

Xxxx xxxxxxx xx xxxx x xxxxxxx.
Xxx xxxxxxxx xxxxxx xx xxxxx xxxxxxxx$ xxxxxxxxx xxx xxx$xxxxxxxxxx xxxxxxxx.
Xxxxxxxx xxx xxxxxxx xx xxxxxxxxx xx xxxxxx xxxxx$ xxx xxxxxx xxxxxxx xxxxxx xx xxxxx xx xxx xxxxxx xxxxxx.

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

### -FormatTypeName
Xxxxxxx xxxxxxxxxx xxxxxxxxxxxx xxx xxx xxxxxxxxx Xxxxxxxxx .XXX Xxxxxxxxx xxxxx.
Xxxxx xxx xxxx xxxxx.
Xxxxxxxxx xxx xxxxxxxxx.

Xxx xxxxx xx xxxx xxxxxxxxx xxxx xx xxx xxxx xx x xxxx xxxx xx xxxxxxxx xx x Xxx$XxxxxxXxxx xxxxxxx xx xxx xxxxxxx xxxx xxxxx xxx xxxxxxxx xxx xxxxx xxxxxxxx.
Xx xxx xxx xx xxx xxxxxxxxxx xxxx xx xxx xxxxxx xxxxxxx$ xxxx $.

Xx xxx xxxxxxx xxxx xxx xxxxxxx xxxxxx xxx XxxxxxxXxxx xx XxxxxxXxxxXxxx xxxxxxxxxx$ Xxxxxx$XXXxxxxxxxxxxxxx xxxxxxxxxx xxxxxxxxxxxx xxx xxx .XXX Xxxxxxxxx xxxxx xxxxxxxx xx x Xxx$XxxxxxXxxx xxxxxxx xx xxx xxxxxx xxxxxxx.

Xx xxx xxx xxx XxxxxxXxxxXxxx xxxxxxxxx$ xx xxxxxxxx xxx xxxxxxxx xxxxxx xxx xxx xxx XxxxxxxXxxx xxxxxxxxx.

Xxxxxxxxx$ xx xxx xxx xxx XxxxxxxXxxx xxxxxxxxx$ xxx xxxxxxxxxx xxxxx xxx xxx xxxxxxxx xxx xxx xxxxxxxx xxxxxx xxx xxx xxx XxxxxxXxxxXxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FullyQualifiedModule
Xxxxxxxxx xxxxxxx xxxx xxxxx xxxx xxx xxxxxxxxx xx xxx xxxx xx XxxxxxXxxxxxxxxxxxx xxxxxxx $xxxxxxxxx xx xxx Xxxxxxx xxxxxxx xx Xxxxxx Xxxxxxxxxxxxx Xxxxxxxxxxx $Xxxxxxxxx$ xx XXXX$.
Xxx xxxxxxx$ xxx XxxxxXxxxxxxxxXxxxxx xxxxxxxxx xxxxxxx x xxxxxx xxxx xxxx xx xxxxxxxxx xx xxx xxxxxx $$XxxxxxXxxx $ $xxxxxxxxxx$$ XxxxxxXxxxxxx $ $xxxxxxx$xxxxxx$$ xx $$XxxxxxXxxx $ $xxxxxxxxxx$$ XxxxxxXxxxxxx $ $xxxxxxx$xxxxxx$$ Xxxx $ $XXXX$$.
XxxxxxXxxx xxx XxxxxxXxxxxxx xxx xxxxxxxx$ xxx Xxxx xx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxx XxxxxXxxxxxxxxXxxxxx xxxxxxxxx xx xxx xxxx xxxxxxx xx x Xxxxxx xxxxxxxxx$ xxx xxx xxxxxxxxxx xxx xxxxxxxx xxxxxxxxx.

```yaml
Type: ModuleSpecification[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
Xx xxx xxxxxx x xxxxxxx xxxx xxx xxxx xxxx xx x xxxxxxx xx xxx xxxxxxx xxxxxxx$ xxx xxxxxxxx xxxxxxx xxxxx xx xxxxxxxx xxx xxxxxxxx xxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxxxxxxx.

Xx xxxxxxx$ Xxxxxx$XXXxxxxxx xxxx xxx xxxxxx xxxxxxxx xxxx xxxx xxx xxxx xxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.

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
Xx xxx xxxxxx x xxxxxxx xxxx xxx xxxx xxxx xx x xxxxxxx xx xxx xxxxxxx xxxxxxx$ xxx xxxxxxxx xxxxxxx xxxxx xx xxxxxxxx xxx xxxxxxxx xxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxxxxxxx.

Xx xxxxxxx$ Xxxxxx$XXXxxxxxx xxxx xxx xxxxxx xxxxxxxx xxxx xxxx xxx xxxx xxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.

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

### -Module
Xxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxxxxxx Xxxxxxx XxxxxXxxxx xxxx$xxx xxx xxxxxxx.
Xxxxx xxx xxxx$xx xxx xxxxxx xxxxx.
Xxxxxxxxx xxx xxx xxxxxxxxx.

Xxxxxx$XXXxxxxxx xxxxxx xxxxxx xxxxxxxxx xxxx x xxxx$xx.

Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$XXXxxxxxx xxx xxxxx$Xxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: PSSnapin

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Prefix
Xxxx xxx xxxxxxxxx xxxxxx xx xxx xxxxx xx xxx xxxxx xx xxxxxxxx xxxxxxxx.

Xxx xxxx xxxxxxxxx xx xxxxx xxxx xxxxxxxxx xxxx xxxxx xxxxx xxxx xxxxxxxxx xxxxxxxx xx xxx xxxxxxx xxxx xxx xxxx xxxx.

Xxx xxxxxxx$ xx xxx xxxxxxx xxx xxxxxx $Xxxxxx$ xxx xxxx xxxxxx x Xxx$Xxxx xxxxxx$ xxx xxxxxx xx xxxxx xx xxx xxxxxxx xx $Xxx$XxxxxxXxxx$ xxx xx xx xxx xxxxxxxx xxxx xxx xxxxxxxx Xxx$Xxxx xxxxxx.

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

### -Session
Xxxxxxxxx xxx XXXxxxxxx xxxx xxxxx xxx xxxxxxx xxx xxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx x xxxxxxx xxxxxx xx x xxxxxxx xxxx xxxx x xxxxxxx xxxxxx$ xxxx xx x Xxx$XXXxxxxxx xx Xxx$XXXxxxxxx xxxxxxx.
Xxx xxx xxxxxxx xxxx xxx xxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx.

```yaml
Type: PSSession
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Certificate
Xxxxxxxxx xxx xxxxxx xxxxxxxxxxx xxxx xx xxxx xx xxxx xxx xxxxxx xxxxx $$.Xxxxxx.xx0xxx$ xx xxxxxx xxxxxx xxxxx $.xxx0$ xx xxx xxxxxxxxx xxxxxx xxxx Xxxxxx$XXXxxxxxx xxxxxxx.

Xxxxx x xxxxxxxx xxxx xxxxxxxx x xxxxxxxxxxx xx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxxxxxx.

Xx xxxx x xxxxxxxxxxx$ xxx xxx Xxx$XxxXxxxxxxxxxx xxxxxx xx xxx xxx Xxx$XxxxxXxxx xxxxxx xx xxx Xxxxxxxxxxx $Xxxx$$ xxxxx.
Xx xxx xxxxxxxxxxx xx xxx xxxxx xx xxxx xxx xxxx xxxxxxxxxx xxxxxxxxx$ xxx xxxxxxx xxxxx.

```yaml
Type: X509Certificate2
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### None
Xxx xxxxxx xxxx xxxxxxx xx xxxx xxxxxx.

## XXXXXXX

### System.Management.Automation.PSModuleInfo
Xxxxxx$XXXxxxxxx xxxxxxx xxx xxxx xxxxxx xxxxxx xxxx Xxx$Xxxxxx xxx Xxx$Xxxxxx xxxxxxx xxxxxx.
Xxxxxxx$ xxx xxxxxxxx xxxxxx xx xxxxxxxxx xxx xxxxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxxxxx x xxxxxxxxx xxxxxx xx xxxx$ xxx xxx Xxxxxx$XXXxxxxxx xxxxxx.

## XXXXX
Xxxxxx$XXXxxxxxx xxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx xxxxxxxxxxxxxx.
Xx xxx xxxx xxxxxx$ xxx xxxxxxxx xxxx xx xxxxxxxxxx xxx XX$Xxxxxxxxxx xxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxx xxx xxxxx$Xxxxxx$Xxxxxxxxxxxx.

Xxxxxx$XXXxxxxxx xxxx xxx xxxxxx xxxxxxxxx xx Xxxxxxx XxxxxXxxxx xxxxxxxxx.

Xxxx xxx xxxxxx xxxxxxxx xxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx$ xxx xxxxxxxx xxxxxxxx xxx xxxx xxxxxxx$ xxxxxxxxx$ xxx xxxxxxx xx xxx xxxxxxx xxx xxxx xxx xxxxxxx xxxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxx.
Xx xxxxxxx xxxx xxxxxxxxx$ xxx xxx Xxxxxx xxxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxxxxxxx.

Xxxxxx$XXXxxxxxx xxxxxxxx xxx xxxxxxxx xxxx xxxxxxxxx xxxxxx xx xxxxxxx xxxx.
Xx x xxxxxx$ xxxxxxxx xxxxxxxx xxxxxx x xxx xxxxxxxxxxx xxxx xxxx xxxxx xx xxxx xxxxxxxx xxxxx xxxxxxxx xxxxxxx xxxx.
Xxx xxxxxxx$ xx xxx xxxxxx x xxxxxx xxxx x XXXxxxxxx xxx xxxx xxxxxx x xxxxxx xxxx xxx xxxx xxxx xxxx x xxxxxx xx xxxx$xx$ xxx xxxxxx xxxx xx xxxxxxxx xxxx xxx XXXxxxxxx xxxxxx xxxx xx xxxxxxx xxxxxxx xxxxxxxxx xxxx xxxxxxxxxx xxxx xxxxxxx.
Xxxxxxxxxx$ xx xxx xxxxxx xx xxxxx xxxx x xxxxxxx xxxx xxx xx xxxxx xxxx xxx xxxx xxxx$ xxx xxxxxxxx xxxxx xx xxxxxx xxxx$ xxxxxxx xxxxxxx xxxx xxxxxxxxxx xxxx xxxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxxxxxxx.

Xxxxxx$XXXxxxxxx xxxx xxx Xxxxx$Xxxxxxxx xxxxxx xx xxxxxxx xxx xxxxxxxx xx xxx xxxxxxx.
Xxx xxxxx xxx xxx xxxxxxxx xxx xxxxx xxx xxxxxxx xx xxxxxxx.

Xx xxxx xxx xxxxxxxx xx xxxxxx$ Xxxxxx$XXXxxxxxx xxxx xxx Xxxxxx$Xxxxxxx xxxxxx xx xxx x Xxx$Xxxxxxx xxxxxxx xx xxx XXXxxxxxx.
Xx xxx xxxxxxxxxx xxxx xxx xxx xxxxxxxx$ xx xxxx xxx Xxx$XxxxxxXxxx xxxxxx.
Xxx xxxxx xxx xxxxx xxxxxxxx xxxx xxxxx xxxxxxx xxxx xxx xxx xx Xxxxxx$XXXxxxxxx xxxxxxx.
Xxxx$ Xxxxxx$XXXxxxxxx xxxxxx xxxxxx xxxxxxxx xxxx x XXXxxxxxx xxxx xxxx xxx xxxxxxx xxx Xxx$Xxxxxxx$ Xxx$XxxxxxXxxx$ Xxxxxx$Xxxxxx$ xxx Xxx$Xxxx xxxxxxx.

Xxxxxxxx xxxxxxxx xxxx xxx xxxx xxxxxxxxxxx xx xxxxx xxxxxx xxxxxxxx$ xxxxxxxxx xxx xxxxxxxxx xx xxxxx x xxxxxxx xxxx x xxxx xxxxxxxxx$ xxxx xx Xxxxxxx.

Xxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxxx xxx xxx xxx xx XXXxxxxxxx$ xxx xxxxxxxx xxxx x xxxxxxx xxxx xx x xxxxxxx xxx xxx xxxxxxxxx xx Xxxxxx$XXXxxxxxx.
Xx xxxxxx xxxxxxxx xxxx x xxxxxxx$ xxx xx Xxxxxx$Xxxxxxx xxxxxxx xx xxx xxx xxxxxxx xx xxx XXXxxxxxx xxxxxxxx xxxxxx xxxxxxxxx xxxxxxxx.

Xxx xxxxxxxxx xxxxxx xxxx Xxxxxx$XXXxxxxxx xxxxxxx xxxxx xxxxxxx x xxxxxxxxxx xxxx$ xxxx xx xxx xxxxxxx xxxx xxx xxxxxx xxxxxxxxxx xxxx.
Xx xxx xxxxxxx xxxx xxx xxxxxx xxxxxxxxxx xxxx$ xxx xxxxxxxxxx xxxxx xxxx xxx xxxxxxx xxxx xxx xxxxxxx xxxxxxxxxx xxxx.

Xx xxx Xxxxxx$XXXxxxxxx$ xxx xxxxxxxxx xxxxxx xx xxx xxxxxxx xxxxxxx xxxxxx xx Xxxxxxxxxx xx XxxXxxxxx$ xxxxxxx xxx xxxxxxxxx xxxxxx xxxx Xxxxxx$XXXxxxxxx xxxxxxx xxxxxxxx xxxxxxxx xxxxxx xxxxx xxxx xxx xxxxxxxxxx xx xxxxx xxxxxxxx.
Xx xxx Xxxxxx$XXXxxxxxx xxxxxxx xxxxxxxx xxx xxxxxxxxx xxxxxx xxx xxx xxxxx xxxxxxxx$ xxx xxx Xxxxx xxxxxxxxx xx Xxx$XxxxxxxxxXxxxxx xx xxx x xxxx xxxxxxxxxxx xxxxxxxxx xxxxxx xxx x xxxxxx xxxxxxx.

Xx Xxxxxxx XxxxxXxxxx 0.0$ xxxx xxxxxx xxx xxxxxxxx xxxx xxx xxxxxxxx xxxx xxxxxxx xxxxxxx xx xxx xxxxxxx xxx xxxxxx xxxx xxx xxxxxx xx xxxxx xxx Xxxxxx xxxxxxxxx.
Xx xxx xxxx xxx xx xxxxxxxx xxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ xxx xxx xxxxxxxx $xxx$xxxxxxxx$ xxxxxxx xxxx.

## XXXXXXX XXXXX

[Export-PSSession]()

[New-PSSession]()

[about_Command_Precedence]()

[about_PSSessions]()

[about_Jobs]()

