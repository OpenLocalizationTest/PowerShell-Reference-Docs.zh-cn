---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293965
schema: 2.0.0
---

# Get-Culture
## XXXXXXXX
Xxxx xxx xxxxxxx xxxxxxx xxx xx xxx xxxxxxxxx xxxxxx.

## XXXXXX

```
Get-Culture [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$Xxxxxxx xxxxxx xxxx xxxxxxxxxxx xxxxx xxx xxxxxxx xxxxxxx xxxxxxxx.
Xxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxx xxxxxxxx xxxxxxxx xx xxx xxxxxx$ xxxx xx xxx xxxxxxxx xxxxxx$ xxx xxx xxxxxxx xxxxxx xx xxxxx xxxx xx xxxxxxx$ xxxxxxxx$ xxx xxxxx.

Xxx xxx xxxx xxx xxx Xxx$XXXxxxxxx xxxxxx$ xxxxx xxxx xxx xxxxxxx xxxx xxxxxxxxx xxxxxxx xx xxx xxxxxx$ xxx xxx Xxx$Xxxxxxx xxxxxx xx xxx Xxxxxxxxxxxxx xxxxxx.
Xxx xxxx$xxxxxxxxx $XX$ xxxxxxx xxxxxxxxxx xxxxx xxxx xxxxxxx xxx xxxx xxx xxxx xxxxxxxxx xxxxxxxx$ xxxx xx xxxxx xxx xxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-culture
```

Xxxx xxxxxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxxx xxxxxxxx xx xxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$c = get-culture
PS C:\>$c | format-list -property *

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

PS C:\>$c.calendar

MinSupportedDateTime : 1/1/0001 12:00:00 AM
MaxSupportedDateTime : 12/31/9999 11:59:59 PM
AlgorithmType        : SolarCalendar
CalendarType         : Localized
Eras                 : {1}
TwoDigitYearMax      : 2029
IsReadOnly           : False

PS C:\>$c.datetimeformat

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

PS C:\>$c.datetimeformat.firstdayofweek
Sunday
```

Xxxx xxxxxxx xxxxxxxxxxxx xxx xxxx xxxxxx xx xxxx xx xxx xxxxxxx xxxxxx.
Xx xxxxx xxx xx xxxxxxx xxx xxxxxxxxxx xxx xxx$xxxxxxxxxx xx xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxx xxxxxxx xxxxxxxx xx xxx xxxxxxxx.
Xx xxxxxx xxx xxxxxxxxx xxxxxxx xxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxxx xxx xx xxx xxxxxxxxxx xx xxx xxxxxxx xxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xxxxxx xx $x xx xxx Xxxxxx$Xxxx xxxxxx.
Xx xxxx xxx Xxxxxxxx xxxxxxxxx xx xxxxxxx xxx $$$ xxxxxxxxxx xx xxx xxxxxx. $Xxxx xxxxxxx xxx xx xxxxxxxxxxx xx $$x $ xx $$.$

Xxx xxxxxxxxx xxxxxxxx xxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxx xxxxxx xx xxxxx xxx xxxxxxxx xx xxxxxxx xxx xxxxxx xx xxx xxxxxx xxxxxxxxxx.
Xxx xxx xxx xxxx xxxxxxxx xx xxxxxxx xxx xxxxx xx xxx xxxxxxxx xx xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxxxxxx xxx xxxxx xx xxx Xxxxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxxxxxx xxx xxxxx xx xxx XxxxXxxxXxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxx.

Xxxx xxxxxx xxxxxxxxxx xxxx xxxxxxxxxx.
Xxx xxxxx xxxxxxx xxxx xxx xxxxxxxx xx xxxxxxx xxx xxxxx xx xxx XxxxxXxxXxXxxx xxxxxxxx xx xxx XxxxXxxxXxxxxx xxxxxxxx.

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

### System.Globalization.CultureInfo
Xxx$Xxxxxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxx xxxxxxx.

## XXXXX
Xxx xxx xxxx xxx xxx $XxXxxxxxx xxx $XxXXXxxxxxx xxxxxxxxx.
Xxx $XxXxxxxxx xxxxxxxx xxxxxx xxx xxxx xx xxx xxxxxxx xxxxxxx xxx xxx $XxXXXxxxxxx xxxxxxxx xxxxxx xxx xxxx xx xxx xxxxxxx XX xxxxxxx.

## XXXXXXX XXXXX

[Set-Culture]()

[Get-UICulture]()

