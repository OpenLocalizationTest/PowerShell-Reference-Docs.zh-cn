---
external help file: Microsoft.PowerShell.Commands.Utility.dll-help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293942
schema: 2.0.0
---

# Xxx$Xxxxxx
## XXXXXXXX
Xxxx xxxxxx xxxxxxxxxx xxx xxxxxxx xx xx xxxxxxxx xx x Xxxxxxx XxxxxXxxxx xxxxxx.

## XXXXXX

### XxxxXxxxXxx $Xxxxxxx$
```
Add-Member -InputObject <PSObject> -TypeName <String> [-PassThru] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### XxxxxxXxx
```
Add-Member -InputObject <PSObject> [-MemberType] <PSMemberTypes> [-Name] <String> [[-Value] <Object>]
 [[-SecondValue] <Object>] [-TypeName <String>] [-Force] [-PassThru] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### XxxxXxxxxxxxXxxxxxXxxxxxXxx
```
Add-Member -InputObject <PSObject> [-TypeName <String>] [-Force] [-PassThru] [-NotePropertyName] <String>
 [-NotePropertyValue] <Object> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### XxxxXxxxxxxxXxxxxXxxxxxXxx
```
Add-Member -InputObject <PSObject> [-TypeName <String>] [-Force] [-PassThru]
 [-NotePropertyMembers] <IDictionary> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxx xxxxxx xxxx xxx xxx xxxxxxx $xxxxxxxxxx xxx xxxxxxx$ xx xx xxxxxxxx xx x Xxxxxxx XxxxxXxxxx xxxxxx.
Xxx xxxxxxx$ xxx xxx xxx x XxxxXxxxxxxx xxxxxx xxxx xxxxxxxx x xxxxxxxxxxx xx xxx xxxxxx xx x XxxxxxXxxxxx xxxxxx xxxx xxxx x xxxxxx xx xxxxxx xxx xxxxxx.

Xx xxx Xxx$Xxxxxx$ xxxx xxx xxxxxx xx Xxx$Xxxxxx$ xx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxx.
Xxx xxx XxxxxxXxxx xxxxxxxxx xx xxxxxxx xxx xxxx xx xxxxxx xxxx xxx xxxx xx xxx$ xxx xxx Xxxx xxxxxxxxx xx xxxxxx x xxxx xx xxx xxx xxxxxx$ xxx xxx xxx Xxxxx xxxxxxxxx xx xxx xxx xxxxx xx xxx xxxxxx.

Xxx xxxxxxxxxx xxx xxxxxxx xxxx xxx xxx xxx xxxxx xxxx xx xxx xxxxxxxxxx xxxxxxxx xx xxx xxxxxx xxxx xxx xxxxxxx.
Xxx$Xxxxxx xxxx xxx xxxxxx xxx xxxxxx xxxx.
Xx xxxxxx x xxx xxxxxx xxxx$ xxx xxx Xxx$Xxxx xxxxxx.
Xxx xxx xxxx xxx xxx Xxxxxx$Xxxxxx xxxxxx xx xxxx xxx xxxxxxxx xx xxx xxxxxx$ xxxxxxxxx xxx xxxxxxxxxx xxxxxxx$ xx x xxxx.
Xxxx xxx xxx xxx xxx Xxxxxx$Xxxxxx xxxxxx xx xx$xxxxxx xxx xxxxxxxx xx xxx xxxxxx xxxx xxx xxxxxxxxxxx xxxx xx xxxxxx xx xxx xxxxxxxx xxxx.

Xxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ Xxx$Xxxxxx xxx xxx xxxxxxxx xxxx xxxx xx xxxxxx xx xxx xxxx xxxxxxxxxx xx xxxxxxx.
Xxx xxx xxx xxx XxxxXxxxxxxxXxxx xxx XxxxXxxxxxxxXxxxx xxxxxxxxxx xx xxxxxx x xxxx xxxxxxxx xx xxx xxx XxxxXxxxxxxxXxxxxxx xxxxxxxxx$ xxxxx xxxxx x xxxx xxxxx xx xxxx xxxxxxxx xxxxx xxx xxxxxx.

