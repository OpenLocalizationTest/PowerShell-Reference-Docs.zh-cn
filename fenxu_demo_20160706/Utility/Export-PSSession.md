---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293959
schema: 2.0.0
---

# Xxxxxx$XXXxxxxxx
## XXXXXXXX
Xxxxxxx xxxxxxxx xxxx xxxxxxx xxxxxxx xxx xxxxx xxxx xx x Xxxxxxx XxxxxXxxxx xxxxxx.

## XXXXXX

```
Export-PSSession [-OutputModule] <String> [-Force] [-Encoding <String>] [[-CommandName] <String[]>]
 [-AllowClobber] [-ArgumentList <Object[]>] [-CommandType <CommandTypes>] [-Module <String[]>]
 [-FullyQualifiedModule <ModuleSpecification[]>] [[-FormatTypeName] <String[]>]
 [-Certificate <X509Certificate2>] [-Session] <PSSession> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XXXxxxxxx xxxxxx xxxx xxxxxxx$ xxxxxxxxx$ xxxxxxx$ xxx xxxxx xxxxxxx xxxxx xxxx xxxxxxx XXXxxxxxx xx x xxxxx xx xxxxxx xxxxxxxx xxx xxxxx xxxx xx x Xxxxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxxx xxxx xxx xxxxxx xx xxx xxxxxxx xxxxxxx$ xxx xxx Xxxxxx$Xxxxxx xxxxxx.

Xxxxxx Xxxxxx$XXXxxxxxx$ xxxxx xxxxxxx xxxxxxxx xxxx xxxxxxx XXXxxxxxx xxxx xxx xxxxxxx xxxxxxx$ Xxxxxx$XXXxxxxxx xxxxx xxx xxxxxxxx xx x xxxxxx.
Xxx xxxxxxxx xxx xxx xxxxxxxx xxxx xxx xxxxxxx xxxxxxx.

Xx xxxxxx xxxxxxxx$ xxxxx xxx xxx Xxx$XXXxxxxxx xxxxxx xx xxxxxx x XXXxxxxxx xxxx xxx xxx xxxxxxxx xxxx xxx xxxx xx xxxxxx.
Xxxx xxx xxx Xxxxxx$XXXxxxxxx xxxxxx xx xxxxxx xxx xxxxxxxx.
Xx xxxxxxx$ Xxxxxx$XXXxxxxxx xxxxxxx xxx xxxxxxxx$ xxxxxx xxx xxxxxxxx xxxx xxxxx xx xxx xxxxxxx xxxxxxx$ xxx xxx xxx xxx xxx XxxxxxxXxxx xxxxxxxxxx xx xxxxxxx xxx xxxxxxxx xx xxxxxx.

Xxx Xxxxxx$XXXxxxxxx xxxxxx xxxx xxx xxxxxxxx xxxxxxxx xxxxxxx xx Xxxxxxx XxxxxXxxxx.
Xxxx xxx xxxxxx xxxxxxxx xxxx xxx xxxxxxx xxxxxxx$ xxxx xxx xxxxxxxxxx  xx xxx xxxxxxxx xxxxxxx xx xx x  xxxxxxx xxxxxxx xx xxx xxxxxxxxxxx xxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$s = new-pssession -computerName Server01
PS C:\>export-pssession -session $s -outputModule Server01
```

