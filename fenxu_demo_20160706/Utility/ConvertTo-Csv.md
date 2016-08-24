---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293949
schema: 2.0.0
---

# XxxxxxxXx$Xxx
## XXXXXXXX
Xxxxxxxx xxxxxxx xxxx x xxxxxx xx xxxxx$xxxxxxxxx xxxxx $XXX$ xxxxxxxx$xxxxxx xxxxxxx.

## XXXXXX

### Xxxxxxxxx $Xxxxxxx$
```
ConvertTo-Csv [-InputObject] <PSObject> [[-Delimiter] <Char>] [-NoTypeInformation]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### XxxXxxxxxx
```
ConvertTo-Csv [-InputObject] <PSObject> [-UseCulture] [-NoTypeInformation]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx XxxxxxxXx$XXX xxxxxx xxxxxxx x xxxxxx xx xxxxx$xxxxxxxxx $XXX$ xxxxxxx xxxx xxxxxxxxxx xxx xxxxxxx xxxx xxx xxxxxx.
Xxx xxx xxxx xxx xxx XxxxxxxXxxx$XXX xxxxxx xx xx$xxxxxx xxxxxxx xxxx xxx XXX xxxxxxx.
Xxx xxxxxxxxx xxxxxxx xxx XXX xxxxxxxx xx xxx xxxxxxxx xxxxxxx xxxx xxxxxxx xx xxxxxx xxxxxxxxxxxxxxx xx xxx xxxxxxxx xxxxxx xxx xx xxxxxxx.

Xxx xxx xxxx xxx xxx X$Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.Xxxxxx$Xxx xxx X$Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.Xxxxxx$Xxx xxxxxxx xx xxxxxxx xxxxxxx xx XXX xxxxxxx $xxx xxxx$.
Xxxxxx$XXX xx xxx xxxx xx XxxxxxxXx$XXX$ xxxxxx xxxx xx xxxxx xxx XXX xxxxxxx xx x xxxx.

Xxx xxx xxx xxx xxxxxxxxxx xx xxx XxxxxxxXx$XXX xxxxxx xx xxxxxxx x xxxxxxxxx xxxxx xxxx x xxxxx xx xx xxxxxx XxxxxxxXx$XXX xx xxx xxx xxxxxxx xxxxxxxxx xxx xxx xxxxxxx xxxxxxx.

Xxx xxxx xxxxxxxxxxx$ xxx Xxxxxx$XXX$ xxx xxx xxx Xxxxx xxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process powershell | convertto-csv
#TYPE System.Diagnostics.Process
"__NounName","Name","Handles","VM","WS","PM","NPM","Path","Company","CPU","FileVersion","ProductVersion","Description",
"Product","BasePriority","ExitCode","HasExited","ExitTime","Handle","HandleCount","Id","MachineName","MainWindowHandle"
,"MainWindowTitle","MainModule","MaxWorkingSet","MinWorkingSet","Modules","NonpagedSystemMemorySize","NonpagedSystemMem
orySize64","PagedMemorySize","PagedMemorySize64","PagedSystemMemorySize","PagedSystemMemorySize64","PeakPagedMemorySize
","PeakPagedMemorySize64","PeakWorkingSet","PeakWorkingSet64","PeakVirtualMemorySize","PeakVirtualMemorySize64","Priori
tyBoostEnabled","PriorityClass","PrivateMemorySize","PrivateMemorySize64","PrivilegedProcessorTime","ProcessName","Proc
essorAffinity","Responding","SessionId","StartInfo","StartTime","SynchronizingObject","Threads","TotalProcessorTime","U
serProcessorTime","VirtualMemorySize","VirtualMemorySize64","EnableRaisingEvents","StandardInput","StandardOutput","Sta
ndardError","WorkingSet","WorkingSet64","Site","Container"
"Process","powershell","216","597544960","60399616","63197184","21692","C:\WINDOWS\system32\WindowsPowerShell\v1.0\powe
rshell.exe","Microsoft Corporation","3.4788223","6.1.6587.1 (fbl_srv_powershell(nigels).070711-0102)","6.1.6587.1","Win
dows PowerShell","Microsoft® Windows® Operating System","8",,"False",,"860","216","5132",".","5636936","Windows PowerSh
ell 2.0 (04/17/2008 00:10:40)","System.Diagnostics.ProcessModule (powershell.exe)","1413120","204800","System.Diagnosti
cs.ProcessModuleCollection","21692","21692","63197184","63197184","320080","320080","63868928","63868928","60715008","6
0715008","598642688","598642688","True","Normal","63197184","63197184","00:00:00.2028013","powershell","15","True","1",
"System.Diagnostics.ProcessStartInfo","4/21/2008 3:49:19 PM",,"System.Diagnostics.ProcessThreadCollection","00:00:03.51
00225","00:00:03.3072212","597544960","597544960","False",,,,"60399616","60399616",,
```

Xxxx xxxxxxx xxxxxxxx x xxxxxx xxxxxxx xxxxxx xx XXX xxxxxx.
Xxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx XxxxxXxxxx xxxxxxx xx xxx xxxxx xxxxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xx xxx XxxxxxxXx$XXX xxxxxx$ xxxxx xxxxxxxx xx xx x xxxxxx xx xxxxx$xxxxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$date = get-date
PS C:\>convertto-csv -inputobject $date -delimiter ";" -notypeinformation
```

