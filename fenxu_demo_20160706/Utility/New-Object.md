---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293993
schema: 2.0.0
---

# New-Object
## XXXXXXXX
Xxxxxxx xx xxxxxxxx xx x Xxxxxxxxx .XXX Xxxxxxxxx xx XXX xxxxxx.

## XXXXXX

### Net (Default)
```
New-Object [-TypeName] <String> [[-ArgumentList] <Object[]>] [-Property <IDictionary>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### Com
```
New-Object [-ComObject] <String> [-Strict] [-Property <IDictionary>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxx xxxxxx xxxxxxx xx xxxxxxxx xx x .XXX Xxxxxxxxx xx XXX xxxxxx.

Xxx xxx xxxxxxx xxxxxx xxx xxxx xx x .XXX Xxxxxxxxx xxxxx xx x XxxxXX xx x XXX xxxxxx.
Xx xxxxxxx$ xxx xxxx xxx xxxxx xxxxxxxxx xxxx xx x .XXX Xxxxxxxxx xxxxx xxx xxx xxxxxx xxxxxxx x xxxxxxxxx xx xx xxxxxxxx xx xxxx xxxxx.
Xx xxxxxx xx xxxxxxxx xx x XXX xxxxxx$ xxx xxx XxxXxxxxx xxxxxxxxx xxx xxxxxxx xxx XxxxXX xx xxx xxxxxx xx xxx xxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>New-Object -TypeName System.Version -ArgumentList "1.2.3.4"
Major  Minor  Build  Revision

-----  -----  -----  --------

1      2      3      4
```

Xxxx xxxxxxx xxxxxxx x Xxxxxx.Xxxxxxx xxxxxx.
Xx xxxx x $0.0.0.0$ xxxxxx xx xxx xxxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$ie = New-Object -COMObject InternetExplorer.Application -Property @{Navigate2="www.microsoft.com"; Visible = $true}
```

Xxxx xxxxxxx xxxxxxx xx xxxxxxxx xx xxx XXX xxxxxx xxxx xxxxxxxxxx xxx Xxxxxxxx Xxxxxxxx xxxxxxxxxxx.
Xxx xxxxx xx xxx Xxxxxxxx xxxxxxxxx xx x xxxx xxxxx xxxx xxxxx xxx Xxxxxxxx0 xxxxxx xxx xxxx xxx Xxxxxxx xxxxxxxx xx xxx xxxxxx xx $xxxx xx xxxx xxx xxxxxxxxxxx xxxxxxx.

Xxxx xxxxxxx xx xxx xxxxxxxxxx xx xxx xxxxxxxxx$

$xx $ Xxx$Xxxxxx $XXXXxxxxx XxxxxxxxXxxxxxxx.Xxxxxxxxxxx

$xx.Xxxxxxxx0$$xxx.xxxxxxxxx.xxx$$

$xx.Xxxxxxx $ $xxxx

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$a=New-Object -COMObject Word.Application -Strict -Property @{Visible=$true}
New-Object : The object written to the pipeline is an instance of the type
"Microsoft.Office.Interop.Word.ApplicationClass" from the component's primary
interop assembly. If this type exposes different members than the IDispatch
members, scripts written to work with this object might not work if the
primary interop assembly is not installed.

At line:1 char:14
+ $a=New-Object  <<<< -COM Word.Application -Strict; $a.visible=$true
```

Xxxx xxxxxxx xxxxxxxxxxxx xxxx xxxxxx xxx Xxxxxx xxxxxxxxx xxxxxx xxx Xxx$Xxxxxx xxxxxx xx xxxxxxxx x xxx$xxxxxxxxxxx xxxxx xxxx xxx XXX xxxxxx xxxx xx xxxxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command uses the ComObject parameter of the New-Object cmdlet to create a COM object with the "Shell.Application" ProgID. It stores the resulting object in the $objShell variable.
PS C:\>$objshell = New-Object -COMObject "Shell.Application"

The second command pipes the $objShell variable to the Get-Member cmdlet, which displays the properties and methods of the COM object. Among the methods is the ToggleDesktop method.
PS C:\>$objshell | Get-Member
   TypeName: System.__ComObject#{866738b9-6cf2-4de8-8767-f794ebe74f4e}


Name                 MemberType Definition

----                 ---------- ----------

AddToRecent          Method     void AddToRecent (Variant, string)

BrowseForFolder      Method     Folder BrowseForFolder (int, string, int, Variant)

CanStartStopService  Method     Variant CanStartStopService (string)

CascadeWindows       Method     void CascadeWindows ()

ControlPanelItem     Method     void ControlPanelItem (string)

EjectPC              Method     void EjectPC ()

Explore              Method     void Explore (Variant)

ExplorerPolicy       Method     Variant ExplorerPolicy (string)

FileRun              Method     void FileRun ()

FindComputer         Method     void FindComputer ()

FindFiles            Method     void FindFiles ()

FindPrinter          Method     void FindPrinter (string, string, string)

GetSetting           Method     bool GetSetting (int)

GetSystemInformation Method     Variant GetSystemInformation (string)

Help                 Method     void Help ()

IsRestricted         Method     int IsRestricted (string, string)

IsServiceRunning     Method     Variant IsServiceRunning (string)

MinimizeAll          Method     void MinimizeAll ()

NameSpace            Method     Folder NameSpace (Variant)

Open                 Method     void Open (Variant)

RefreshMenu          Method     void RefreshMenu ()

ServiceStart         Method     Variant ServiceStart (string, Variant)

ServiceStop          Method     Variant ServiceStop (string, Variant)

SetTime              Method     void SetTime ()

ShellExecute         Method     void ShellExecute (string, Variant, Variant, Variant, Variant)

ShowBrowserBar       Method     Variant ShowBrowserBar (string, Variant)

ShutdownWindows      Method     void ShutdownWindows ()

Suspend              Method     void Suspend ()

TileHorizontally     Method     void TileHorizontally ()

TileVertically       Method     void TileVertically ()
ToggleDesktop        Method     void ToggleDesktop ()

TrayProperties       Method     void TrayProperties ()

UndoMinimizeALL      Method     void UndoMinimizeALL ()

Windows              Method     IDispatch Windows ()

WindowsSecurity      Method     void WindowsSecurity ()

WindowSwitcher       Method     void WindowSwitcher ()

Application          Property   IDispatch Application () {get}

Parent               Property   IDispatch Parent () {get}

The third command calls the ToggleDesktop method of the object to minimize the open windows on your desktop.
PS C:\>$objshell.ToggleDesktop()
```

Xxxx xxxxxxx xxxxx xxx xx xxxxxx xxx xxx x XXX xxxxxx xx xxxxxx xxxx Xxxxxxx xxxxxxx.

## XXXXXXXXXX

### -ArgumentList
Xxxxxxxxx x xxxx xx xxxxxxxxx xx xxxx xx xxx xxxxxxxxxxx xx xxx .XXX Xxxxxxxxx xxxxx.
Xxxxxxxx xxxxxxxx xx xxx xxxx xx xxxxx xxxxxx $$$.
Xxx xxxxx xxx XxxxxxxxXxxx xx Xxxx.

```yaml
Type: Object[]
Parameter Sets: Net
Aliases: Args

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ComObject
Xxxxxxxxx xxx xxxxxxxxxxxx xxxxxxxxxx $XxxxXX$ xx xxx XXX xxxxxx.

```yaml
Type: String
Parameter Sets: Com
Aliases: 

Required: True
Position: 1
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

### -Property
Xxxx xxxxxxxx xxxxxx xxx xxxxxxx xxxxxxx xx xxx xxx xxxxxx.

Xxxxx x xxxx xxxxx xx xxxxx xxx xxxx xxx xxx xxxxx xx xxxxxxxxxx xx xxxxxxx xxx xxx xxxxxx xxx xxxxxxxx xxxxxx xx xxxxxx xxxxxxxxx.
Xxx$Xxxxxx xxxxxxx xxx xxxxxx xxx xxxx xxxx xxxxxxxx xxxxx xxx xxxxxxx xxxx xxxxxx xx xxx xxxxx xxxx xxxx xxxxxx xx xxx xxxx xxxxx.

Xx xxx xxx xxxxxx xx xxxxxxx xxxx xxx XXXxxxxx xxxxx$ xxx xxx xxxxxxx x xxxxxxxx xxxx xxxx xxx xxxxx xx xxx xxxxxx$ Xxx$Xxxxxx xxxx xxx xxxxxxxxx xxxxxxxx xx xxx xxxxxx xx x XxxxXxxxxxxx.
Xx xxx xxxxxx xx xxx x XXXxxxxx$ xxx xxxxxxx xxxxxxxxx x xxx$xxxxxxxxxxx xxxxx.

```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Strict
Xxxxxxxxx x xxx$xxxxxxxxxxx xxxxx xxxx x XXX xxxxxx xxxx xxx xxxxxxx xx xxxxxx xxxx xx xxxxxxx xxxxxxxx.
Xxxx xxxxxxx xxxxxxxxxxxxx xxxxxx XXX xxxxxxx xxxx .XXX Xxxxxxxxx xxxxxxx xxxx XXX$xxxxxxxx xxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: Com
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TypeName
Xxxxxxxxx xxx xxxxx xxxxxxxxx xxxx xx xxx .XXX Xxxxxxxxx xxxxx.
Xxx xxxxxx xxxxxxx xxxx xxx XxxxXxxx xxxxxxxxx xxx xxx XxxXxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: Net
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### None
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### Object
Xxx$Xxxxxx xxxxxxx xxx xxxxxx xxxx xx xxxxxxx.

## XXXXX
Xxx$Xxxxxx xxxxxxxx xxx xxxx xxxxxxxx$xxxx xxxxxxxxxxxxx xx xxx XXXxxxxx XxxxxxXxxxxx xxxxxxxx.
X xxxxxxxxx xxxx Xxx xxxXxxxx $ XxxxxxXxxxxx$$Xxxxx.Xxxxxxxxxxx$$ xx XXXxxxxx xxx xx xxxxxxxxxx xx $xxxXxxxx $ Xxx$Xxxxxx $XXXXxxxxx $Xxxxx.Xxxxxxxxxxx$ xx Xxxxxxx XxxxxXxxxx.

Xxx$Xxxxxx xxxxxxx xxxx xxx xxxxxxxxxxxxx xxxxxxxxx xx xxx Xxxxxxx Xxxxxx Xxxx xxxxxxxxxxx xx xxxxxx xx xxxx xx xxxx xxxx .XXX Xxxxxxxxx xxxxxxx xxxx xxx xxxxxxx xxxx xxx xxxxxx xxxxxxx.

## XXXXXXX XXXXX

[Compare-Object]()

[ForEach-Object]()

[Group-Object]()

[Measure-Object]()

[Select-Object]()

[Sort-Object]()

[Tee-Object]()

[Where-Object]()