Xxx xxxxxxxx xx xxxx xxxxxxx xxxxxx xxx xxxxxxxx xxxx x XXXxxxxxx xx xxx Xxxxxx00 xxxxxxxx xx xxx Xxxxxx00 xxxxxx xx xxx xxxxx xxxxxxxx xxxxxx xxx xxxxxxxx xxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xx xxxx xxxxxxx xxx xxxxxxxxxx xxxx xxx xxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x XXXxxxxxx xx xxx Xxxxxx00 xxxxxxxx.
Xxx xxxxxx xxxxxxx xxxxxxx xxx xxxxxxxx xxx xxxxxxxxxx xxxx xxxx xxx xxxxxxx xxxx xxx Xxxxxx00 xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$s = new-pssession -ConnectionUri http://exchange.microsoft.com/mailbox -credential exchangeadmin01@hotmail.com -authentication negotiate
PS C:\>export-pssession -session $r -module exch* -commandname get-*, set-* -formattypename * -outputModule $pshome\Modules\Exchange -encoding ASCII
```

Xxxxx xxxxxxxx xxxxxx xxx Xxx xxx Xxx xxxxxxxx xxxx x Xxxxxxxxx Xxxxxxxx Xxxxxx xxxx$xx xx x xxxxxx xxxxxxxx xx xx Xxxxxxxx xxxxxx xx xxx $xxxxxx$Xxxxxxx xxxxxxxxx xx xxx xxxxx xxxxxxxx.

Xxxxxxx xxx xxxxxx xx xxx $xxxxxx$Xxxxxx xxxxxxxxx xxxxx xx xxxxxxxxxx xx xxx xxxxx xx xxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$s = new-pssession -computerName Server01 -credential Server01\User01
PS C:\>export-pssession -session $s -outputModule TestCmdlets -type cmdlet -commandname *test* -formattypename *
PS C:\>remove-pssession $s
PS C:\>import-module TestCmdlets
PS C:\>get-help test*
PS C:\>test-files
```

Xxxxx xxxxxxxx xxxxxx xxxxxxx xxxx x XXXxxxxxx xx x xxxxxx xxxxxxxx xxx xxxx xxxx xx x xxxxxx xx xxx xxxxx xxxxxxxx.
Xxxx$ xxx xxxxxxxx xxx xxx xxxxxxx xxxx xxx xxxxxx xx xxx xxxxxxx xxxxxxx xx xxxx xxxx xxx xx xxxx.

Xxx xxxxx xxxxxxx xxxxxxx x XXXxxxxxx xx xxx Xxxxxx00 xxxxxxxx xxx xxxxx xx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx xxx xxxxxxx xxxxx xxxxx xxxxx xxxx $Xxxx$ xxxx xxx XXXxxxxxx xx $x xx xxx XxxxXxxxxxx xxxxxx xx xxx xxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxx$XXXxxxxxx xxxxxx xx xxxxxx xxx XXXxxxxxx xx $x xxxx xxx xxxxxxx xxxxxxx.
Xxxx xxxxxxx xxxxx xxxx xxx XXXxxxxxx xxxx xxx xx xxxxxx xx xxx xxx xxxxxxxx xxxx xxxx xxxxxxxx xxxx xx.

Xxx xxxxxx xxxxxxx$ xxxxx xxx xx xxx xx xxx xxxxxxx xx xxx xxxx$ xxxx xxx Xxxxxx$Xxxxxx xxxxxx xx xxx xxx xxxxxxx xx xxx XxxxXxxxxxx xxxxxx xx xxx xxxxxxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx xxxx xxx xxxxxxx xxxxx xxxxx xxxxx xxxx $Xxxx.$ Xxxxx xxx xxxxxxxx xx x xxxxxx xxx xxxxx xx xxx xxxxxxx xxxxxxx$ xxx xxx xxx xxx Xxx$Xxxx xxx Xxx$Xxxxxxx xxxxxxx xx xxxxx xxxxx xxx xxxxxxxx xxxxxxxx$ xxxx xx xxx xxxxx xxx xxxx xxx xxx xxxxxxx xx xxx xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxx$Xxxxx xxxxxx$ xxxxx xxx xxxxxxxx xxxx xxx Xxxxxx00 xxxxxxxx xxx xxxxx xx xxx xxxxxxx.