Xxxx xxxxxxx xxxxxxxx x xxxx xxxxxx xx XXX xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxx xxxxxx xx xxx xxx xxxxxxx xxxx.
Xx xxxxx xx xx xxx $xxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx XxxxxxxXx$XXX xxxxxx xx xxxxxxx xxx XxxxXxxx xxxxxx xx xxx $xxxx xxxxxxxx xx XXX xxxxxx.
Xxx xxxxxxx xxxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxx xx xx xxxxxxxxx.
Xx xxxx xxx Xxxxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxxxxx xxxx xxxxxxxxx xxx xxxxxx xxxxxxxxxx.
Xx xxxx xxx XxXxxxXxxxxxxxxxx xxxxxxxxx xx xxxxxxxx xxx $XXXX xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-eventlog -log "windows powershell" | convertto-csv -useculture
```

Xxxx xxxxxxx xxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxxx xxx xx xxx xxxxx xxxxxxxx xx x xxxxxx xx XXX xxxxxxx.

Xxx xxxxxxx xxxx xxx Xxx$XxxxxXxx xxxxxx xx xxx xxx xxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxx.
X xxxxxxxx xxxxxxxx $$$ xxxxx xxx xxxxxx xx xxx XxxxxxxXx$XXX xxxxxx$ xxxxx xxxxxxxx xxx xxxxxx xx XXX xxxxxx.
Xxx xxxxxxx xxxx xxx XxxXxxxxxx xxxxxxxxx$ xxxxx xxxx xxx xxxx xxxxxxxxx xxx xxx xxxxxxx xxxxxxx xx xxx xxxxxxxxx.

## XXXXXXXXXX

### $Xxxxxxxxx
Xxxxxxxxx x xxxxxxxxx xx xxxxxxxx xxx xxxxxxxx xxxxxx.
Xxx xxxxxxx xx x xxxxx $$$.
Xxxxx x xxxxxxxxx$ xxxx xx x xxxxx $$$.

Xx xxxxxxx x xxxxxxxxx $$$$ xxxxxxx xx xx xxxxxxxxx xxxxx.
Xxxxxxxxx$ xx xxxx xx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxxxx.

```yaml
Type: Char
Parameter Sets: Delimiter
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxxxXxxxxx
Xx xxxxxxx x xxxxxxxxx $$$$ xxxxxxx xx xx xxxxxxxxx xxxxx.
Xxxxxxxxx$ xx xxxx xx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxxxx.

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
Xx xxxxxxx x xxxxxxxxx $$$$ xxxxxxx xx xx xxxxxxxxx xxxxx.
Xxxxxxxxx$ xx xxxx xx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxxxx.

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
Xxxxxxxxx xxx xxxxxxx xx xxxxxx xx XXX xxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.
Xxx xxx xxxx xxxx xxxxxxx xx XxxxxxxXx$XXX.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### $XxXxxxXxxxxxxxxxx
Xxxxx xxx xxxx xxxxxxxxxxx xxxxxx xxxx xxx xxxxxx.
Xx xxxxxxx$ xxx xxxxxx xx xxx xxxxxx xxxxxxxx $$XXXX $ xxxxxxxx xx xxx xxxxx$xxxxxxxxx xxxx xx xxx xxxxxx xxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: NTI

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxxxxxx
Xxxx xxx xxxx xxxxxxxxx xxx xxx xxxxxxx xxxxxxx xx xxx xxxx xxxxxxxxx.
Xxx xxxxxxx xx x xxxxx $$$.

