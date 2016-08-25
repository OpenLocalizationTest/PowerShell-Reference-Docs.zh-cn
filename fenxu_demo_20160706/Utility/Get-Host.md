---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293970
schema: 2.0.0
---

# Get-Host
## XXXXXXXX
Xxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxx xxxx xxxxxxx.

## XXXXXX

```
Get-Host [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxx xxxxxx xxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxx xxxx xx xxxxxxx Xxxxxxx XxxxxXxxxx.

Xxx xxxxxxx xxxxxxx xxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xxxxxx xxx xxx xxxxxxx xxxxxx xxx xxxxxxxx xxxxxxxx xxxx xxx xxxx xx xxxxx$ xxx xxx xxxx xxxxxx xxxxxxxx x xxxxxx xx xxxxxxxxxxx$ xxxxxxxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxx xx Xxxxxxx XxxxxXxxxx xxxx xx xxxxxxxxx xxxxxxx xxx xxx xxxxxxx xxxxxxx xxx XX xxxxxxx xx Xxxxxxx XxxxxXxxxx.
Xxx xxx xxxx xxx xxxx  xxxxxx xx xxxxxxxxx xxxxxxxx xx xxx xxxx xxxxxxx xxxx xxxxxxxxx$ xxxx xx xxx xxxx xxx xxxxxxxxxx xxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-host

Name             : ConsoleHost
Version          : 2.0
InstanceId       : e4e0ab54-cc5e-4261-9117-4081f20ce7a2
UI               : System.Management.Automation.Internal.Host.InternalHostUserInterface
CurrentCulture   : en-US
CurrentUICulture : en-US
PrivateData      : Microsoft.PowerShell.ConsoleHost+ConsoleColorProxy
IsRunspacePushed : False
Runspace         : System.Management.Automation.Runspaces.LocalRunspace
```

Xxxx xxxxxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx$ xxxxx xx xxx xxxxxxx xxxx xxxxxxx xxx Xxxxxxx XxxxxXxxxx xx xxxx xxxxxxx.
Xx xxxxxxxx xxx xxxx xx xxx xxxx$ xxx xxxxxxx xx Xxxxxxx XxxxxXxxxx xxxx xx xxxxxxx xx xxx xxxx$ xxx xxxxxxx xxxxxxx xxx XX xxxxxxx.

Xxx Xxxxxxx$ XX$ XxxxxxxXxxxxxx$ XxxxxxxXXXxxxxxx$ XxxxxxxXxxx$ xxx Xxxxxxxx xxxxxxxxxx xxxx xxxxxxx xx xxxxxx xxxx xxxx xxxxxx xxxxxxxxxx.
Xxxxx xxxxxxxx xxxxxxx xxxxx xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$h = get-host
PS C:\>$win = $h.ui.rawui.windowsize
PS C:\>$win.height = 10
PS C:\>$win.width  = 10
PS C:\>$h.ui.rawui.set_windowsize($win)
```

Xxxx xxxxxxx xxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxx xx 00 xxxxxx xx 00 xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>(get-host).version | format-list -property *
Major         : 2
Minor         : 0
Build         : -1
Revision      : -1
MajorRevision : -1
MinorRevision : -1
```

Xxxx xxxxxxx xxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxx xx Xxxxxxx XxxxxXxxxx xxxxxxx xx xxx xxxx.
Xxx xxx xxxx$ xxx xxx xxxxxx$ xxxxx xxxxxx.

Xxx Xxxxxxx xxxxxxxx xx Xxx$Xxxx xxxxxxxx x Xxxxxx.Xxxxxxx xxxxxx.
Xxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xxxxxx xx xxx Xxxxxx$Xxxx xxxxxx.
Xxx Xxxxxx$Xxxx xxxxxxx xxxx xxx Xxxxxxxx xxxxxxxxx xxxx x xxxxx xx xxx $$$ xx xxxxxxx xxx xx xxx xxxxxxxxxx xxx xxxxxxxx xxxxxx xx xxx xxxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>(get-host).currentculture | format-list -property *