Xxxxxxxx xx xx xxx xxxxxxx$ xxx Xxxx$Xxxxx xxxxxxx xxxxxxxx xxxx xx x xxxxxx xxxxxxx xx xxx xxxxxxxx xxxx xxxxx xxx xxxxxxx xxx xxxxxxxx.
Xxxxxxx XxxxxXxxxx xxxxxxx x xxxxxxx xxxx xxxxxxxxxxx xxxx xx xxxxxx xx xxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>export-pssession -session $s -AllowClobber -outputModule AllCommands
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxxxx xxx xxx xxxxxxxxxx xxxx xxxx xxx XXXxxxxxx xx xxx $x xxxxxxxx xxxx xxx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx XxxxxXxxxxxx xxxxxxxxx xx xxxxxxx xxxxxxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$options = New-PSSessionOption -NoMachineProfile
PS C:\>$s = new-pssession -computername Server01 -sessionoption $options
PS C:\>export-pssession -session $s -outputModule Server01
PS C:\>remove-pssession $s
PS C:\>new-pssession -computername Server01 -sessionoption $options
PS C:\>import-module Server01
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx xxxxxxxx xxxxxxxx xx x xxxxxxx xxxx xxxxxxxxxx xxxxxxx xxxx xxx XXXxxxxxx xxxx xxxxx xxx xxxxxxxx xxxx xxxxxxxx xx xxxxxx.

Xxxx xxx xxx Xxxxxx$XXXxxxxxx$ xx xxxxx xxxxxxxxxxx xxxxx xxx xxxxxxxx XXXxxxxxx xx xxx xxxxxx xxxx xx xxxxxxx.
Xxxx xxx xxxxxx xxx xxxxxx$ xx xxx xxxxxxxx xxxxxx xxxxxxx xx xxxxxx$ xxx xxxxxx xxxx xxx xxx xxxx xxxxxx xxxxxxx xxxx xxxxxxxx xx xxxxxxxxxxx xxxxxxxx.

Xx xxx xxxxxxx xxxxxxx xxxx xxx xxxxxxx x xxxxxx xxxxxxx xx xxx xxxxxxxxxxx xxxxxxxx$ xxx xxxxxxxx xx xxx xxxxxx xxxx xx$xxxxxxxxx x xxxxxxx xx xxxx xxxxxxxx.
Xxxxxxx$ Xxxxxx$XXXxxxxxx xxxx xxx xxxx xxxxxxx xxxxxxx$ xxxx xx xxxxx xxx xx xxxxx xxx XxxxxxxXxxxxx xxxxxxxxx xx Xxx$XXXxxxxxx$ xx xxx xxxxxx.

Xxxxxxxxx$ xx xxx xxxx xx xxx xxx xxxxxxxx xxxxxxxx xx x xxxxxx xxxxxxx xxxx xxxxxxxxxx xxxxxxx$ xxx xxxx xx xxxxxx x xxxxxx xxxxxxx xxxx xxx xxxxxxx xxxx xxx xxxx xxxxxx xxx xxxxxx xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XXXxxxxxxXxxxxx xxxxxx xx xxxxxx x XXXxxxxxxXxxxxx xxxxxx$ xxx xx xxxxx xxx xxxxxx xx xxx $xxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx x XXXxxxxxx xxxx xxxxxxxx xxx xxxxxxxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx Xxx$XXXxxxxxx xxxxxx xx xxxxxx x XXXxxxxxx xx xxx Xxxxxx00 xxxxxxxx.
Xx xxxx xxx XxxxxxxXxxxxx xxxxxxxxx xx xxxxxx xxx xxxxxx xxxxxx xx $xxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxx$XXXxxxxxx xxxxxx xx xxxxxx xxxxxxxx xxxx xxx XXXxxxxxx xx $x xx xxx Xxxxxx00 xxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxx$XXXxxxxxx xxxxxx xx xxxxxx xxx XXXxxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XXXxxxxxx xxxxxx xx xxxxxx x xxx XXXxxxxxx xxxx xxxxxxxx xx xxx Xxxxxx00 xxxxxxxx.
Xxxx XXXxxxxxx xxxx xxxx xxx xxxxxxx xxxxxxx xx xxx $xxxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxxx$Xxxxxx xxxxxx xx xxxxxx xxx xxxxxxxx xxxx xxx Xxxxxx00 xxxxxx.
Xxx xxxxxxxx xx xxx xxxxxx xxx xx xxx XXXxxxxxx xx xxx Xxxxxx00 xxxxxxxx.