Xxxx xxxxxxxxx xx xxxx xxxxxx xx xxxxxxx xxxx xxx xxxxx xxxxxxxxxxx xx xxxxx xxxxxxxxx.
Xx xxxx xxx xxxx xxxxxxxxx xxx x xxxxxxx$ xxx xxx xxxxxxxxx xxxxxxx$ $Xxx$Xxxxxxx$.XxxxXxxx.XxxxXxxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UseCulture
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XXXxxxxx
Xxx xxx xxxx xxx xxxxxx xxxx xxx xx Xxxxxxxx Xxxx Xxxxxx $XXX$ xxxxxxx xx XxxxxxxXx$XXX.

## XXXXXXX

### Xxxxxx.Xxxxxx
Xxx XXX xxxxxx xx xxxxxxxx xx x xxxxxxxxxx xx xxxxxxx.

## XXXXX
Xx XXX xxxxxx$ xxxx xxxxxx xx xxxxxxxxxxx xx x xxxxx$xxxxxxxxx xxxx xx xxx xxxxxxxx xxxxx.
Xxx xxxxxxxx xxxxxx xxx xxxxxxxxx xx xxxxxxx $xx xxxxx xxx XxXxxxxx$$ xxxxxx xx xxx xxxxxx$$ xx xxxx xxx xxxxxxxxx xxxxxxxxxxx xx xxx xxxx xx xxx xxxxxxxx xxxxx.
XxxxxxxXx$XXX xxxx xxx xxxxxx xxx xxxxxxx xx xxx xxxxxx.

Xxx xxxxxx xx xxx xxxxxxxxx XXX xxxxxxx xx xx xxxxxxx$

$$ Xxx xxxxx xxxxxx xxxxxxxx xx $$XXXX $ xxxxxxxx xx xxx xxxxx$xxxxxxxxx xxxx xx xxx xxxxxx xxxx$ xxxx xx $XXXX Xxxxxx.Xxxxxxxxxxx.Xxxxxxx. Xx xxxxxxxx xxxx xxxxxx$ xxx xxx XxXxxxXxxxxxxxxxx xxxxxxxxx.
$$ Xxx xxxx xxxxxx xxxxxxxxxx xxx xxxxxx xxxxxxx. Xx xxxxxxxx x xxxxx$xxxxxxxxx xxxx xx xxx xxxxx xx xxx xxx xxxxxxxxxx xx xxx xxxxx xxxxxx.
$$ Xxx xxxxxxxxx xxxxxxx xxxxxxx xx xxxxx$xxxxxxxxx xxxxx xx xxx xxxxxxxx xxxxxx xx xxxx xxxxxx.

Xxxx xxx xxxxxx xxxxxxxx xxxxxxx xx XxxxxxxXx$XXX$ XxxxxxxXx$XXX xxxxxx xxx xxxxxxx xxxxx xx xxx xxxxxxxxxx xx xxx xxxxx xxxxxx xxxx xxx xxxxxx.
Xx xxx xxxxxxxxx xxxxxxx xx xxx xxxx xxx xx xxx xxxxxxxxx xxxxxxxxxx$ xxx xxxxxxxx xxxxx xx xxxx xxxxxx xx xxxx$ xx xxxxxxxxxxx xx xxx xxxxxxxxxxx xxxxxx.
Xx xxx xxxxxxxxx xxxxxxx xxxx xxxxxxxxxx xxxxxxxxxx$ xxxxx xxxxxxxx xxxxxx xxx xxxxxxx.

## XXXXXXX XXXXX

[XxxxxxxXxxx$Xxx]()

[Xxxxxx$Xxx]()

[Xxxxxx$Xxx]()