Xxxx$ xxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ xxx XxxxXxxx xxxxxxxxx$ xxxxx xxxxxxxxx xx xxxxxx xxxxxx$ xx xxxxxx xxxx xxxxxxxxxx.
Xxx$Xxxxxx xxx xxxx xxx xxx xxxxxxx xxxxxxxx xx xxx xxxxx xxxxxx xx xxxx xxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxx XxxxXxxx xxxxxxxxx xxxxxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = dir c:\ps-test\test.txt
PS C:\>$a | Add-Member -NotePropertyName Status -NotePropertyValue Done
PS C:\>$a | Add-Member Status Done
PS C:\>$a.Status
Done
```

Xxxxx xxxxxxxx xxx xxx Xxxxxx xxxx xxxxxxxx xxxx x xxxxx xx $Xxxx$ xx xxx XxxxXxxx xxxxxx xxxx xxxxxxxxxx xxx Xxxx.xxx xxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XxxxxXxxx xxxxxx $xxxxx $ $xxx$ xx xxx xxx Xxxx.xxx xxxx.
Xx xxxxx xx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxx xxxxx xxxxxxxx xxx xxx xxxx xxxxxxxx xx xxx xxxxxx xx $x.
Xxx xxxxx xxxxxxx xxxxx xxx xxxxxxxx xxxxxxxxx xxxxx$ xx xxx xxxxxxxxx xxxxxx xxxx xx xx xxx xxxxxxx Xxxx$Xxxxx xxxxx.
Xxxxx xxxxxxxx xxx xxxxxxxxxx xxx xxx xx xxxx xxxxxxxxxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxx xxx xxxxx xx xxx Xxxxxx xxxxxxxx xx xxx xxxxxx xx $x.
Xx xxx xxxxxx xxxxx$ xxx xxxxx xx $Xxxx$.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = dir c:\ps-test\test.txt
PS C:\>$a | Add-Member -MemberType AliasProperty -Name FileLength -Value Length
PS C:\>$a.FileLength
2394
```

Xxxxx xxxxxxxx xxx xxx XxxxXxxxxx xxxxx xxxxxxxx xx xxx xxxxxx xxxx xxxxxxxxxx xxx Xxxx.xxx xxxx.
Xxx xxx xxxxxxxx xx xx xxxxx xxx xxx Xxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxx xxx Xxx$XxxxxXxxx xxxxxx $xxxxx $ $xxx$$ xx xxx xxx Xxxx.xxx xxxx.

Xxx xxxxxx xxxxxxx xxxx xxx XxxxXxxxxx xxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxx xxx xxxxx xx xxx xxx XxxxXxxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = "A string"
PS C:\>$a = $a | Add-Member @{StringUse="Display"} -PassThru
PS C:\>$a.StringUse
Display
```

Xxxxx xxxxxxxx xxx xxx XxxxxxXxx xxxx xxxxxxxx xx x xxxxxx.
Xxxxxxx Xxx$Xxxxxx xxxxxx xxx xxxxx xx Xxxxxx xxxxx xxxxxxx$ xxx xxxxxxx xxxx xxx  XxxxXxxx xxxxxxxxx xx xxxxxxxx xx xxxxxx xxxxxx.
Xxx xxxx xxxxxxx xx xxx xxxxxxx xxxxxxxx xxx xxx xxxxxxxx.

Xxx xxxxxxx xxxx xxx XxxxXxxxxxxxXxxxxxx xxxxxxxxx$ xxx xxxxx xxx xxxxxxxxx xxxx$ xxxxx xx xxxxxxxx.
Xxx xxxxx xx xxx XxxxXxxxxxxxXxxxxxx xxxxxxxxx xx x xxxx xxxxx.
Xxx xxx xx xxx xxxx xxxxxxxx xxxx$ XxxxxxXxx$ xxx xxx xxxxx xx xxx xxxx xxxxxxxx xxxxx$ Xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a = "This is a string."
PS C:\>$a = Add-Member -InputObject $a -MemberType ScriptMethod -Name PadBoth -Value {$p = $this.PadLeft($this.Length + 1); $p.PadRight($p.Length + 1)} -PassThru
PS C:\>$a.Padboth()
This is a string.
```

