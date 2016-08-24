---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293995
schema: 2.0.0
---

# Xxx$Xxxxxxxx
## XXXXXXXX
Xxxxxxx x xxx xxxxxxxx.

## XXXXXX

```
New-Variable [-Name] <String> [[-Value] <Object>] [-Description <String>] [-Option <ScopedItemOptions>]
 [-Visibility <SessionStateEntryVisibility>] [-Force] [-PassThru] [-Scope <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxxxx xxxxxx xxxxxxx x xxx xxxxxxxx xx Xxxxxxx XxxxxXxxxx.
Xxx xxx xxxxxx x xxxxx xx xxx xxxxxxxx xxxxx xxxxxxxx xx xx xxxxxx xx xxxxxx xxx xxxxx xxxxx xx xx xxxxxxx.

Xxx xxx xxx xxx xxxxxxxxxx xx Xxx$Xxxxxxxx xx xxx xxx xxxxxxxxxx xx xxx xxxxxxxx $xxxx xx xxxxx xxxx xxxxxx xxxx$xxxx xx xxxxxxxx xxxxxxxxx$$ xxx xxx xxxxx xx x xxxxxxxx$ xxx xxxxxxxxx xxxxxxx xxxxxxxxx xxx xxxxxx xx xxxxxxx.

Xxxxxxxxx$ xxx xxxxxx x xxx xxxxxxxx xx xxxxxx xxx xxxxxxxx xxxx xxx xxx xxxxx$ xxxx xx $$xxx $ 0$$ xxx xxx xxx xxx xxx Xxx$Xxxxxxxx xxxxxx xx xxx xxx xxxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>new-variable days
```

Xxxx xxxxxxx xxxxxxx x xxx xxxxxxxx xxxxx $xxxx$.
Xx xxx xx xxxxx xxxxxxxxxxx xxxxxxxxx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>new-variable zipcode -value 98033
```

Xxxx xxxxxxx xxxxxxx x xxxxxxxx xxxxx $xxxxxxx$ xxx xxxxxxx xx xxx xxxxx $00000$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>new-variable -name max -value 256 -option readonly
PS C:\>new-variable -name max -value 1024

New-Variable : A variable with name 'max' already exists.
At line:1 char:13
+ new-variable <<<<  -name max -value 1024

PS C:\>new-variable -name max -value 1024 -force
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx XxxxXxxx xxxxxx xx Xxx$Xxxxxxxx xx xxxxxxx x xxxxxxxx xxxx xxxxx xxxxxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxx xxxxxxxx xxxxx Xxx xxx xxxx xxx xxxxx xx $000$.
Xx xxxx xxx Xxxxxx xxxxxxxxx xxxx x xxxxx xx XxxxXxxx.

Xxx xxxxxx xxxxxxx xxxxx xx xxxxxx x xxxxxx xxxxxxxx xxxx xxx xxxx xxxx.
Xxxx xxxxxxx xxxxxxx xx xxxxx$ xxxxxxx xxx xxxx$xxxx xxxxxx xx xxx xx xxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxxxx xxxxxxxxx xx xxxxxxxx xxx xxxx$xxxx xxxxxxxxxx xx xxx xxxxxxxx.
Xx xxxx xxxx$ xxx xxxxxxx xx xxxxxx x xxx xxxxxxxx xxxx xxx xxxx xxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>new-variable -name counter -visibility private

#Effect of private variable in a module.

PS C:\>get-variable c*

Name                           Value
----                           -----
Culture                        en-US
ConsoleFileName
ConfirmPreference              High
CommandLineParameters          {}

PS C:\>$counter

"Cannot access the variable '$counter' because it is a private variable"

PS C:\>Get-Counter

Name         Value
----         -----
Counter1     3.1415
...
```

Xxxx xxxxxxx xxxxxxxxxxxx xxx xxxxxxxx xx x xxxxxxx xxxxxxxx xx x xxxxxx.
Xxx xxxxxx xxxxxxxx xxx Xxx$Xxxxxxx xxxxxx$ xxxxx xxx x xxxxxxx xxxxxxxx xxxxx $Xxxxxxx$.
Xxx xxxxxxx xxxx xxx Xxxxxxxxxx xxxxxxxxx xxxx x xxxxx xx $Xxxxxxx$ xx xxxxxx xxx xxxxxxxx.

Xxx xxxxxx xxxxxx xxxxx xxx xxxxxxxx xx x xxxxxxx xxxxxxxx.
Xxx xxxx xxx xxx xxxxxx xxx xxxxxx xxxxxx xxxx xx xxxxxx xxx xxxxx xx xxx Xxxxxxx xxxxxxxx$ xxx xxx Xxxxxxx xxxxxxxx xxx xx xxxx xxx xxxxxxx xx xxx xxxxxxxx xx xxx xxxxxx.

## XXXXXXXXXX

### $Xxxxxxxxxxx
Xxxxxxxxx x xxxxxxxxxxx xx xxx xxxxxxxx.

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
Xxxxxx xxx xx xxxxxx x xxx xxxxxxxx xxxx xxx xxxx xxxx xx xx xxxxxxxx xxxx$xxxx xxxxxxxx.

Xx xxxxxxx$ xxx xxx xxxxxxxxx x xxxxxxxx xxxxxx xxx xxxxxxxx xxx xx xxxxxx xxxxx xx XxxxXxxx xx Xxxxxxxx.
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
Xxxxxxxxx x xxxx xxx xxx xxx xxxxxxxx.

```yaml
Type: String
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
Xxxxxxxxxx xxx xxxxx xx xxx xxx xxxxxxxx.
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
Xxxxxxxxx xxx xxxxxxx xxxxx xx xxx xxxxxxxx.

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
Xxx xxx xxxx x xxxxx xx Xxx$Xxxxxxxx.

## XXXXXXX

### Xxxx xx Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxxxx
Xxxx xxx xxx xxx XxxxXxxx xxxxxxxxx$ Xxx$Xxxxxxxx xxxxxxxxx x Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxxxx xxxxxx xxxxxxxxxxxx xxx xxx xxxxxxxx.
Xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX

## XXXXXXX XXXXX

[Xxxxx$Xxxxxxxx]()

[Xxx$Xxxxxxxx]()

[Xxxxxx$Xxxxxxxx]()

[Xxx$Xxxxxxxx]()