Parent                         : en
LCID                           : 1033
KeyboardLayoutId               : 1033
Name                           : en-US
IetfLanguageTag                : en-US
DisplayName                    : English (United States)
NativeName                     : English (United States)
EnglishName                    : English (United States)
TwoLetterISOLanguageName       : en
ThreeLetterISOLanguageName     : eng
ThreeLetterWindowsLanguageName : ENU
CompareInfo                    : CompareInfo - 1033
TextInfo                       : TextInfo - 1033
IsNeutralCulture               : False
CultureTypes                   : SpecificCultures, InstalledWin32Cultures, FrameworkCultures
NumberFormat                   : System.Globalization.NumberFormatInfo
DateTimeFormat                 : System.Globalization.DateTimeFormatInfo
Calendar                       : System.Globalization.GregorianCalendar
OptionalCalendars              : {System.Globalization.GregorianCalendar, System.Globalization.GregorianCalendar}
UseUserOverride                : True
IsReadOnly                     : False
```

Xxxx xxxxxxx xxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxx xxxxxxx xxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xx xxx xxxx.
Xxxx xx xxx xxxx xxxxxxxxxxx xxxx xx xxxxxxxx xx xxx Xxx$Xxxxxxx xxxxxx.

$Xxxxxxxxx$ xxx XxxxxxxXXXxxxxxx xxxxxxxx xxxxxxx xxx xxxx xxxxxx xxxx Xxx$XXXxxxxxx xxxxxxx.$

Xxx XxxxxxxXxxxxxx xxxxxxxx xx xxx xxxx xxxxxx xxxxxxxx x  Xxxxxx.Xxxxxxxxxxxxx.XxxxxxxXxxx xxxxxx.
Xxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx XxxxxxxXxxx xxxxxx xx xxx Xxxxxx$Xxxx xxxxxx.
Xxx Xxxxxx$Xxxx xxxxxxx xxxx xxx Xxxxxxxx xxxxxxxxx xxxx x xxxxx xx xxx $$$ xx xxxxxxx xxx xx xxx xxxxxxxxxx xxx xxxxxxxx xxxxxx xx xxx XxxxxxxXxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>(get-host).currentculture.DateTimeFormat | format-list -property *

AMDesignator                     : AM
Calendar                         : System.Globalization.GregorianCalendar
DateSeparator                    : /
FirstDayOfWeek                   : Sunday
CalendarWeekRule                 : FirstDay
FullDateTimePattern              : dddd, MMMM dd, yyyy h:mm:ss tt
LongDatePattern                  : dddd, MMMM dd, yyyy
LongTimePattern                  : h:mm:ss tt
MonthDayPattern                  : MMMM dd
PMDesignator                     : PM
RFC1123Pattern                   : ddd, dd MMM yyyy HH':'mm':'ss 'GMT'
ShortDatePattern                 : M/d/yyyy
ShortTimePattern                 : h:mm tt
SortableDateTimePattern          : yyyy'-'MM'-'dd'T'HH':'mm':'ss
TimeSeparator                    : :
UniversalSortableDateTimePattern : yyyy'-'MM'-'dd HH':'mm':'ss'Z'
YearMonthPattern                 : MMMM, yyyy
AbbreviatedDayNames              : {Sun, Mon, Tue, Wed...}
ShortestDayNames                 : {Su, Mo, Tu, We...}
DayNames                         : {Sunday, Monday, Tuesday, Wednesday...}
AbbreviatedMonthNames            : {Jan, Feb, Mar, Apr...}
MonthNames                       : {January, February, March, April...}
IsReadOnly                       : False
NativeCalendarName               : Gregorian Calendar
AbbreviatedMonthGenitiveNames    : {Jan, Feb, Mar, Apr...}
MonthGenitiveNames               : {January, February, March, April...}
```

Xxxx xxxxxxx xxxxxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx XxxxXxxxXxxxxx xx xxx xxxxxxx xxxxxxx xxxx xx xxxxx xxxx xxx Xxxxxxx XxxxxXxxxx.

Xxx XxxxxxxXxxxxxx xxxxxxxx xx xxx xxxx xxxxxx xxxxxxxx x XxxxxxxXxxx xxxxxx xxxx$ xx xxxx$ xxx xxxx xxxxxx xxxxxxxxxx.
Xxxxx xxxx$ xxx XxxxXxxxXxxxxx xxxxxxxx xxxxxxxx x XxxxXxxxXxxxxxXxxx xxxxxx xxxx xxxx xxxxxx xxxxxxxxxx.