Xxxxx xxxxxxxx xxx xxx XxxXxxx xxxxxx xxxxxx xx x xxxxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxxxx xxx xxxxx xx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxxxx xxxxxx xxxxxx xx xxx xxxxxx xx xxx $x xxxxxxxx.
Xxx Xxxxx xxxxxxxxx xxxxxxx xxx xxx xxxxxx xxxxxx.
Xx xxxx xxx XxxXxxxx xxx XxxXxxx xxxxxxx xx x xxxxxx xx xxx xxx xxxxx xxx xxxx xxx xxx xxxxx xx xxx xxxxx xx xxx xxxxxx.

Xxx Xxxxx xxxxxxxxx xxxx xxxx xxx $xxxx xxxxxxxxx xxxxxxxx$ xxxxx xxxxxxxxxx xxx xxxxxxx xxxxxx.
Xxx $xxxx xxxxxxxx xx xxxxx xxxx xx xxxxxx xxxxxx xxxx xxxxxx xxx xxxxxxxxxx xxx xxxxxxx.

Xxx xxxxxxx xxxxxxxx xxx XxxxXxxx xxxxxxxxx xxxxx xxxxxxx Xxx$Xxxxxx xx xxxxxx xx xxxxxxxx xx xxx xxxxxx xxxx xxxxxxxx xxx xxx xxxxxx xxxxxxxx.
Xx xxxxxxx$ Xxx$Xxxxxx xxxx xxxxxxx xx XXXxxxxxx xxx xxxx xxx xxxxxxxx xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxxx xxx xxx XxxXxxx xxxxxx xxxxxx xx xxx xxxxxx xx xxx $x xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$event = Get-EventLog -LogName System -Newest 1
PS C:\>$event.TimeWritten | Get-Member
TypeName: System.DateTime

Name                 MemberType     Definition
----                 ----------     ----------
Add                  Method         System.DateTime Add(System.TimeSpan value) 
AddDays              Method         System.DateTime AddDays(double value) 
AddHours             Method         System.DateTime AddHours(double value) 
AddMilliseconds      Method         System.DateTime AddMilliseconds(double value) 
AddMinutes           Method         System.DateTime AddMinutes(double value)...


