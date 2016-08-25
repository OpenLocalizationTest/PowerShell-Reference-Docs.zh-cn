---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293984
schema: 2.0.0
---

# Import-LocalizedData
## XXXXXXXX
Xxxxxxx xxxxxxxx$xxxxxxxx xxxx xxxx xxxxxxx xxx xxxxxxxxx xxxxx xx xxx XX xxxxxxx xxxx xx xxxxxxxx xxx xxx xxxxxxxxx xxxxxx.

## XXXXXX

```
Import-LocalizedData [[-BindingVariable] <String>] [[-UICulture] <String>] [-BaseDirectory <String>]
 [-FileName <String>] [-SupportedCommand <String[]>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XxxxxxxxxXxxx xxxxxx xxxxxxxxxxx xxxxxxxxx xxxxxxx xxxx x xxxxxxxxxxxx xxxxx xxxx xxxxxxx xxx XX xxxxxxxx xxx xxx xxx xxxxxxx xxxx xx xxx xxxxxxxxx xxxxxx.
Xx xx xxxxxxxx xx xxxxxx xxxxxxx xx xxxxxxx xxxx xxxxxxxx xx xxx XX xxxxxxxx xxxxxxxx xx xxx xxxxxxx xxxx.

Xxxxxx$XxxxxxxxxXxxx xxxxxxx xxxx xxxx .xxx0 xxxxx xx xxxxxxxx$xxxxxxxx xxxxxxxxxxxxxx xx xxx xxxxxx xxxxxxxxx xxx xxxxx xxxx xx x xxxxx xxxxxxxx xxxx xx xxxxxxxxx xx xxx xxxxxxx.
Xxx xxxxxx xxxxxxx xxx xxxxxxxxxxxx xxx xxxx xxxxx xx xxx xxxxx xx xxx $XXXXXxxxxxx xxxxxxxxx xxxxxxxx.
Xxxx xxx xxx xxx xxxxx xxxxxxxx xx xxx xxxxxx xx xxxxxxx x xxxx xxxxxxx$ xxx xxxxxxx xxxxxxx xx xxx xxxx$x XX xxxxxxxx.

Xxx xxx xxx xxx xxxxxxxxxx xx Xxxxxx$XxxxxxxxxXxxx xx xxxxxxx xx xxxxxxxxx XX xxxxxxx$ xxxx$ xxx xxxx xxxx$ xx xxx xxxxxxxxx xxxxxxxx$ xxx xx xxxxxxxx xxx xxxxx xxxxxxx xxxx xxxxxxx xx xxx .xxx0 xxxxx xxx xxx xxxxx.

Xxx Xxxxxx$XxxxxxxxxXxxx xxxxxx xxxxxxxx xxx xxxxxx xxxxxxxxxxxxxxxxxxxx xxxxxxxxxx xxxx xxx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.
Xxxx xxxxxxxxxx xxxx xx xxxxxx xxxxx xxxxx xxxxxxxxx xx xxxxxx xx xxxx xxx xxxxxxx xx xxxxxxx xxxx xxxxxxxx xx xxx XX xxxxxxxx xx xxx xxxxxxx xxxx. Xxx xxxx xxxxxxxxxxx xxxxx xxxx xxx xxxxx xxx xxxxxx xx xxx .xxx0 xxxxx$ xxx xxxxx$Xxxxxx$Xxxxxxxxxxxxxxxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Import-LocalizedData -BindingVariable Messages
```

Xxxx xxxxxxx xxxxxxx xxxx xxxxxxx xxxx xxx $Xxxxxxxx xxxxxxxx.
Xx xxxx xxx xxxxxxx xxxxxx xx xxx xxxxx xxxxxx xxxxxxxxxx.

Xx xxx xxxxxxx xx xxxxxxxx xx xxx Xxxxxxxx.xx0 xxxxxx xx xxx X$$Xxxx xxxxxxxxx$ xxx xxx xxxxx xx xxx $XxXXXxxxxxx xxxxxxxxx xxxxxxxx xx xx$XX$ Xxxxxx$XxxxxxxxxXxxx xxxxxxx xxx Xxxxxxxx.xxx0 xxxx xx xxx X$$xxxx$xx$XX xxxxxxxxx xxxx xxx $Xxxxxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Import-LocalizedData -FileName Test.psd1 -UICulture en-US