## XXXXXXXXXX

### $XxxxxXxxxxxx
Xxxxxxx xxx xxxxxxxxx xxxxxxxx$ xxxx xx xxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.

Xx xxx xxxxxx x xxxxxxx xxxx xxx xxxx xxxx xx x xxxxxxx xx xxx xxxxxxx xxxxxxx$ xxx xxxxxxxx xxxxxxx xxxxx xx xxxxxxxx xxx xxxxxxxx xxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxxxxxxx.

Xxxxxx$XXXxxxxxx xxxx xxx xxxxxx xxxxxxxx xxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxxxxxx xx xxxxxxxx xx xxxxxxx xxxxxxx xxxx xxxxxxxxx.

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

### $XxxxxxxxXxxx
Xxxxxxx xxx xxxxxxx xx xxx xxxxxxx xxxx xxxxxxx xxxx xxxxx xxx xxxxxxxxx xxxxxxxxx $xxxxxxxxx xxxxxx$.

Xxx xxxxxxx$ xx xxxxxx xxx xxxxxxx xx xxx Xxx$Xxxx xxxxxxx xx xxx xxxxxxxxxxx $Xxxx$$ xxxxx xx xxx XXXxxxxxx xx $x$ xxxx $xxxxxx$xxxxxxxxx $xxxxxxx $x $xxxxxxx xxx$xxxx $xxxxxxxxxxxx xxxx$$.

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

### $XxxxxxxXxxx
Xxxxxxx xxxx xxx xxxxxxxx xxxx xxx xxxxxxxxx xxxxx xx xxxx xxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx.
Xxx $XxxxxxxXxxx$ xx xxx xxxxx$ $Xxxx$.

Xx xxxxxxx$ Xxxxxx$XXXxxxxxx xxxxxxx xxx xxxxxxxx xxxx xxx XXXxxxxxx xxxxxx xxx xxxxxxxx xxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xxxx xxxxxxxx xxxxxxxx xxxxxxxx xxxx xxxxxx xx xxxxxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxx.
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

### $XxxxxxxXxxx
Xxxxxxx xxxx xxx xxxxxxxxx xxxxx xx xxxxxxx xxxxxxx.
Xxx $XxxxxxxXxxx$ xx xxx xxxxx$ $Xxxx$.

Xxxxx xxxxxx xxx$

$$ Xxxxx$ Xxx Xxxxxxx XxxxxXxxxx xxxxxxx xx xxx xxxxxxx xxxxxxx.
$$ Xxx$ Xxx xxxxxxx xxxxx. Xx xx xxx xxxxxxxxxx xx $xxx$xxxxxxx $$.
$$ Xxxxxxxxxxx$ Xxx xxxxx xxxxx xxxx Xxxxxxx XxxxxXxxxx xxxxx xx xxxxx xxxxxx xx xxx Xxxx xxxxxxxxxxx xxxxxxxx $$xxx$xxxx$$ xxxxxxxxx .xxx$ .xxx$ xxx .xxx xxxxx.
$$ Xxxxxx$ Xxx xxxxxxx xx xxx xxxxxxx xxxxxxx. $Xxxxxx$ xx xxx xxxxxxx.
$$ XxxxxxxxXxxxxx$ Xxx .xx0 xxxxx xx xxx xxxxx xxxxxx xx xxx Xxxx xxxxxxxxxxx xxxxxxxx $$xxx$xxxx$.
$$ Xxxxxx xxx Xxxxxxxx$ Xxx Xxxxxxx XxxxxXxxxx xxxxxxxxx.
$$ Xxxxxx$ Xxxxxx xxxxxx xx xxx xxxxxxx xxxxxxx.

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

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxxxxx xxx xxx xxxxxx xxxxx.
Xxxxx xxxxxx xxx $Xxxxxxx$$ $XXX0$$ $XXX0$$ $XXXXX$$ $XXX00$$ $XxxXxxxxxXxxxxxx$$ $Xxxxxxx$$ xxx $XXX$.
Xxx xxxxxxx xx $XXX$0$.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: Unicode, UTF7, UTF8, ASCII, UTF32, BigEndianUnicode, Default, OEM

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxx
Xxxxxxxxxx xxx xx xxxx xxxxxxxx xxxxxx xxxxx$ xxxx xx xxx xxxx xxx xxx xxxx$xxxx xxxxxxxxx.

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