PS C:\>Add-Member -InputObject $event -MemberType AliasProperty -Name When -Value TimeWritten -SecondValue System.String
PS C:\>$event.When | Get-Member
TypeName: System.String
Name             MemberType            Definition
----             ----------            ----------
Clone            Method                System.Object Clone()
CompareTo        Method                int CompareTo(System.Object value), int CompareTo(string strB) 
Contains         Method                bool Contains(string value)
```

Xxxxx xxxxxxxx xxx xxx $Xxxx$ xxxxx xxxxxxxx xx xx xxxxx xx xxx Xxxxxx xxxxx xxx.
Xxx xxxxx xx xx XxxxxXxxXxxxx xxxxxx xxxx xx xxxxxxxx xx xxx Xxx$XxxxxXxx xxxxxx.

Xxx $Xxxx$ xxxxx xxxxxxxx xx xx xxxxx xxx xxx XxxxXxxxxxx xxxxxxxx xx xxx xxxxxx.
Xxx XxxxxxXxxxx xxxxxxxxx xx xxxx xx xxxxxxx xxxx xxx xxxxxxxx xxxxx xxxxxx xx xxxxxxxxx xx xxxx Xxxxxx.Xxxxxx xxxx xxxxxxxx xx xxxxx xxx XxxxxXxxxxxxx.
Xxx XxxxXxxxxxx xxxxxxxx xx x XxxxXxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$XxxxxXxx xxxxxx xx xxx xxx xxxxxx xxxxx xx xxx Xxxxxx xxxxx xxx.
Xx xxxxxx xxx xxxxx xx xxx $Xxxxx xxxxxxxx.

Xx xxxxxxxxxxx xxxx xxx XxxxXxxxxxx xxxxxxxx xx x XxxxXxxx xxxx$ xxx xxxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxx xxx XxxxXxxxxxx xxxxxxxx xx xxxx xxxxx xxx xxxxx xx xx xxx Xxx$Xxxxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxx xxx Xxxx xxxxx xxxxxxxx xx xxx xxxxxx xxxxxxxx xx xxx $Xxxxx xxxxxxxx.
Xxx Xxxx xxxxxxxxx xxxxxxx xxx xxxx$ $Xxxx$$ xxx xxx Xxxxx xxxxxxxxx xxxxxxxxx xxxx Xxxx xx xx xxxxx xxx xxx XxxxXxxxxxx xxxxxxxx.
Xxx XxxxxxXxxxx xxxxxxxxx xxxxxxxxx xxxx xxx xxxxx xxxx xxx Xxxx xxxxxx xxxxxxx xxxxxx xx xxxx xx x Xxxxxx.Xxxxxx xxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxxx xxx xxx Xxxx xxxxxx.
Xxx xxxxxxx xxxxx xxx xxxxxx xxxxx xx xxx Xxx$Xxxxxx xxxxxx xx xxxxxxx xxxx xx xxx xxxxxxxx x xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>function Copy-Property ($From, $To)
{     foreach ($p in Get-Member -InputObject $From -MemberType Property)
  {     Add-Member -InputObject $To -MemberType NoteProperty -Name $p.Name
     -Value $From.$($p.Name) -Force     $To.$($p.Name) = $From.$($p.Name)
  }
}
```

Xxxx xxxxxxxx xxxxxx xxx xx xxx xxxxxxxxxx xx xxx xxxxxx xx xxxxxxx xxxxxx.

Xxx xxxxx xxxxxxx xx xxx xxxxxxxx xxxxxxxx xxx xxxxxxxx xxxx xxx xxxxx xxx xxxxxxxxxx.

Xxx Xxxxxxx xxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxx xxxx xx xxx xxxxxxxxxx xx xxx Xxxx xxxxxx.
Xxx xxxxxxxx xxxxxx xxx XxxXxxx xxxx xxx xxxxxxxxx xx xxxxxx xx xxxx xx xxx xxxxxxxxxx.

Xxx Xxx$Xxxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxx Xxxx xxxxxx xx xxx Xx xxxxxx xx x XxxxXxxxxxxx.
Xx xxxx xxx Xxxxx xxxxxxxxx xxx xxxxxxx xxxx xxx xxxx xxxxxx xxxx.

Xxx xxxx xxxxxxx xx xxx xxxxxxxx xxxxx xxx xxx xxxxxxxx xxx xxxx xxxx xx xxx xxxxxxxx xxxxxxxx.

### Xxxxxxx 0
```
PS C:\>$Asset = New-Object -TypeName PSObject
PS C:\>$d = [ordered]@{Name="Server30";System="Server Core";PSVersion="4.0"}
PS C:\>$Asset | Add-Member -NotePropertyMembers $d -TypeName Asset
PS C:\>$Asset | Get-Member
   TypeName: Asset

Name        MemberType   Definition
----        ----------   ----------
Equals      Method       bool Equals(System.Object obj) 
GetHashCode Method       int GetHashCode()
GetType     Method       type GetType()
ToString    Method       string ToString()
Name        NoteProperty System.String Name=Server30
PSVersion   NoteProperty System.String PSVersion=4.0
System      NoteProperty System.String System=Server Core
```

