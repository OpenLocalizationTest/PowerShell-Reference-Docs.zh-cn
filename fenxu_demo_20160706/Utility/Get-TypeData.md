---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293976
schema: 2.0.0
---

# Get-TypeData
## XXXXXXXX
Xxxx xxx xxxxxxxx xxxx xxxx xx xxx xxxxxxx xxxxxxx.

## XXXXXX

```
Get-TypeData [[-TypeName] <String[]>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$XxxxXxxx xxxxxx xxxx xxx xxxxxxxx xxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xxxx xxxxxxxx xxxx xxxx xxxx xxx xxxxx xx xxx xxxxxxx xx Xxxxx.xx0xxx xxxx xxx xxxxxxx xxxx xxxx xxxx xxx xxxxx xx xxxxx xxx xxxxxxxxx xx xxx Xxxxxx$XxxxXxxx xxxxxx.

Xxx xxx xxx xxx xxxxxxxx xxxx xxxx xxxx Xxx$XxxxXxxx xxxxxxx xx xxxxxxx xxx xxxx xxxx xx xxx xxxxxxx xxx xxxx xx xx xxx Xxxxxx$XxxxXxxx xxx Xxxxxx$XxxxXxxx xxxxxxx.

Xxxxxxxx xxxx xxxx xxxx xxxxxxxxxx xxx xxxxxxx xx xxxxxxx xx Xxxxxxx XxxxxXxxxx.
Xxx xxx xxx xxx xxxxx xxxxxxxxxx xxx xxxxxxx xx xxx xxxx xxxx xxxx xxx xxxxx xxx xxx xxxxxxxxxx xxx xxxxxxx xxxx xxx xxxxxxx xx xxx xxxxxx xxxx.
Xxxxxxx$ xxxx xxxxxxx xxxxxxx$ xx xxxxx xxxx xxx xxxxx xxxxxxxxxx xxx xxxxxxx xxxxx xxx xx xxxxxxx xx xxxxx Xxxxxxx XxxxxXxxxx xxxxxxx.

Xxx xxxx xxxxxxxxxxx xxxxx Xxxxx.xx0xxx xxxxx$ xxx xxxxx$Xxxxx.xx0xxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.
Xxx xxxx xxxxxxxxxxx xxxxx xxxxxxx xxxx xxxx xxxx xxx Xxxxxx$XxxxXxxx xxxxxx xxxx$ xxx Xxxxxx$XxxxXxxx.

Xxxx xxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

## XXXXXXXX

### Xxxxxxx 0
```
PS C:\>Get-TypeData
```

Xxxx xxxxxxx xxxx xxx xxxxxxxx xxxx xxxx xx xxx xxxxxxx xxxxxxx.

### Xxxxxxx 0
```
PS C:\>"*Eventing*" | Get-TypeData
TypeName                                                              Members--------                                                              -------System.Diagnostics.Eventing.Reader.EventLogConfiguration              {}System.Diagnostics.Eventing.Reader.EventLogRecord                    {}System.Diagnostics.Eventing.Reader.ProviderMetadata                   {[ProviderName, System.Management.Automation.Runspaces.AliasProper...
```

Xxxx xxxxxxx xxxx xxx xxxxx xx xxx xxxxxxx xxxxxxx xxxx xxxx xxxxx xxxx xxxxxxx $Xxxxxxxx$.

### 0$
```
PS C:\>(Get-TypeData *EventLogEntry*).Members.EventID
GetScriptBlock                     SetScriptBlock                                               IsHidden Name

--------------                     --------------                                               -------- ----
$this.get_EventID() -band 0xFFFF                                                                   False EventID
```

Xxxx xxxxxxx xxxx xxx xxxxxx xxxxx xxxx xxxxxxx xxx xxxxx xx xxx XxxxxXX xxxxxxxx xx XxxxxXxxXxxxx xxxxxxx.

### Xxxxxxx 0
```
PS C:\>(Get-TypeData -TypeName System.DateTime).Members["DateTime"].GetScriptBlock
if ((& { Set-StrictMode -Version 1; $this.DisplayHint }) -ieq  "Date")                    
{                        
    "{0}" -f $this.ToLongDateString()                    
}
elseif ((& { Set-StrictMode -Version 1; $this.DisplayHint }) -ieq "Time")                    
{                        
    "{0}" -f  $this.ToLongTimeString()                    
}                    
else                    
{                        
    "{0} {1}" -f $this.ToLongDateString(), $this.ToLongTimeString()                    
}
```

Xxxx xxxxxxx xxxx xxx xxxxxx xxxxx xxxx xxxxxxx xxx XxxxXxxx xxxxxxxx xx Xxxxxx.XxxxXxxx xxxxxxx xx Xxxxxxx XxxxxXxxxx.

Xxx xxxxxxx xxxx xxx Xxx$XxxxXxxx xxxxxx xx xxx xxx xxxxxxxx xxxx xxxx xxx xxx Xxxxxx.XxxxXxxx xxxx.
Xxx xxxxxxx xxxx xxx Xxxxxxx xxxxxxxx xx xxx XxxxXxxx xxxxxx.

Xxx Xxxxxxx xxxxxxxx xxxxxxxx  x xxxx xxxxx xx xxxxxxxxxx xxx xxxxxxx xxxx xxx xxxxxxx xx xxxxxxxx xxxx xxxx.
Xxxx xxx xx xxx Xxxxxxx xxxx xxxxx xx x xxxxxxxx xx xxxxxx xxxx xxx xxxx xxxxx xx xxx xxxxxxxxxx xx xxx xxxxxxxx xx xxxxxx xxxxx.

Xxx xxxxxxx xxxx xxx XxxxXxxx xxx xx Xxxxxxx xxx xxx XxxXxxxxxXxxxx xxxxxxxx xxxxx.

Xxx xxxxxx xxxxx xxx xxxxxx xxxxx xxxx xxxxxxx xxx xxxxx xx xxx XxxxXxxx xxxxxxxx xx xxxxx Xxxxxx.XxxxXxxx xxxxxx xx Xxxxxxx XxxxxXxxxx.

### Xxxxxxx 0
```
PS C:\>dir $pshome\*types.ps1xml -Recurse | Select-String "EventLogEntry"
C:\WINDOWS\System32\WindowsPowerShell\v1.0\DotNetTypes.format.ps1xml:180: 
<Name>System.Diagnostics.EventLogEntry</Name>
C:\WINDOWS\System32\WindowsPowerShell\v1.0\DotNetTypes.format.ps1xml:182: 
<TypeName>System.Diagnostics.EventLogEntry</TypeName>
C:\WINDOWS\System32\WindowsPowerShell\v1.0\DotNetTypes.format.ps1xml:801: 
<Name>System.Diagnostics.EventLogEntry</Name>
C:\WINDOWS\System32\WindowsPowerShell\v1.0\DotNetTypes.format.ps1xml:803: 
<TypeName>System.Diagnostics.EventLogEntry</TypeName>
C:\WINDOWS\System32\WindowsPowerShell\v1.0\types.ps1xml:433: 
<Name>System.Diagnostics.EventLogEntry</Name>
```

Xxxx xxxxxxx xxxxx xxx Xxxxx.xx0xxx xxxx xxxx xxxxx xxxxxxxx xxxx xxxx xxx xxx XxxxxXxxXxxxx xxxx xx xxx xxxxxxx.
Xxxx xxxxxxx xxxx xxx Xxx$XxxxxXxxx xxxxxx $xxxxx $ $xxx$$ xx xxxxxxx x xxxxxxxxx xxxxxx xxx Xxxxx.xx0xxx xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxxxxx xxxxxxxxx $$xxxxxx$ xxx xxx xxxxxxxxxxxxxx.
Xxx xxxxxxx xxxxx xxx Xxxxx.xx0xxx xxxxx xx xxx Xxxxxx$Xxxxxx xxxxxx$ xxxxx xxxx x xxxx$xxxx xxxxxx xxx xxx $XxxxxXxxXxxxx$ xxxx xxxx xx xxx xxxxx xxx xxxxxxx xxx xxxxxxx.

## XXXXXXXXXX

### -InformationAction
Xxxxx xxxx xxxxx xx x xxxx xxxxxxxx.
Xxxx xxxxx $xx xxxx xxxxxxxx xxxx xxxxxxxx xxxxxxxxxx$ xxx xxxxxxxx$ xxxx xxx xxxxx xx xxx Xxxxxx xxxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx xxx xxx xxxxxxxxx xxxx $$XxxxXxxx$ xx xxxxxxxx.
Xxx xxx xxxx xxxx xxxx xxxxx xx Xxx$XxxxXxxx.

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
Xxxxx xxxx xxxxx xx x xxxx xxxxxxxx.
Xxxx xxxxx $xx xxxx xxxxxxxx xxxx xxxxxxxx xxxxxxxxxx$ xxx xxxxxxxx$ xxxx xxx xxxxx xx xxx Xxxxxx xxxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx xxx xxx xxxxxxxxx xxxx $$XxxxXxxx$ xx xxxxxxxx.
Xxx xxx xxxx xxxx xxxx xxxxx xx Xxx$XxxxXxxx.

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

### -TypeName
Xxxx xxxx xxxx xxxx xxx xxx xxxxx xxxx xxx xxxxxxxxx xxxxx.
Xx xxxxxxx$ Xxx$XxxxXxxx xxxx xxx xxxxx xx xxx xxxxxxx.

Xxxxx xxxx xxxxx xx x xxxx xxxxxxxx.
Xxxx xxxxx $xx xxxx xxxxxxxx xxxx xxxxxxxx xxxxxxxxxx$ xxx xxxxxxxx$ xxxx xxx xxxxx xx xxx Xxxxxx xxxxxxxxx.
Xxxxxxxxx xxx xxxxxxxxx xxx xxx xxxxxxxxx xxxx $$XxxxXxxx$ xx xxxxxxxx.
Xxx xxx xxxx xxxx xxxx xxxxx xx Xxx$XxxxXxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## XXXXXX

### System.String
Xxx xxx xxxx xxxx xxxxx xx Xxx$XxxxXxxx.

## XXXXXXX

### System.Management.Automation.Runspaces.TypeData

## XXXXX
Xxx$XxxxXxxx xxxx xxxx xxx xxxxxxxx xxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxxx xxx xxx xxxxxxxx xxxx xxxx xxxx xx xx xxx xxxxxxxx$ xxx xxx xxx xxxx xxxxx xx xxx xxxxxxx xxxxxxx$ xxxx xx xxxxxxxx xxxxx xxxx xxx xxxxxxx xx xxxxxxx xxxx xxxx xxx xxxx xxxxxxxx xxxx xxx xxxxxxx xxxxxxx.

## XXXXXXX XXXXX

[about_Types.ps1xml]()

[Remove-TypeData]()

[Update-TypeData]()