Xx xxxx xxx xxxx xx xx xxxxxx xxxx xx xxxxxx xx xx xxxxxx xxxxxxxx$ xxx xxx Xxx$Xxxxxx xxxxxx.
Xx xxxxxxx xxx xxxxxxxx xxxxxx xx xxx xxxxxx$ xxx xxx Xxxxxx$Xxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>(get-host).ui.rawui | format-list -property *

ForegroundColor       : DarkYellow
BackgroundColor       : DarkBlue
CursorPosition        : 0,390
WindowPosition        : 0,341
CursorSize            : 25
BufferSize            : 120,3000
WindowSize            : 120,50
MaxWindowSize         : 120,81
MaxPhysicalWindowSize : 182,81
KeyAvailable          : False
WindowTitle           : Windows PowerShell 2.0 (04/11/2008 00:08:14)
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxxxx xx xxx XxxXX xxxxxxxx xx xxx xxxx xxxxxx.
Xx xxxxxxxx xxxxx xxxxxx$ xxx xxx xxxxxx xxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>(get-host).ui.rawui.backgroundcolor = "Black"
PS C:\>cls
```

Xxxxx xxxxxxxx xxxxxx xxx xxxxxxxxxx xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xx xxxxx.
Xxx $xxx$ xxxxxxx xx xx xxxxx xxx xxx Xxxxx$Xxxx xxxxxxxx$ xxxxx xxxxxx xxx xxxxxx xxx xxxxxxx xxx xxxxx xxxxxx xx xxx xxx xxxxx.

Xxxx xxxxxx xx xxxxxxxxx xxxx xx xxx xxxxxxx xxxxxxx.
Xx xxxxxx xxx xxxxxxxxxx xxxxx xx xxx xxxxxxx xxx xxx xxxxxxxx$ xxx xxx xxxxxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$host.privatedata.errorbackgroundcolor = "white"
```

Xxxx xxxxxxx xxxxxxx xxx xxxxxxxxxx xxxxx xx xxxxx xxxxxxxx xx xxxxx.

Xxxx xxxxxxx xxxx xxx $xxxx xxxxxxxxx xxxxxxxx$ xxxxx xxxxxxxx xxx xxxx xxxxxx xxx xxx xxxxxxx xxxx xxxxxxx.
Xxx$Xxxx xxxxxxx xxx xxxx xxxxxx xxxx $xxxx xxxxxxxx$ xx xxx xxx xxx xxxx xxxxxxxxxxxxxxx.

Xxxx xxxxxxx xxxx xxx XxxxxxxXxxx xxxxxxxx xx $xxxx xx xxx XxxxxXxxxxxxxxxXxxxx xxxxxxxx.
Xx xxx xxx xx xxx xxxxxxxxxx xx xxx xxxxxx xx xxx $xxxx.xxxxxxxxxxx xxxxxxxx$ xxxx $$xxxx.xxxxxxxxxxx $ xxxxxx$xxxx $ $.

## XXXXXXXXXX

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

## XXXXXX

### None
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### System.Management.Automation.Internal.Host.InternalHost
Xxx$Xxxx xxxxxxx x Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.Xxxxxxxx.Xxxx.XxxxxxxxXxxx xxxxxx.

## XXXXX
Xxx $xxxx xxxxxxxxx xxxxxxxx xxxxxxxx xxx xxxx xxxxxx xxxx Xxx$Xxxx xxxxxxx$ xxx xxx xxx xxx xx xx xxx xxxx xxx. Xxxxxxxxx$ xxx $XXXxxxxxx xxx $XXXXXxxxxxx xxxxxxxxx xxxxxxxxx xxxxxxx xxx xxxx xxxxxxx xxxx xxx XxxxxxxXxxxxxx xxx XxxxxxxXXXxxxxxx xxxxxxxxxx xx xxx xxxx xxxxxx xxxxxxx.
Xxx xxx xxx xxxxx xxxxxxxx xxxxxxxxxxxxxxx.

Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxx$Xxxxxxxxx.

## XXXXXXX XXXXX

[Clear-Host]()

[Out-Host]()

[Read-Host]()

[Write-Host]()