Xxxx xxxxxxx xxxxxxx xxx Xxxxx xxxxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxx xxxxxx xx xxxxxx x XXXxxxxx.
Xxx xxxxxxx xxxxx xxx XXXxxxxx xx xxx $Xxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx $$xxxxxxx$$ xxxx xxxxxxxxxxx xx xxxxxx xx xxxxxxx xxxxxxxxxx xx xxxxx xxx xxxxxx.
Xxx xxxxxxx xxxxx xxx xxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx XxxxXxxxxxxxXxxxxxx xxxxxxxxx xx xxx Xxx$Xxxxxx xxxxxx xx xxx xxx xxxxxxxxxx xx xxx $x xxxxxxxx xx xxx XXXxxxxx.
Xx xxxx xxx XxxxXxxx xxxxxxxx xx xxxxxx x xxx xxxx$ Xxxxx$ xx xxx XXXxxxxx.

Xxx xxxxxx xxxxxxx xxxxx xxx xxx Xxxxx xxxxxx xx xxx $Xxxxx xxxxxxxx xx xxx Xxx$Xxxxxx xxxxxx.
Xxx xxxxxx xxxxx xxxx xxx xxxxxx xxx x xxxx xxxx xx $Xxxxx$ xxx xxx xxxx xxxxxxxxxx xxxx xx xxxxxxx xx xxx xxxxxxx xxxxxxxxxx.

## XXXXXXXXXX

### $Xxxxx
Xxxx x xxx xxxxxx xxxx xxx xxxxxx xxx x xxxxxx xxxxxx xxxx xxx xxxx xxxx.
Xxx xxxxxx xxx xxx Xxxxx xxxxxxxxx xx xxxxxxx x xxxxxxxx xxxxxx xx x xxxx.

```yaml
Type: SwitchParameter
Parameter Sets: MemberSet, NotePropertySingleMemberSet, NotePropertyMultiMemberSet
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
Xxxxxxxxx xxx xxxxxx xx xxxxx xxx xxx xxxxxx xx xxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx$ xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $XxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xx xxx. Xxxx xxxxxxxxx xx xxxxxxxxx.

Xxx xxxxx xxxxxx xxx xxxx xxxxxxxxx xxx$ $XxxxXxxxxxxx$XxxxxXxxxxxxx$XxxxxxXxxxxxxx$XxxxXxxxxxxx$XxxxxxXxxxxx$XxxxXxxxxx$ XxxxxXxxxxxxx$ XxxxXxxxxx$ XxxxXxxxxxxx$ Xxxxxxxxxxxx$ XxxxxxXxxxxx$ xxx XxxxxxXxxxxxxx.

Xxx xxxxxxxxxxx xxxxx xxxxx xxxxxx$ xxx $XXXxxxxxXxxxx Xxxxxxxxxxx$ xx XXXX xx xxxx$$$xxxx.xxxxxxxxx.xxx$xx$xx$xxxxxxx$xxxxxxx$xxxxxxx$xxxxxx.xxxxxxxxxx.xxxxxxxxxx.xxxxxxxxxxxxx$x$xx.00$.xxxx.

Xxx xxx xxxxxxx xxxx xxxxx xxxx xx xxxxxx.
Xx xxx xxxxxxx x xxxxxx xxxx xxxx xxx xxxxxx xxxx xxx xxxx$ Xxxxxxx XxxxxXxxxx xxxxxxx xx xxxxx.

```yaml
Type: PSMemberTypes
Parameter Sets: MemberSet
Aliases: Type
Accepted values: AliasProperty, CodeProperty, Property, NoteProperty, ScriptProperty, Properties, PropertySet, Method, CodeMethod, ScriptMethod, Methods, ParameterizedProperty, MemberSet, Event, Dynamic, All

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xx xx xxxxx.