Name                           Value
----                           -----
Msg3                           "Use $_ to represent the object that is being processed."
Msg2                           "This command requires the credentials of a member of the Administrators group on the...
Msg1                           "The Name parameter is missing from the command."
```

Xxxx xxxxxxx xx xxx xx xxx xxxxxxx xxxx$ xxx xx x xxxxxx.
Xx xxxx xxxxxxxxx xxxx xxxxxxx xxxx xxx Xxxx.xxx0 xxxx xxx xxxxxxxx xxxx xx xxx xxxxxxx xxxx.
Xxxxxxx xxx xxxxxxx xx xxx xxxx xx x xxxxxx$ xxx XxxxXxxx xxxxxxxxx xx xxxxxxxx.
Xxx xxxxxxx xxxx xxx XXXxxxxx xxxxxxxxx xx xxxxxxx xxx xx$XX xxxxxxx.

Xxxxxx$XxxxxxxxxXxxx xxxxxxx x xxxx xxxxx xxxx xxxxxxxx xxx xxxxxxxxx xxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Import-LocalizedData -BindingVariable msgTbl -UICulture ar-SA -FileName Simple -BaseDirectory C:\Data\Localized
```

Xxxx xxxxxxx xxxxxxx xxxx xxxxxxx xxxx xxx $xxxXxx  xxxxxxxx xx x xxxxxx.

Xx xxxx xxx XXXxxxxxx xxxxxxxxx xx xxxxxx xxx xxxxxx xx xxxxxx xxxx xxxx xxx Xxxxxx.xxx0 xxxx xx xxx xx$XX xxxxxxxxxxxx xx X$$Xxxx$Xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\># In C:\Test\en-US\Test.psd1:

ConvertFrom-StringData @'

# English strings

Msg1 = "The Name parameter is missing from the command."
Msg2 = "This command requires the credentials of a member of the Administrators group on the computer."
Msg3 = "Use $_ to represent the object that is being processed."
'@

# In C:\Test\Test.ps1

Import-LocalizedData -Bindingvariable Messages
Write-Host $Messages.Msg2

# In Windows PowerShell

.\Test.ps1
This command requires the credentials of a member of the Administrators group on the computer.
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxxxxxxxx xxxx xx x xxxxxx xxxxxx.

Xxx xxxxx xxxx xx xxx xxxxxxx xxxxx xxx xxxxxxxx xx xxx Xxxx.xxx0 xxxx.
Xx xxxxxxxx x XxxxxxxXxxx$XxxxxxXxxx xxxxxxx xxxx xxxxxxxx x xxxxxx xx xxxxx xxxx xxxxxxx xxxx x xxxx xxxxx.
Xxx Xxxx.xxx0 xxxx xx xxxxxxx xx xxx xx$XX xxxxxxxxxxxx xx xxx X$$Xxxx xxxxxxxxx xxxx xxxxxxxx xxx xxxxxx.

Xxx xxxxxx xxxx xx xxx xxxxxxx xxxxx xxx xxxxxxxx xx xxx Xxxx.xx0 xxxxxx.
Xx xxxxxxxx xx Xxxxxx$XxxxxxxxxXxxx xxxxxxx xxxx xxxxxxx xxx xxxx xxxx xxx xxxxxxxx .xxx0 xxxx xxxx xxx $Xxxxxxxx xxxxxxxx xxx x Xxxxx$Xxxx xxxxxxx xxxx xxxxxx xxx xx xxx xxxxxxxx xx xxx $Xxxxxxxx xxxxxxxx xx xxx xxxx xxxxxxx.

Xxx xxxx xxxx xx xxx xxxxxxx xxxx xxx xxxxxx.
Xxx xxxxxx xxxxx xxxx xx xxxxxxxx xxx xxxxxxx xxxx xxxxxxx xx xxx XX xxxxxxxx xxx xxx xxx xxxxxxx xxxx xx xxx xxxxxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\># In TestScript.ps1$UserMessages = DATA 