### $XxxxxxXxxxXxxx
Xxxxxxx xxxxxxxxxx xxxxxxxxxxxx xxxx xxx xxx xxxxxxxxx Xxxxxxxxx .XXX Xxxxxxxxx xxxxx.
Xxxxx xxx xxxx xxxxx.
Xx xxxxxxx$ Xxxxxx$XXXxxxxxx xxxxxxx xxxxxxxxxx xxxxxxxxxxxx xxx xxx .XXX Xxxxxxxxx xxxxx xxxx xxx xxx xx xxx Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx xxxxxxxxx.

Xxx xxxxx xx xxxx xxxxxxxxx xxxx xx xxx xxxx xx x xxxx xxxx xx xxxxxxxx xx x Xxx$XxxxxxXxxx xxxxxxx xx xxx xxxxxxx xxxx xxxxx xxx xxxxxxxx xxx xxxxx xxxxxxxx.
Xx xxx xxx xx xxx xxxxxxxxxx xxxx xx xxx xxxxxx xxxxxxx$ xxxx $.

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

### $XxxxxXxxxxxxxxXxxxxx
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

### $XxxxxxxxxxxXxxxxx
Xx xxx xxxxxx x xxxxxxx xxxx xxx xxxx xxxx xx x xxxxxxx xx xxx xxxxxxx xxxxxxx$ xxx xxxxxxxx xxxxxxx xxxxx xx xxxxxxxx xxx xxxxxxxx xxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxxxxxxx.

Xxxxxx$XXXxxxxxx xxxx xxx xxxxxx xxxxxxxx xxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxxxxxx xx xxxxxxxx xx xxxxxxx xxxxxxx xxxx xxxxxxxxx.

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
Xx xxx xxxxxx x xxxxxxx xxxx xxx xxxx xxxx xx x xxxxxxx xx xxx xxxxxxx xxxxxxx$ xxx xxxxxxxx xxxxxxx xxxxx xx xxxxxxxx xxx xxxxxxxx xxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxxxxxxx.

Xxxxxx$XXXxxxxxx xxxx xxx xxxxxx xxxxxxxx xxxx xxxx xxx xxxx xxxxx xx xxxxxxxx xx xxx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxxxxxx xx xxxxxxxx xx xxxxxxx xxxxxxx xxxx xxxxxxxxx.

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

### $Xxxxxx
Xxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxxxxxx Xxxxxxx XxxxxXxxxx xxxx$xxx xxx xxxxxxx.
Xxxxx xxx xxxx$xx xxx xxxxxx xxxxx.
Xxxxxxxxx xxx xxx xxxxxxxxx.

Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$XXXxxxxxx xxx Xxxxxx$Xxxxxx.

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

### $XxxxxxXxxxxx
Xxxxxxxxx x xxxx $xxxxxxxx$ xxx xxxx xxx xxx xxxxxx xxxx Xxxxxx$XXXxxxxxx xxxxxxx.
Xxx xxxxxxx xxxx xx $xxxx$Xxxxxxxxx$XxxxxxxXxxxxXxxxx$Xxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx.

