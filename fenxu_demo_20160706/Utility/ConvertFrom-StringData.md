---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293948
schema: 2.0.0
---

# ConvertFrom-StringData
## XXXXXXXX
Xxxxxxxx x xxxxxx xxxxxxxxxx xxx xx xxxx xxx xxx xxxxx xxxxx xx x xxxx xxxxx.

## XXXXXX

```
ConvertFrom-StringData [-StringData] <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx XxxxxxxXxxx$XxxxxxXxxx xxxxxx xxxxxxxx x xxxxxx xxxx xxxxxxxx xxx xx xxxx xxx xxx xxxxx xxxxx xxxx x xxxx xxxxx.
Xxxxxxx xxxx xxx$xxxxx xxxx xxxx xx xx x xxxxxxxx xxxx$ xxxx$xxxxxxx xxx xxxxx xxxx xx xxx xxxxx xxxxxx.

Xxx XxxxxxxXxxx$XxxxxxXxxx xxxxxx xx xxxxxxxxxx xx xx x xxxx xxxxxx xxxx xxx xx xxxx xx xxx XXXX xxxxxxx xx x xxxxxx xx xxxxxxxx.
Xxxx xxxx xx x XXXX xxxxxxx$ xxx xxxxxxxx xx xxx xxxxxx xxxx xxxxxxx xx xxx xxxxx xxx x XXXX xxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxx$Xxxxxxxx.

XxxxxxxXxxx$XxxxxxXxxx xxxxxxxx xxxxxx xxxxxxxxx xxxxxxxxx xxxx xxx xxxxxxx xx xxxxxxxxxxxx xxxxxxx xxxxxxxxxxx xxxxx.
Xxxx xx$ xxx xxxxxx xxx xxxxxxxxx xxxxxxxxxxx $$$$ xx xxxxxx xxxxxxxxxx xx xxx xxxxxx xxxx xx xxxxx xxx Xxxxx.Xxxxxxxx Xxxxxx$ xxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxx xxxxxxxxx $$$$ xxxx xxxxx xxxxxxxx xxxxxx xxx xxx xx x xxxx xx x xxxxxx.
Xxxxxx xxx xxxx$xxxxxx$ xxx xxxxxxxx xxxxxxxxx xxxx xxx xxxx.
Xxx xxx xxxx xxxxxxxx x xxxxxxx xxxxxxxxx xx xxxx xxxxxxx xx xxxxxxxx xx xxxx x xxxxxxxxx xxxxxxxxx$ xxxx xxxx$  $$$$.
Xxxxxxxxx xxxxxxxxx xxxxxxxxxx$ xxxx xx xxxxx xxxx xxx xxxxxxxx xxxx xx xxxx xxxxx$ xxx xxxxxx xx xxxxxxx xxxxxx xxxxxxxxx xx xxxx xxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$here = @'
Msg1 = The string parameter is required.
Msg2 = Credentials are required for this command.
Msg3 = The specified variable does not exist.
'@
PS C:\>convertfrom-stringdata -stringdata $here

Name                           Value
----                           -----
Msg3                           The specified variable does not exist.
Msg2                           Credentials are required for this command.
Msg1                           The string parameter is required.
```

Xxxxx xxxxxxxx xxxxxxx x xxxxxx$xxxxxx xxxx$xxxxxx xx xxxx xxxxxxxx xxxx x xxxx xxxxx.
Xx x xxxxxx$xxxxxx xxxxxx$ xxxxxx xxx xxx xxxxxxxxxxx xxx xxxxxxxxx xxx xxxxxxxxxxx xxx xxx xxxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxx$xxxxxx xxx xxxxx xx xx xxx $xxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx XxxxxxxXxxx$XxxxxxXxxx xxxxxx xx xxxxxxx xxx xxxx$xxxxxx xx xxx $xxxx xxxxxxxx xx x xxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$p = @"
ISE = Windows PowerShell Integrated Scripting Environment
"@
PS C:\>$p | get-member
TypeName: System.String

Name             MemberType            Definition
----             ----------            ----------
Clone            Method                System.Object Clone()
...
PS C:\>$hash = convertfrom-stringdata -stringdata $p
PS C:\>$hash | get-member
TypeName: System.Collections.Hashtable

