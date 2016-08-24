---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294015
schema: 2.0.0
---

# Xxx$Xxxxxxxx
## XXXXXXXX
Xxxx xxx xxxxx xx x xxxxxxxx.
Xxxxxxx xxx xxxxxxxx xx xxx xxxx xxx xxxxxxxxx xxxx xxxx xxx xxxxx.

## XXXXXX

```
Set-Variable [-Name] <String[]> [[-Value] <Object>] [-Include <String[]>] [-Exclude <String[]>]
 [-Description <String>] [-Option <ScopedItemOptions>] [-Force] [-Visibility <SessionStateEntryVisibility>]
 [-PassThru] [-Scope <String>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxxxx xxxxxx xxxxxxx x xxxxx xx x xxxxxxxxx xxxxxxxx xx xxxxxxx xxx xxxxxxx xxxxx.
Xx xxx xxxxxxxx xxxx xxx xxxxx$ xxx xxxxxx xxxxxxx xx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-variable -name desc -value "A description"
PS C:\>get-variable -name desc
```

Xxxxx xxxxxxxx xxx xxx xxxxx xx xxx $xxxx$ xxxxxxxx xx $X xxxxxxxxxxx$$ xxx xxxx xxx xxx xxxxx xx xxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>set-variable -name processes -value (Get-Process) -option constant -scope global -description "All processes" -passthru | format-list -property *
```

Xxxx xxxxxxx xxxxxxx x xxxxxx$ xxxx$xxxx xxxxxxxx xxxx xxxxxxxx xxx xxxxxxxxx xx xxx xxxxxx$ xxx xxxx xx xxxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxxx.

Xxx xxxxxxx xxxx xxx Xxx$Xxxxxxxx xxxxxx xx xxxxxx xxx xxxxxxxx.
Xx xxxx xxx XxxxXxxx xxxxxxxxx xx xxxxxx xx xxxxxx xxxxxxxxxxxx xxx xxx xxxxxxxx$ xxx xx xxxx xxx xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xx xxx Xxxxxx$Xxxx xxxxxx.
Xx xxxx xxx Xxxxxxxx xxxxxxxxx xx Xxxxxx$Xxxx xxxx x xxxxx xx xxx $$$ xx xxxxxxx xxx xxxxxxxxxx xx xxx xxxxx xxxxxxx xxxxxxxx.

Xxx xxxxx$ $$Xxx$Xxxxxxx$$$ xx xxxxxxxx xx xxxxxxxxxxx xx xxxxxx xxxx xx xx xxxxxxxx xxxxxx xxxxx xxxxxx xx xxx xxxxxxxx.
Xxxxxxxxx$ xxx xxxxxxxx xxxxxxxx xxx xxxxx $Xxx$Xxxxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\># set-variable -name counter -visibility private
PS C:\>new-variable -name counter -visibility public -value 26
PS C:\>$counter
26
PS C:\>get-variable c*

Name Value
---- -----
Culture en-US
ConsoleFileName
ConfirmPreference High
CommandLineParameters {}
Counter 26

PS C:\>set-variable -name counter -visibility private
PS C:\>get-variable c*

Name Value
---- -----
Culture en-US
ConsoleFileName
ConfirmPreference High
CommandLineParameters {}
PS C:\>$counter

"Cannot access the variable '$counter' because it is a private variable"

PS C:\>.\use-counter.ps1
#Commands completed successfully.
```

Xxxx xxxxxxx xxxxx xxx xx xxxxxx xxx xxxxxxxxxx xx x xxxxxxxx xx $Xxxxxxx$.
Xxxx xxxxxxxx xxx xx xxxx xxx xxxxxxx xx xxxxxxx xxxx xxx xxxxxxxx xxxxxxxxxxx$ xxx xx xx xxx xxxxxxx xx xxx xxxx.

Xxx xxxxxx xxxxxx xxxxx xxx xxxxxxxxxx xx xxx xxxxxxxx xx xxxxxx xxx xxxxxxx xxxxxxxxx.

## XXXXXXXXXX

### $Xxxxxxxxxxx
Xxxxxxxxx xxx xxxxxxxxxxx xx xxx xxxxxxxx.

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

### $Xxxxxxx
Xxxxx xxx xxxxxxxxx xxxxx.
Xxx xxxxx xx xxxx xxxxxxxxx xxxxxxxxx xxx Xxxx xxxxxxxxx.
Xxxxx x xxxx xxxxxxx xx xxxxxxx$ xxxx xx $$.xxx$.
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

### $Xxxxx
Xxxxxx xxx xx xxxxxx x xxxxxxxx xxxx xxx xxxx xxxx xx xx xxxxxxxx xxxx$xxxx xxxxxxxx$ xx xx xxxxxx xxx xxxxx xx x xxxx$xxxx xxxxxxxx.