Xx xxx xxxxxx xxxxxxxxxxxx xx xxx xx xxx xxxxx xxxx Xxxxxx$XXXxxxxxx xxxxxxx xxxxxxx xxxxx$ xxx xxxxxxx xxxxx.
Xx xxxxxxxxx xxxxxxxx xxxxx$ xxx xxx Xxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: PSPath, ModuleName

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxx
Xxxxxxxxx xxx XXXxxxxxx xxxx xxxxx xxx xxxxxxxx xxx xxxxxxxx. Xxxxx x xxxxxxxx xxxx xxxxxxxx x xxxxxxx xxxxxx xx x xxxxxxx xxxx xxxx x xxxxxxx xxxxxx$ xxxx xx x Xxx$XXXxxxxxx xxxxxxx.
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

### $Xxxxxxxxxxx
Xxxxxxxxx xxx xxxxxx xxxxxxxxxxx xxxx xx xxxx xx xxxx xxx xxxxxx xxxxx $$.Xxxxxx.xx0xxx$ xx xxxxxx xxxxxx xxxxx $.xxx0$ xx xxx xxxxxx xxxx Xxxxxx$XXXxxxxxx xxxxxxx.
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

### Xxxx
Xxx xxxxxx xxxx xxxxxxx xx Xxxxxx$XXXxxxxxx.

## XXXXXXX

### Xxxxxx.XX.XxxxXxxx
Xxxxxx$XXXxxxxxx xxxxxxx x xxxx xx xxxxx xxxx xxxxxxxx xxx xxxxxx xxxx xx xxxxxxx.

## XXXXX
Xxxxxx$XXXxxxxxx xxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx xxxxxxxxxxxxxx.
Xx xxx xxxx xxxxxx$ xxx xxxxxxxx xxxx xx xxxxxxxxxx xxx xxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxx$Xxxxxxxxxxxx.

Xxx xxxxxx xxx Xxxxxx$XXXxxxxxx xx xxxxxx x Xxxxxxx XxxxxXxxxx xxxxxxxx.

Xxxxxxxx xxxxxxxx xxx xxxxxxxxxx xx xxx XXXxxxxxx xxxx xxxxx xxxx xxxx xxxxxxxx.
Xxxxxxx$ xxx xxxxxxx xx xxxxxxx xxx xxxxxxxx xxxxxxxx xxx xxxxxxx xxxxxxxx xx Xxxxxxx XxxxxXxxxx.
Xxx xxx xxx xxx xxxxxxxx xxxxxxxx xxxx xx xxx xxxxx xxx xxxxx xxxxxxxx.

Xxxxxx$Xxxxxx xxxxxxxx xxx xxxxx xxxxxxxxxxx xxxxx xxx XXXxxxxxx xx xxx xxxxxx xxxx xx xxxxxxx.
Xx xxx XXXxxxxxx xxxx xxxxx xxx xxxxxxxx xxxx xxxxxxxx xx xxxxxx xxxx xxx xxxxxx xxx xxxxxx$ xxx xxxxx xxx xx xxxxxx XXXxxxxxxx xx xxx xxxx xxxxxxxx$ xxx xxxxxxxx xx xxx xxxxxx xxxxxxx xx xx$xxxxxx xxx XXXxxxxxx.
Xx xxxxxxxx xx xx$xxxxxx xxx XXXxxxxxx xxxx$ xxx xxxxxxxx xxxxxxxx xxxx xxx xxx.

Xxx xxxxxxx xxxxxxxxxxx xxxx Xxxxxx$Xxxxxx xxxxxxxx xxx xxxxx xx xxx xxxxxx xxxx xxx xxxxxxx xxxxxxx xxxxxxx$ xxxx xx xxxxx xxxx xxx xxxxxxx xx xxx $XXXxxxxxxXxxxxx xxxxxxxxxx xxxxxxxx xx xx xxxxx xxx XxxxxxxXxxxxx xxxxxxxxxx xx  xxx Xxx$XXXxxxxxx$ Xxxxx$XXXxxxxxx$ xx Xxxxxx$Xxxxxxx xxxxxx.
Xx xxx xxxxxxxx XXXxxxxxx xx xxxxxx xxxx xxx xxxxxx xxx xxxxxx$ xxx xxxxxx xxxx xxx xxxxxxx XXXxxxxxx xx xxx xxxx xxxxxxxx$ xx xxx xx xxxxxxxxx.
Xx xxxxxx xxx xxxxxxxx xxxxxxxx xx xxx xx x xxxxxxxxx xxxxxxxxxx xxxxxxx$ xxxxxx x XXXxxxxxx xxxx xxx xxxxxxx xxxx xxx xxxx xxxxxx xxx xxxxxx xxx xxxxxx.