Name              MemberType            Definition
----              ----------            ----------
Add               Method                System.Void Add(Object key, Object
...
```

Xxxxx xxxxxxxx xxxxxxxxxxx xxxx XxxxxxxXxxx$XxxxxxXxxx xxxxxxxx xxxxxxxx x xxxx$xxxxxx xx x xxxx xxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxxxx$xxxxxx xxxx$xxxxxx xxxx xxxxxxxx xxx xxx$xxxxx xxxx xxx xxxxx xx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx $x xxxxxxxx xx xxx Xxx$Xxxxxx xxxxxx.
Xxx xxxxxx xxxxx xxxx $x xx x xxxxxx $Xxxxxx.Xxxxxx$.

Xxx xxxxx xxxxxxx xxxx xxx XxxxxxxXxxx$XxxxxxXxxx xxxxxx xx xxxxxxx xxx xxxx$xxxxxx xx $x xx x xxxx xxxxx.
Xxx xxxxxxx xxxxxx xxx xxxxxx xx xxx $xxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx $xxxx xxxxxxxx xx xxx Xxx$Xxxxxx xxxxxx.
Xxx xxxxxx xxxxx xxxx xxx xxxxxxx xx xxx $xxxx xxxxxxxx xx x xxxx xxxxx $Xxxxxx.Xxxxxxxxxxx.Xxxxxxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>convertfrom-stringdata -stringdata @'
Name = Disks.ps1

# Category is optional.

Category = Storage
Cost = Free
'@

Name                           Value
----                           -----
Cost                           Free
Category                       Storage
Name                           Disks.ps1
```

Xxxx xxxxxxx xxxxxxxx x xxxxxx$xxxxxx xxxx$xxxxxx xxxx xxxxxxxx xxxxxxxx xxx$xxxxx xxxxx xxxx x xxxx xxxxx.

Xx xxxx xxxxxxx$ xxx xxxxx xx xxx XxxxxxXxxx xxxxxxxxx xx x xxxx$xxxxxx$ xxxxxxx xx x xxxxxxxx xxxx xxxxxxxx x xxxx$xxxxxx.
Xxxxxx xxxxxx xx xxxxx.

Xxx xxxx$xxxxxx xxxxxxxx x xxxxxxx xxxxx xxx xx xxx xxxxxxx.
Xxxxxxxx xxx xxxxx xx xxxxxxx$ xxxxxxxx xxxx xxx xxxxxxx xx xx x xxxxxxxxx xxxx xxxx x xxx$xxxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = convertfrom-stringdata -stringdata "Top = Red `n Bottom = Blue"
PS C:\>"Top = " + $a.Top
Top = Red
PS C:\>"Bottom = " + $a.Bottom
Bottom = Blue
```

Xxxx xxxxxxx xxxxxxxx x xxxxxxx xxxxxx$xxxxxx xxxxxx $xxx x xxxx$xxxxxx$ xxxx x xxxx xxxxx xxx xxxxx xx xx xxx $x xxxxxxxx.

Xx xxxxxxx xxx xxxxxxxxx xxxx xxxx xxx$xxxxx xxxx xxxx xx xx x xxxxxxxx xxxx$ xx xxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xxxxxxxxx $$$x$ xx xxxxxxxx xxx xxxxx.

Xxx xxxxxx xx x xxxx xxxxx xx xxx xxxxx.
Xxx xxxxxxxxx xxxxxxxx xxxxxxx xxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$TextMsgs = DATA {
ConvertFrom-StringData @'
Text001 = The $Notebook variable contains the name of the user's system notebook.
Text002 = The $MyNotebook variable contains the name of the user's private notebook.
'@
}
PS C:\>$TextMsgs.Text001
The $Notebook variable contains the name of the user's system notebook.
PS C:\>$TextMsgs.Text002
The $MyNotebook variable contains the name of the user's private notebook.
```

Xxxx xxxxxxx xxxxx x XxxxxxxXxxx$XxxxxxXxxx xxxxxxx xxxx xx xxx XXXX xxxxxxx xx x xxxxxx.
Xxx xxxxxxxxxx xxxxx xxx XXXX xxxxxxx xxxxxxx xxx xxxx xx xxx xxxx.

Xxxxxxx xxx xxxx xxxxxxxx xxxxxxxx xxxxx$ xx xxxx xx xxxxxxxx xx x xxxxxx$xxxxxx xxxxxx xx xxxx xxx xxxxxxxxx xxx xxxxxxxxxxx xxxxxxxxx xxx xxx xxxxxxxx.
Xxxxxxxxx xxx xxx xxxxxxxxx xx xxx XXXX xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$here = @'
Msg1 = The string parameter is required.
Msg2 = Credentials are required for this command.
Msg3 = The specified variable does not exist.
'@
PS C:\>$hash = $here | convertfrom-stringdata
PS C:\>$hash

Name     Value
----     -----
Msg3     The specified variable does not exist.
Msg2     Credentials are required for this command.
Msg1     The string parameter is required.
```

Xxxx xxxxxxx xxxxx xxxx xxx xxx xxx x xxxxxxxx xxxxxxxx $$$ xx xxxx x xxxxxx xx XxxxxxxXxxx$XxxxxxXxxx.

Xxx xxxxx xxxxxxx xxxxx x xxxx$xxxxxx xx xxx $xxxx xxxxxxxx.
Xxx xxxxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx $xxxx xxxxxxxx xx XxxxxxxXxxx$XxxxxxXxxx.
Xxx xxxxxxx xxxxx xxx xxxxxx xx xxx $xxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxxx xxx xxxxxxxx xx xxx $xxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>ConvertFrom-StringData @"
Vincentio = Heaven doth with us as we with torches do,\nNot light them for themselves; for if our virtues\nDid not go forth of us, 'twere all alike\nAs if we had them not.
Angelo = Let there be some more test made of my metal,\nBefore so noble and so great a figure\nBe stamp'd upon it.
"@ | Format-List

Name  : Angelo

Value : Let there be some more test made of my metal,
        Before so noble and so great a figure
        Be stamp'd upon it. 

Name  : Vincentio
Value : Heaven doth with us as we with torches do, 
        Not light them for themselves; for if our virtues
        Did not go forth of us, 'twere all alike
        As if we had them not.
```

Xxxx xxxxxxx xxxxx xxx xxx xx xxxxxx xxxxxxxxxx xx xxxxxx xxx xxxxx xxx xxxxxx xxxxxxxxxx xx XxxxxxxXxxx$XxxxxxXxxx.
Xx xxxx xxxxxxx$ xxx xxxxxx xxxxxxxx $x xx xxxx xx xxxxxx xxx xxxxx xxxxxx x xxxxx xx xxxx $xxx xxxxx$ xx xxx xxxxxxxxx xxxx xxxxx$ xxxx xx xxxxxxxxxx xxxx x xxxx xx xxxx $xxx xxxx$ xx xxx xxxxxxxxx xxxx xxxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>ConvertFrom-StringData "Message=Look in c:\\Windows\\System32"
Name                           Value                                                                                                                                     
----                           -----                                                                                                                                     
Message                        Look in c:\Windows\System32
```

Xxxx xxxxxxx xxxxx xxx xx xxx xx xxx xxxxxxxxx xxxxxx xxxxxxxxx xx xxx xxxxxx xxxx xx xxxxx x xxxx xxxx xx xxxxxx xxxxxxxxx xx xxx xxxxxxxxx XxxxxxxXxxx$XxxxxxXxxx xxxx xxxxx.
Xxx xxxxxx xxxxxxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxxxx xxxxxxxxxx xxxxxx xxxxxxxxx xx xxx xxxx xxxxx xxxxxx.

## XXXXXXXXXX

### -InformationAction
Xxx xxxxx xx xxxx xxxxxxxxx xxxx xx x xxxxxx xxxx xx xxxxxxxx xx xxxxxx xxxxxxxxx xxxxx $x xxxxxx$xxxxxx xxxxxx$ xx x xxxxxx xxxx xx xxxxxxxx xx xxxxxx xxxxxxxxx xxxxx $x xxxxxx$xxxxxx xxxxxx$ xx x xxxx$xxxxxx xxxxxxxxxx xxx xx xxxx xxx$xxxxx xxxxx.
Xxxx xxx$xxxxx xxxx xxxx xx xx x xxxxxxxx xxxx$ xx xxxx xxxx xxxx xx xxxxxxxxx xx xxxxxxx xxxxxxxxxx $$$x$.

Xxx xxx xxxxxxx xxxxxxxx xx xxx xxxxxx$ xxx xxx xxxxxxxx xxxxxx xx xx xxx xxxx xxxx xx x xxx$xxxxx xxxx.
Xxx xxxxxxxx xxx xxx xxxxxxxx xx xxx xxxx xxxxx.

X xxxx$xxxxxx xx x xxxxxx xxxxxxxxxx xx xxx xx xxxx xxxxx xxxxxx xxxxx xxxxxxxxx xxxxx xxx xxxxxxxxxxx xxxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxx.

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
Xxx xxxxx xx xxxx xxxxxxxxx xxxx xx x xxxxxx xxxx xx xxxxxxxx xx xxxxxx xxxxxxxxx xxxxx $x xxxxxx$xxxxxx xxxxxx$ xx x xxxxxx xxxx xx xxxxxxxx xx xxxxxx xxxxxxxxx xxxxx $x xxxxxx$xxxxxx xxxxxx$ xx x xxxx$xxxxxx xxxxxxxxxx xxx xx xxxx xxx$xxxxx xxxxx.
Xxxx xxx$xxxxx xxxx xxxx xx xx x xxxxxxxx xxxx$ xx xxxx xxxx xxxx xx xxxxxxxxx xx xxxxxxx xxxxxxxxxx $$$x$.

Xxx xxx xxxxxxx xxxxxxxx xx xxx xxxxxx$ xxx xxx xxxxxxxx xxxxxx xx xx xxx xxxx xxxx xx x xxx$xxxxx xxxx.
Xxx xxxxxxxx xxx xxx xxxxxxxx xx xxx xxxx xxxxx.

X xxxx$xxxxxx xx x xxxxxx xxxxxxxxxx xx xxx xx xxxx xxxxx xxxxxx xxxxx xxxxxxxxx xxxxx xxx xxxxxxxxxxx xxxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxx.

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

### -StringData
Xxxxxxxxx xxx xxxxxx xx xx xxxxxxxxx.
Xxx xxx xxx xxxx xxxxxxxxx xx xxxx x xxxxxx xx XxxxxxxXxxx$XxxxxxXxxx.
Xxx xxxxxxxxx xxxx xx xxxxxxxx.

Xxx xxxxx xx xxxx xxxxxxxxx xxxx xx x xxxxxx xxxx xx xxxxxxxx xx xxxxxx xxxxxxxxx xxxxx $x xxxxxx$xxxxxx xxxxxx$ xx x xxxxxx xxxx xx xxxxxxxx xx xxxxxx xxxxxxxxx xxxxx $x xxxxxx$xxxxxx xxxxxx$ xx x xxxx$xxxxxx xxxxxxxxxx xxx xx xxxx xxx$xxxxx xxxxx.
Xxxx xxx$xxxxx xxxx xxxx xx xx x xxxxxxxx xxxx$ xx xxxx xxxx xxxx xx xxxxxxxxx xx xxxxxxx xxxxxxxxxx $$$x$.

Xxx xxx xxxxxxx xxxxxxxx xx xxx xxxxxx$ xxx xxx xxxxxxxx xxxxxx xx xx xxx xxxx xxxx xx x xxx$xxxxx xxxx.
Xxx xxxxxxxx xxx xxx xxxxxxxx xx xxx xxxx xxxxx.

X xxxx$xxxxxx xx x xxxxxx xxxxxxxxxx xx xxx xx xxxx xxxxx xxxxxx xxxxx xxxxxxxxx xxxxx xxx xxxxxxxxxxx xxxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## XXXXXX

### System.String
Xxx xxx xxxx x xxxxxx xxxxxxxxxx x xxx$xxxxx xxxx xx XxxxxxxXxxx$XxxxxxXxxx.

## XXXXXXX

### System.Collections.Hashtable
XxxxxxxXxxx$XxxxxxXxxx xxxxxxx x xxxx xxxxx xxxx xx xxxxxxx xxxx xxx xxx$xxxxx xxxxx.

## XXXXX
X xxxx$xxxxxx xx x xxxxxx xxxxxxxxxx xx xxx xx xxxx xxxxx xxxxxx xxxxx xxxxxxxxx xxxxx xxx xxxxxxxxxxx xxxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxx$Xxxxx.

XxxxxxxXxxx$XxxxxxXxxx xxx xx xxxxxx xx xxxxxxx xxxx xxxxxxx xxxx xxxxxxxx xx xxxxxxxx xxxxxx xxxxxxxxx.
Xxx xxx xxx xxx xxxxxxxxxx$xxxxx xxxx xxxxxx xx xxxxxxx xxxx xxxxxxx xxxx xxxx$ xxxx xx xx xxxxxxxx xxxxx$ xxx xx xxxxxx xxx xxxx xxxxxxx xxx xxx xx xxxxxxxxxxx xxxxx.

## XXXXXXX XXXXX

[about_Quoting_Rules]()

[about_Script_Internationalization]()

[about_Data_Sections]()

