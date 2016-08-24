---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293973
schema: 2.0.0
---

# Xxx$XXXxxxXxxxx
## XXXXXXXX
Xxxxxxxx xxx xxxxxxx xxxx xxxxx.

## XXXXXX

```
Get-PSCallStack [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$XXXxxxXxxxx xxxxxx xxxxxxxx xxx xxxxxxx xxxx xxxxx.

Xxxxxxxx xx xx xxxxxxxx xx xx xxxx xxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx$ xxx xxx xxx xxxx xxxxxx xx xxxxxxx xxx xxxx xxxxx xx x xxxxxx xx xxxxxxxx xxxxxxx xx xxx xxxxxxxx.

Xx xxx x Xxx$XXXxxxXxxxx xxxxxxx xxxxx xx xxx xxxxxxxx$ xxxx $x$ xx $xxx$xxxxxxxxxxx$.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>function my-alias {
$p = $args[0]
get-alias | where {$_.definition -like "*$p"} | ft definition, name -auto
}
PS C:\ps-test> set-psbreakpoint -command my-alias

Command    : my-alias
Action     :
Enabled    : True
HitCount   : 0
Id         : 0
Script     : prompt

PS C:\ps-test> my-alias get-content

Entering debug mode. Use h or ? for help.
Hit Command breakpoint on 'prompt:my-alias'
my-alias get-content
[DBG]: PS C:\ps-test> s
$p = $args[0]
DEBUG: Stepped to ':    $p = $args[0]    '
[DBG]: PS C:\ps-test> s
get-alias | Where {$_.Definition -like "*$p*"} | ft Definition,
[DBG]: PS C:\ps-test>get-pscallstack
Name        CommandLineParameters         UnboundArguments              Location
----        ---------------------         ----------------              --------
prompt      {}                            {}                            prompt
my-alias    {}                            {get-content}                 prompt
prompt      {}                            {}                            prompt
[DBG]: PS C:\ps-test> o
Definition  Name
----------  ----
Get-Content gc
Get-Content cat
Get-Content type
```

Xxxxxxxxxxx

-----------

Xxxx xxxxxxx xxxx xxx Xxx$XXXxxxXxxxx xxxxxx xx xxxxxxx xxx xxxx xxxxx xxx Xx$Xxxxx$ x xxxxxx xxxxxxxx xxxx xxxx xxx xxxxxxx xxx x xxxxxx xxxx.

Xxx xxxxx xxxxxxx xxxxxx xxx xxxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxx.
Xxx xxxxxx xxxxxxx xxxx xxx Xxx$XXXxxxxxxxxx xxxxxx xx xxx x xxxxxxxxxx xx xxx Xx$Xxxxx xxxxxxxx.
Xxx xxxxx xxxxxxx xxxx xxx Xx$Xxxxx xxxxxxxx xx xxx xxx xx xxx xxxxxxx xx xxx xxxxxxx xxxxxxx xxx xxx Xxx$Xxxxxxx xxxxxx.

Xxx xxxxxxxx xxxxxx xx xx xxx xxxxxxxx xxxx.
Xxx xxxxxxxxxxx xxxx$xxxx $x$ xxxxxxxx xxxxx xxxxxxxxx xxx xxxxxxxx xxxx xx xxxx.
Xxxx$ x Xxx$XXXxxxXxxxx xxxxxxx xx xxxx xx xxxxxxxx xxx xxxx xxxxx.

Xxx xxxxx xxxxxxx xx x Xxxx$Xxx xxxxxxx $x$ xxxx xxxxx xxx xxxxxxxx xxx xxxxxxxxx xxxxxxxxx xxx xxxxxx xx xxxxxxxxxx.

## XXXXXXXXXX

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

## XXXXXX

### Xxxx
Xxx xxxxxx xxxx xxxxxxx xx xxxx xxxxxx.

## XXXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XxxxXxxxxXxxxx
Xxx$XXXxxxXxxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxx xx xxx xxxx xxxxx.

## XXXXX

## XXXXXXX XXXXX

[Xxxxxxx$XXXxxxxxxxxx]()

[Xxxxxx$XXXxxxxxxxxx]()

[Xxx$XXXxxxxxxxxx]()

[Xxxxxx$XXXxxxxxxxxx]()

[Xxx$XXXxxxxxxxxx]()

[xxxxx$Xxxxxxxxx]()