{    ConvertFrom-StringData @'

    # English strings

        Msg1 = "Enter a name." 
        Msg2 = "Enter your employee ID." 
        Msg3 = "Enter your building number." 
'@ }
Import-LocalizedData -BindingVariable UserMessages
$UserMessages.Msg1...
```

Xxxx xxxxxxx xxxxx xxx xx xxx Xxxxxx$XxxxxxxxxXxxx xx xxxxxxx xxxxxxx xxxx xxxxxxx xxxxxxx xx xxx XXXX xxxxxxx xx x xxxxxx.

Xx xxxx xxxxxxx$ xxx XXXX xxxxxxx xx xxx XxxxXxxxxx.xx0 xxxxxx xxxxxxxx x XxxxxxxXxxx$XxxxxxXxxx xxxxxxx xxxx xxxxxxxx xxx xxxxxxxx xx xxx XXXX xxxxxxx xx x xxxx xxxxx xxx xxxxxx xx xxx xxxxx xx xxx $XxxxXxxxxxxx xxxxxxxx.

Xxx xxxxxx xxxx xxxxxxxx xx Xxxxxx$XxxxxxxxxXxxx xxxxxxx$ xxxxx xxxxxxx x xxxx xxxxx xx xxxxxxxxxx xxxx xxxxxxx xxxx xxx XxxxXxxxxx.xxx0 xxxx xx xxx xxxxxxxxxxxx xxxxxxxxx xx xxx xxxxx xx xxx $XxXXXxxxxxx xxxxxxxx.
Xx xxx xxxxxxx xxxxx xxx .xxx0 xxxx$ xx xxxxx xxx xxxxxxxxxx xxxxxxx xxxx xxx xxxx xx xxx xxxxx xx xxx xxxx $XxxxXxxxxxxx xxxxxxxx$ xxxxxxxxxxx xxx xxxx xxxxx xxxxx xx xxx XXXX xxxxxxx xxxxx.

Xxx xxxxx xxxxxxx xxxxxxxx xxx xxxxx xxxxxxx xx xxx $XxxxXxxxxxxx xxxxxxxx.

Xx xxx Xxxxxx$XxxxxxxxxXxxx xxxxxxx xxxxx x .xxx0 xxxx xxx xxx $XxXXXxxxxxx xxxxxxxx$ xxx xxxxx xx xxx $XxxxXxxxxxxx xxxxxxxx xxxxxxxx xxx xxxxxxxxxx xxxx xxxxxxx.
Xx xxx xxxxxxx xxxxx xxx xxx xxxxxx$ xxx xxxxxxx xxxxxxxx xxx xxxxxxx xxxx xxxxxxx xxxxxxx xx xxx XXXX xxxxxxx xx xxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\># In Day1.ps1

PS C:\>Import-LocalizedData -BindingVariable DayDay.MessageDate

# In Day2.ps1

PS C:\>Import-LocalizedData -BindingVariable Day -ErrorAction:SilentlyContinue
Day.MessageDate
PS C:\>.\Day1.ps1
Import-LocalizedData : Cannot find PowerShell data file 'Day1.psd1' in directory 'C:\ps-test\fr-BE\' or any parent culture directories. 
At C:\ps-test\Day1.ps1:17 char:21+ Import-LocalizedData <<<<  Day
Today is Tuesday
PS C:\>.\Day2.ps1
Today is Tuesday
```

Xxxx xxxxxxx xxxxx xxx xx xxxxxxxx xxx xxxxx xxxxxxxx xxxx xxxxxx xxxx Xxxxxx$XxxxxxxxxXxxx xxxxxx xxxx xxx xxxxxxxxxxx xxxx xxxxx xxx xxxx$x XX xxxxxxx xx xxxxxx xxxx x .xxx0 xxxx xxx xxx xxxxxx xx xxxxx xxxxxxxxxxx.

Xxx xxx xxx xxx XxxxxXxxxxx xxxxxx xxxxxxxxx xxxx x xxxxx xx XxxxxxxxXxxxxxxx xx xxxxxxxx xxx xxxxx xxxxxxx.
Xxxx xx xxxxxxxxxx xxxxxx xxxx xxx xxxx xxxxxxxx xxxx xxxxxxxx xx x xxxxxxx xx $xxxxxxxx$ xxxxxxxx$ xxx xx xxxxx xxxxxxx xx xxxxxx.

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxx$ Xxx0.xx0 xxx Xxx0.xx0$ xxxx xxxxxxx xx Xxxxxx$XxxxxxxxxXxxx xxxxxxx.
Xxx xxxxxxx xxx xxxxxxxxx$ xxxxxx xxxx Xxx0 xxxx xxx XxxxxXxxxxx xxxxxx xxxxxxxxx xxxx x xxxxx xx XxxxxxxxXxxxxxxx.

Xxx xxxxxx xxxxxx xxxxx xxx xxxxxxx xx xxxxxxx xxxx xxxxxxx xxxx xxx XX xxxxxxx xx xxx xx xx$XX xxx xxxxx xxx xx xxxxxxxx xxxxx xx xxxxxxxxxxx xxx xxxx XX xxxxxxx.
Xxx0.xx0 xxxxxxxx xx xxxxx xxxxxxx xxx Xxxxxxx xxxxxx.
Xxx0.xx0 xxxx xxxxxxxx xxx Xxxxxxx xxxxxx.

## XXXXXXXXXX

### -BaseDirectory
Xxxxxxxxx xxx xxxx xxxxxxxxx xxxxx xxx .xxx0 xxxxx xxx xxxxxxx.
Xxx xxxxxxx xx xxx xxxxxxxxx xxxxx xxx xxxxxx xx xxxxxxx.
Xxxxxx$XxxxxxxxxXxxx xxxxxxxx xxx xxx .xxx0 xxxx xxx xxx xxxxxx xx x xxxxxxxx$xxxxxxxx xxxxxxxxxxxx xx xxx xxxx xxxxxxxxx.

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

### -BindingVariable
Xxxxxxxxx xxx xxxxxxxx xxxx xxxxx xxx xxxx xxxxxxx xxx xxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxx x xxxxxx xxxx $$$.

Xx Xxxxxxx XxxxxXxxxx 0.0$ xxxx xxxxxxxxx xx xxxxxxxx.
Xx Xxxxxxx XxxxxXxxxx 0.0$ xxxx xxxxxxxxx xx xxxxxxxx.
Xx xxx xxxx xxxx xxxxxxxxx$ Xxxxxx$XxxxxxxxxXxxx xxxxxxx x xxxx xxxxx xx xxx xxxx xxxxxxx.
Xxx xxxx xxxxx xx xxxxxx xxxx xxx xxxxxxxx xx xxxxxxxxx xx xxx xxxxxxx xxxx.

Xxxx xxxxx Xxxxxx$XxxxxxxxxXxxx xx xxxxxxx xxxxxxx xxxx xxxxxxx xxxxxxxxx xx xxx XXXX xxxxxxx xx x xxxxxx$ xxxxxx xxx XXXX xxxxxxx xx x xxxxxxxx xxx xxxxx xxx xxxx xx xxx XXXX xxxxxxx xxxxxxxx xx xxx xxxxx xx xxx XxxxxxxXxxxxxxx xxxxxxxxx.
Xxxx$ xxxx Xxxxxx$XxxxxxxxxXxxx xxxxx xxx xxxxxxxx xxxxxxx xx xxx XxxxxxxXxxxxxxx$ xxx xxxxxxxx xxxx xxxx xxxxxxx xxx xxxxxxx xxxx xxxxxxx.
Xx xxx xxx xxx xxxxxxxxxx xxxxxxx xxxx xxxxxxx$ xxx xxx xxxxxx xxx xxxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Variable

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FileName
Xxxxxxxxx xxx xxxx xx xxx xxxx xxxx $.xxx0$ xx xx xxxxxxxx.
Xxxxx x xxxx xxxx.
Xxx xxx xxxxxxx x xxxx xxxx xxxx xxxx xxx xxxxxxx xxx .xxx0 xxxx xxxx xxxxxxxxx$ xx xxx xxx xxxxxxx xxx xxxx xxxx xxxxxxxxx xxx .xxx0 xxxx xxxx xxxxxxxxx.

Xxx XxxxXxxx xxxxxxxxx xx xxxxxxxx xxxx Xxxxxx$XxxxxxxxxXxxx xx xxx xxxx xx x xxxxxx.
Xxxxxxxxx$ xxx xxxxxxxxx xx xxxxxxxx xxx xxx xxxxxxx xxxxx xx xxx xxxx xxxx xx xxx xxxxxx.
Xxx xxx xxx xxxx xxxxxxxxx xx xxxxxx Xxxxxx$XxxxxxxxxXxxx xx xxxxxx xxx x xxxxxxxxx .xxx0 xxxx.

Xxx xxxxxxx$ xx xxx Xxxxxxxx xx xxxxxxx xxx xxx xxxxxx xxxx xx XxxxXxxxx.xx0$ Xxxxxx$XxxxxxxxxXxxx xxxxxxxx xxx xxx XxxxXxxxx.xxx0 xxxx xxxx.

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

### -SupportedCommand
Xxxxxxxxx xxxxxxx xxx xxxxxxxxx xxxx xxxxxxxx xxxx xxxx.

Xxx xxxx xxxxxxxxx xx xxxxxxx xxxxxxx xxx xxxxxxxxx xxxx xxx xxxx xxxxxxx xx xxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxx$Xxxxxxxxxxxxxxxxxxxx.

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

### -UICulture
Xxxxxxxxx xx xxxxxxxxx XX xxxxxxx.
Xxx xxxxxxx xx xxx xxxxx xx xxx $XxXXXxxxxxx xxxxxxxxx xxxxxxxx.
Xxxxx x XX xxxxxxx xx $$$xxxxxxxx$$$$$xxxxxx$$$ xxxxxx$ xxxx xx xx$XX$ xx$XX$ xx xx$XX.

Xxx xxxxx xx xxx XXXxxxxxx xxxxxxxxx xxxxxxxxxx xxx xxxxxxxx$xxxxxxxx xxxxxxxxxxxx $xxxxxx xxx xxxx xxxxxxxxx$ xxxx xxxxx Xxxxxx$XxxxxxxxxXxxx xxxx xxx .xxx0 xxxx xxx xxx xxxxxx.

Xxx xxxxxx xxxxxxxx xxx x xxxxxxxxxxxx xxxx xxx xxxx xxxx xx xxx xxxxx xx  xxx XXXxxxxxx xxxxxxxxx xx xxx $XxXXXxxxxxx xxxxxxxxx xxxxxxxx$ xxxx xx $xx$XX$ xx $xx$XX$.
Xx xx xxxxxx xxxx xxx xxxxxxxxx$ xx xxx xxxxxxxxx xxxx xxx xxxxxxx x .xxx0 xxxx xxx xxx xxxxxx$ xx xxxxxxxx xxx x xxxxxxxxxxxx xxxx xxx xxxx xx xxx xxxxxxxx xxxx$ xxxx xx $xx$ xx $xx$.
Xx xx xxxxxx xxxx xxx xxxxxxxxxxxx xx .xxx0 xxxx$ xxx xxxxxxx xxxxx xxx xxx xxxx xx xxxxxxxxx xx xxx xxxxxxx xxxxxxxx xxxxxxxxx xx xxx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### None
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### System.Collections.Hashtable
Xxxxxx$XxxxxxxxxXxxx xxxxx xxx xxxx xxxxx xx xxx xxxxxxxx xxxx xx xxxxxxxxx xx xxx xxxxx xx xxx XxxxxxxXxxxxxxx xxxxxxxxx.

## XXXXX
Xxxxxx xxxxx Xxxxxx$XxxxxxxxxXxxx$ xxxxxxxx xxxx xxxx xxxxxxxx.
Xxxxxx xxx xxxxxxxx xxx xxxx xxxxxx $XX xxxxxxx$ xx x xxxx xxxxx xx xxx$xxxxx xxxxx$ xxx xxxx xxx xxxx xxxxx xx x xxxx xxxx xxx xxxx xxxx xx xxx xxxxxx xxx x .xxx0 xxxx xxxx xxxxxxxxx.
Xxxxxx x xxxxxxxxx xxxxx xxx xxxxxx xxxxxxxxx xxx xxxx xxxxxxxxx XX xxxxxxx$ xxx xxxx xxxx xxx .xxx0 xxxx xxx xxxx XX xxxxxxx xx xxx xxxxxxxxx xxxx xxx XX xxxxxxx xxxx.

Xxx xxxxxxx$ xxxxxxxx xxxx xxxx xxxxxxxx xxx xxx xx$XX xxxxxx xxx xxxxxx xxxx xx x xxxx xxxxx.
Xxxx xxx xxxx xxxxx xx x $$XxxxxxXxxx$$.xxx0 xxxx.
Xxxx xxxxxx x xx$XX xxxxxxxxxxxx xxxxx xxx xxxxxx xxxxxxxxx$ xxx xxxx xxx xx$XX $$XxxxxxXxxx$$.xxx0 xxxx xx xxx xx$XX xxxxxxxxxxxx.
Xxxxxx xxxx xxxxxx xxx xxxx xxxxxx xxxx xxx xxxxxxx.

Xxxxxx$XxxxxxxxxXxxx xxxxxxxx x xxxxxxxxxx xxxxxx xxx xxx xxxxxxxxx xxxx xxxxxxxx xxx x xxxxxx.

Xxxxxx$XxxxxxxxxXxxx xxxxxx xxx xxxxxx xx xxx xxxxxxxxx xxxxx xxx xxxxxx xxxx xx xxxxxxx $xx xxx xxxxx xx xxx XxxxXxxxxxxxx xxxxxxxxx$.
Xx xxxx xxxxxxxx xxxxxx xxx xxxx xxxxxxxxx xxx x xxxxxxxxxxxx xxxx xxx xxxx xxxx xx xxx xxxxx xx xxx $XxXXXxxxxxx xxxxxxxx $xx xxx xxxxx xx xxx XXXxxxxxx xxxxxxxxx$$ xxxx xx $xx$XX$ xx $xx$XX$.
Xxxx$ xx xxxxxxxx xx xxxx xxxxxxxxxxxx xxx x .xxx0 xxxx xxxx xxx xxxx xxxx xx xxx xxxxxx $xx xxx xxxxx xx xxx XxxxXxxx xxxxxxxxx$.

Xx Xxxxxx$XxxxxxxxxXxxx xxxxxx xxxx x xxxxxxxxxxxx xxxx xxx xxxx xx xxx XX xxxxxxx$ xx xxx xxxxxxxxxxxx xxxx xxx xxxxxxx x .xxx0 xxxx xxx xxx xxxxxx$ xx xxxxxxxx xxx x .xxx0 xxxx xxx xxx xxxxxx xx x xxxxxxxxxxxx xxxx xxx xxxx xx xxx xxxxxxxx xxxx$ xxxx xx $xx$ xx $xx$.
Xx xx xxxxxx xxxx xxx xxxxxxxxxxxx xx .xxx0 xxxx$ xxx xxxxxxx xxxxx$ xxx xxxx xx xxxxxxxxx xx xxx xxxxxxx xxxxxxxx xx xxx xxxxxx$ xxx xx xxxxx xxxxxxx xx xxxxxxxxx xxxxxxxxxx xxxx xxx xxxx xxxxx xxx xx xxxxxxxx.
Xx xxxxxxxx xxx xxxxxxx xxx xxxx xxxxxxxxxx$ xxx xxx XxxxxXxxxxx xxxxxx xxxxxxxxx xxxx x xxxxx xx XxxxxxxxXxxxxxxx.

Xx Xxxxxx$XxxxxxxxxXxxx xxxxx xxx xxxxxxxxxxxx xxx xxx .xxx0 xxxx$ xx xxxxxxx xxx xxxx xxxxx xx xxxx xxxxxxxx xxxx xxx xxxxx xx xxx XxxxxxxXxxxxxxx xxxxxxxxx xx xxx xxxxxxx.
Xxxx$ xxxx xxx xxxxxxx x xxxxxxx xxxx xxx xxxx xxxxx xx xxx xxxxxxxx$ xxx xxxxxxxxx xxxxxxx xx xxxxxxxxx.

Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxx$Xxxxxxxxxxxxxxxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

## XXXXXXX XXXXX

[about_Script_Internationalization]()