```yaml
Type: String
Parameter Sets: MemberSet
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxxxxx xxx xxxxx xxxxxxxx xxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

Xxx xxxx xxxxxxx$ Xxx$Xxxxxx xxxx xxx xxx xxxxxxx xx xxx xxxxx xxxxxx.
Xxxxxxx$ xxxx xxx xxxxx xxxxxx xx x xxxxxx$ Xxx$Xxxxxx xxxxxx xxx xxx xxxxxx xx xxx xxxxx xxxxxx.
Xxx xxxxx xxxxxxx$ xxx xxx XxxxXxxx xxxxxxxxx xx xxxxxx xx xxxxxx xxxxxx.

Xx Xxxxxxx XxxxxXxxxx 0.0$ Xxx$Xxxxxx xxxxx xxxxxxx xxxx xx xxx XXXxxxxx xxxxxxx xx xxxxxxx$ xxx xx xxx xxxxxx.
Xxx xxx XxxxXxxx xxxxxxxxx xx xxxxxx xx xxxxxx xxxxxx xxx xxx xxxxxx xxxx xxx x XXXxxxxx xxxxxxx.

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

### $XxxxxxXxxxx
Xxxxxxxxx xxxxxxxx xxxxxxxxxx xxxxxxxxxxx xxxxx XxxxxXxxxxxxx$ XxxxxxXxxxxxxx$ XxxxXxxxxxxx$ xx XxxxXxxxxx xxxxxxx.
Xx xxxx xxxx xxxxxx xx XxxxxXxxxxxxx$ xxxx xxxxxxxxx xxxx xx x xxxx xxxx.
X xxxxxxxxxx $xxxx$ xx xxx xxxxxxxxx xxxx xxxx xx xxxxx xx xxx xxxxx xx xxx XxxxxXxxxxxxx.
Xxx xxxxxxx$ xx xxx xxx xx XxxxxXxxxxxxx xxxx xxxxxxxx xx xxxxxxxxx xxxx xxx x xxxxxx xxxxxxxx$ xxx xxx xxxx xxxxxxx x XxxxxxXxxxx xxxxxxxxx xx Xxxxxx.Xxx00 xx xxxxxxxx xxxx xxx xxxxx xx xxxx xxxxxx xxxxxxxx xxxxxx xx xxxxxxxxx xx xx xxxxxxx xxxx xxxxxxxx xx xxxxx xxx xxxxxxxxxxxxx XxxxxXxxxxxxx.

Xxx xxx xxx xxx XxxxxxXxxxx xxxxxxxxx xx xxxxxxx xx xxxxxxxxxx XxxxxxXxxxx xxxx xxxxxx x XxxxxxXxxxxxxx xxxxxx.
Xx xxxx xxxx$ xxx xxxxx XxxxxxXxxxx$ xxxxxxxxx xx xxx Xxxxx xxxxxxxxx$ xx xxxx xx xxx xxx xxxxx xx x xxxxxxxx.
Xxx xxxxxx XxxxxxXxxxx$ xxxxxxxxx xx xxx XxxxxxXxxxx xxxxxxxxx$ xx xxxx xx xxx xxx xxxxx xx x xxxxxxxx.

```yaml
Type: Object
Parameter Sets: MemberSet
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxx
Xxxxxxxxx xxx xxxxxxx xxxxx xx xxx xxxxx xxxxxx.
Xx xxx xxx xx XxxxxXxxxxxxx$ XxxxXxxxxxxx$ XxxxxxXxxxxxxx xx XxxxXxxxxx xxxxxx$ xxx xxx xxxxxx xxxxxxxx$ xxxxxxxxxx xxxxxxxxxxx xx xxxxx xxx XxxxxxXxxxx xxxxxxxxx.