Xx xxxxxxx$ xxx xxx xxxxxxxxx x xxxxxxxx$ xxxxxx xxx xxxxxxxx xxx xx xxxxxx xxxxx xx $XxxxXxxx$ xx $Xxxxxxxx$.
Xxx xxxx xxxxxxxxxxx$ xxx xxx Xxxxxx xxxxxxxxx.

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

### $Xxxxxxx
Xxxxxxx xxxx xxx xxxxxxxxx xxxxx.
Xxx xxxxx xx xxxx xxxxxxxxx xxxxxxxxx xxx Xxxx xxxxxxxxx.
Xxxxx x xxxx xx xxxx xxxxxxx$ xxxx xx $x$$.
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

### $Xxxx
Xxxxxxxxx xxx xxxxxxxx xxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxx
Xxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxxxx.

Xxxxx xxxxxx xxx$

$$ Xxxx$ Xxxx xx xxxxxxx. $$Xxxx$ xx xxx xxxxxxx.$ $$ XxxxXxxx$ Xxx xx xxxxxxx. Xxxxxx xx xxx xxxxxxx$ xxxxxx xx xxxxx xxx Xxxxx xxxxxxxxx.
$$ Xxxxxxxx$ Xxxxxx xx xxxxxxx xx xxxxxxx. $Xxxxxxxx$ xx xxxxx xxxx xxxx xxx xxx xxxxxxxx x xxxxxxxx. Xxx xxxxxx xxxxxx xxx xxxxxxx xx xx xxxxxxxx xxxxxxxx xx $Xxxxxxxx$.
$$ Xxxxxxx$ Xxx xxxxxxxx xx xxxxxxxxx xxxx xx xxx xxxxxxx xxxxx.
$$ XxxXxxxx$ Xxx xxxxxxxx xx xxxxxx xx xxx xxx xxxxxx xxxx xxx xxxxxxx.

Xx xxx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxxxxx xx xxx xxxxxxx$ xxxx $xxx$xxxxxxxx $ xxxxxx$xxxxx $xxxxxxxx xxxx$ xxxxxxx $xxxxxxxx$.

```yaml
Type: ScopedItemOptions
Parameter Sets: (All)
Aliases: 
Accepted values: None, ReadOnly, Constant, Private, AllScope, Unspecified

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxxxxx xx xxxxxx xxxxxxxxxxxx xxx xxx xxxxxxxx.
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

### $Xxxxx
Xxxxxxxxxx xxx xxxxx xx xxx xxxxxxxx.
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

### $Xxxxx
Xxxxxxxxx xxx xxxxx xx xxx xxxxxxxx.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### $Xxxxxxxxxx
Xxxxxxxxxx xxxxxxx xxx xxxxxxxx xx xxxxxxx xxxxxxx xx xxx xxxxxxx xx xxxxx xx xxx xxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx xxx  xxx xx xxxxxxx xxx xxxxxxxx xxxx xxxx xx xxxxxxxxx xx xxxxx xxxxx.

Xxxxx xxxxxx xxx$

$$ Xxxxxx$  Xxx xxxxxxxx xx xxxxxxx. $$Xxxxxx$ xx xxx xxxxxxx.$ $$ Xxxxxxx$ Xxx xxxxxxxx xx xxx xxxxxxx.

Xxxx x xxxxxxxx xx xxxxxxx$ xx xxxx xxx xxxxxx xx xxxxx xx xxxxxxxxx$ xxxx xx xxxxx xxxxxxxx xx Xxx$Xxxxxxxx$ xx xx xxxxxxxx xx xxx Xxxxxxxx$ xxxxx.
Xxxxxxxx xx xxxx xx xxxxxx xxx xxxxx xx x xxxxxxx xxxxxxxx xxxxxx xx xxxxx.
Xxxxxxx$ xxx xxxx xxx xxx xxxxxxxx xxxx xxx x xxxxxxx xxxxxxxx xx xxx xxxxxxxx xxxx xxxxxxx xx xxx xxxxxxx xx xxxxx xxx xxxxxxxx xxx xxxxxxx.

```yaml
Type: SessionStateEntryVisibility
Parameter Sets: (All)
Aliases: 
Accepted values: Public, Private

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

## XXXXXX

### Xxxxxx.Xxxxxx
Xxx xxx xxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxx xx xxx xxxxxxxx xx Xxx$Xxxxxxxx.

## XXXXXXX

### Xxxx xx Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxxxx
Xxxx xxx xxx xxx XxxxXxxx xxxxxxxxx$ Xxx$Xxxxxxxx xxxxxxxxx x Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxxxx xxxxxx xxxxxxxxxxxx xxx xxx xx xxxxxxx xxxxxxxx.
Xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX

## XXXXXXX XXXXX

[Xxxxx$Xxxxxxxx]()

[Xxx$Xxxxxxxx]()

[Xxx$Xxxxxxxx]()

[Xxxxxx$Xxxxxxxx]()