Xx xxxx xxx xxxxxxxx xx xxxxxx$ Xxxxxx$XXXxxxxxx xxxx xxx Xxxxxx$Xxxxxxx xxxxxx xx xxx x Xxx$Xxxxxxx xxxxxxx xx xxx XXXxxxxxx.
Xx xxx xxx xxxx xxxxxxxxxx xxxx xxx xxx xxxxxxxx$ xx xxxx xxx Xxx$XxxxxxXxxx xxx Xxxxxx$XxxxxxXxxx xxxxxxx.
Xxx xxxxx xxx xxxxx xxxxxxxx xxxx Xxxxxx$Xxxxxxx$ Xxx$Xxxxxxx$ Xxx$XxxxxxXxxx$ xxx Xxxxxx$XxxxxxXxxx xxxx xxx xxx xx Xxxxxx$XXXxxxxxx xxxxxxx.
Xxxx$ Xxxxxx$XXXxxxxxx xxxxxx xxxxxx xxxxxxxx xxxx x xxxxxxx xxxx xxxx xxx xxxxxxx xxx Xxx$Xxxxxxx$ Xxx$XxxxxxXxxx$ Xxxxxx$Xxxxxx$ xxx Xxx$Xxxx xxxxxxx.

Xxxxxx$XXXxxxxxx xxxx xxx Xxxxx$Xxxxxxxx xxxxxx xx xxxxxxx xxx xxxxxxxx xx xxx xxxxxxx.
Xxx xxxxx xxx xxx xxxxxxxx xxx xxxxx xxx xxxxxxx xx xxxxxxx.

Xxxxxxxx xxxxxxxx xxxx xxx xxxx xxxxxxxxxxx xx xxxxx xxxxxx xxxxxxxx$ xxxxxxxxx xxx xxxxxxxxx xx xxxxx x xxxxxxx xxxx x xxxx xxxxxxxxx$ xxxx xx Xxxxxxx.

Xxxxxxx Xxxxxxx XxxxxXxxxx xxxxxxxx xxx xxx xxx xx XXXxxxxxxx$ xxx xxxxxxxx xxxx x xxxxxxx xxxx xx x xxxxxxx xxx xxx xxxxxxxxx xx Xxxxxx$XXXxxxxxx.
Xx xxxxxx xxxxxxxx xxxx x xxxxxxx$ xxx xx Xxxxxx$Xxxxxxx xxxxxxx xx xxx xxx xxxxxxx xx xxx XXXxxxxxx xxxxxxxx xxxxxx xxxxxxxxx xxxxxxxx.

Xxx xxxxxx xxxx Xxxxxx$XXXxxxxxx xxxxxxx xxxxx xxxxxxx x xxxxxxxxxx xxxx$ xxxx xx xxx xxxxxxx xxxx xxx xxxxxx xxxxxxxxxx xxxx.
Xx xxx xxxxxxx xxxx xxx xxxxxx xxxxxxxxxx xxxx$ xxx xxxxxxxxxx xxxxx xxxx xxx xxxxxxx xxxx xxx xxxxxxx xxxxxxxxxx xxxx.

## XXXXXXX XXXXX

[Xxxxxx$Xxxxxx]()

[Xxxxxx$XXXxxxxxx]()

[Xxxxxx$Xxxxxxx]()

[Xxx$XXXxxxxxx]()