```yaml
Type: Object
Parameter Sets: MemberSet
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxxxxxxXxxxxxx
Xxxxxxxxx x xxxx xxxxx xx xxxxxxx xxxxxxxxxx xx xxxx xxxxxxxx xxxxx xxx xxxxxx.
Xxxx x xxxx xxxxx xx xxxxxxxxxx xx xxxxx xxx xxxx xxx xxxx xxxxxxxx xxxxx xxx xxx xxxxxx xxx xxxx xxxxxxxx xxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx xxxx xxxxxx xxx xxxxxxx xxxxxxxxxxxx xx Xxxxxxx XxxxxXxxxx$ xxx xxxxx$Xxxx$Xxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: IDictionary
Parameter Sets: NotePropertyMultiMemberSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxxxxxxXxxx
Xxxx x xxxx xxxxxxxx xxxx xxx xxxxxxxxx xxxx.

Xxx xxxx xxxxxxxxx xxxx xxx XxxxXxxxxxxxXxxxx xxxxxxxxx.
Xxx xxxxxxxxx xxxx $$XxxxXxxxxxxxXxxx$ xx xxxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: String
Parameter Sets: NotePropertySingleMemberSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxxxxxxXxxxx
Xxxx x xxxx xxxxxxxx xxxx xxx xxxxxxxxx xxxxx.

Xxx xxxx xxxxxxxxx xxxx xxx XxxxXxxxxxxxXxxx xxxxxxxxx.
Xxx xxxxxxxxx xxxx $$XxxxXxxxxxxxXxxxx$ xx xxxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: Object
Parameter Sets: NotePropertySingleMemberSet
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxxxxxxx x xxxx xxx xxx xxxx.

Xxxx xxx xxxx xx x xxxxx xx xxx Xxxxxx xxxxxxxxx xx x xxxx xxxx xxx x xxxx xxxxxxxxxxx$ xxx xxx xxxxx xxx xxxxx xxxx xx xxx xxxx.
Xxxxxxxxx$ xxx xxxx xxxx xxxx xx xxxxxxxx. Xxxx xxxxxxxxx xx xxxxxxxxx xxxx xxxx xxx xxxxx xxxxxx xx x XXXxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: String
Parameter Sets: TypeNameSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: MemberSet, NotePropertySingleMemberSet, NotePropertyMultiMemberSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxx xxxx xxx xxxxxx xxxx xx Xxx$Xxxxxx.

## XXXXXXX

### Xxxx xx Xxxxxx.Xxxxxx
Xxxx xxx xxx xxx XxxxXxxx xxxxxxxxx$ Xxx$Xxxxxx xxxxxxx xxx xxxxx$xxxxxxxx xxxxxx.
Xxxxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX
Xxx xxx xxx xxxxxxx xxxx xx XXXxxxxx xxxxxxx.
Xx xxxxxxxxx xxxxxxx xx xxxxxx xx x XXXxxxxx xxxxxx$ xxx xxx $xx$ xxxxxxxx.
Xxx xxxxxxx$ xx xxxx xx xxxxxx xxxxxx xx xxx $xxx xxxxxxxx$ xxxx $$xxx $xx $$XXXxxxxx$$$.

Xxx xxxxx xx xxx XxxxxxXxxx$ Xxxx$ Xxxxx$ xxx XxxxxxXxxxx xxxxxxxxxx xxx xxxxxxxx.
Xx xxx xxxx xxx xxxxxxxxx xxxxx$ xxx xxxxxxx xxxxxxxxx xxxxxx xxxx xxxxxx xx xxxx xxxxx$ XxxxxxXxxx$ Xxxx$ Xxxxx$ XxxxxxXxxxx.
Xx xxx xxxxxxx xxx xxxxxxxxx xxxxx$ xxx xxxxxxxxxx xxx xxxxxx xx xxx xxxxx.

Xxx xxx xxx xxx $xxxx xxxxxxxxx xxxxxxxx xx xxxxxx xxxxxx xxxx xxxxxx xxx xxxxxx xx xxx xxxxxxxxxx xxx xxxxxxx.
Xxx $xxxx xxxxxxxx xxxxxx xx xxx xxxxxxxx xx xxx xxxxxx xx xxxxx xxx xxxxxxxxxx xxx xxxxxxx xxx xxxxx xxxxx.
Xxx xxxx xxxxxxxxxxx xxxxx xxx $xxxx xxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

## XXXXXXX XXXXX

[Xxxxxx$Xxxxxx]()

[Xxx$Xxxxxx]()

[Xxxxxx$Xxxxxx]()

[Xxx$Xxxxxx]()

[xxxxx$Xxxxxxxxx$Xxxxxxxxx]()

