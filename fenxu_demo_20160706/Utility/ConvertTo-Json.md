---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293951
schema: 2.0.0
---

# XxxxxxxXx$Xxxx
## XXXXXXXX
Xxxxxxxx xx xxxxxx xx x XXXX$xxxxxxxxx xxxxxx

## XXXXXX

```
ConvertTo-Json [-InputObject] <Object> [-Depth <Int32>] [-Compress] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx XxxxxxxXx$Xxxx xxxxxx xxxxxxxx xxx xxxxxx xx x xxxxxx xx XxxxXxxxxx Xxxxxx Xxxxxxxx $XXXX$ xxxxxx.
Xxx xxxxxxxxxx xxx xxxxxxxxx xx xxxxx xxxxx$ xxx xxxxx xxxxxx xxx xxxxxxxxx xx xxxxxxxx xxxxxx$ xxx xxx xxxxxxx xxx xxxxxxx.

Xxx xxx xxxx xxx xxx XxxxxxxXxxx$Xxxx xxxxxx xx xxxxxxx x XXXX$xxxxxxxxx xxxxxx xx x XXXX xxxxxx$ xxxxx xx xxxxxx xxxxxxx xx Xxxxxxx XxxxxXxxxx.

Xxxx xxx xxxxx xxx XXXX xxxxxxx xx XXX xx xxxxxxxxx xxxx xxx xxxxxxxxxxxxx xxxxxxx xxxxxxx xxx xxx$xxxxx xxxx.

Xxxx xxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

## XXXXXXXX

### Xxxxxxx 0
```
PS C:\>(Get-UICulture).Calendar | ConvertTo-Json

{

    "MinSupportedDateTime":  "\/Date(-62135568000000)\/", 

    "MaxSupportedDateTime":  "\/Date(253402300799999)\/", 

    "AlgorithmType":  1, 

    "CalendarType":  1, 

    "Eras":  [

                 1

             ], 

    "TwoDigitYearMax":  2029, 

    "IsReadOnly":  false

}
```

Xxxx xxxxxxx xxxx xxx XxxxxxxXx$Xxxx xxxxxx xx xxxxxxx x XxxxxxxxxXxxxxxxx xxxxxx xx x XXXX$xxxxxxxxx xxxxxx.

### Xxxxxxx 0
```
PS C:\>@{Account="User01";Domain="Domain01";Admin="True"} | ConvertTo-Json - Compress
{"Admin":"True","Account":"User01","Domain":"Domain01"}
```

Xxxx xxxxxxx xxxxx xxx xxxxxx xx xxxxx xxx Xxxxxxxx xxxxxxxxx xx XxxxxxxXx$Xxxx.
Xxx xxxxxxxxxxx xxxxxxx xxxx xxx xxxxxxxxxx xx xxx xxxxxx$ xxx xxx xxxxxxxx.

### Xxxxxxx 0
```
The first command uses the ConvertTo-Json cmdlet to convert a System.DateTime object from the Get-Date cmdlet to a JSON-formatted string. The command uses the Select-Object cmdlet to get all (*) of the properties of the DateTime object.The output shows the JSON string that ConvertTo-Json returned.
PS C:\>Get-Date | Select-Object -Property * | ConvertTo-Json

{

    "DisplayHint":  2, 

    "DateTime":  "Friday, January 13, 2012 8:06:16 PM",

    "Date":  "\/Date(1326441600000)\/", 

    "Day":  13, 

    "DayOfWeek":  5, 

    "DayOfYear":  13, 

    "Hour":  20, 

    "Kind":  2, 

    "Millisecond":  221, 

    "Minute":  6, 

    "Month":  1, 

    "Second":  16, 

    "Ticks":  634620819762218083, 

    "TimeOfDay":  {

                      "Ticks":  723762218083, 

                      "Days":  0, 

                      "Hours":  20, 

                      "Milliseconds":  221, 

                      "Minutes":  6, 

                      "Seconds":  16, 

                      "TotalDays":  0.83768775241087956, 

                      "TotalHours":  20.104506057861109, 

                      "TotalMilliseconds":  72376221.8083, 

                      "TotalMinutes":  1206.2703634716668, 

                      "TotalSeconds":  72376.22180829999

                  },

    "Year":  2012

}

The second command uses ConvertFrom-Json to convert the JSON string to a JSON object. 
PS C:\>Get-Date | Select-Object -Property * | ConvertTo-Json | ConvertFrom-Json

DisplayHint : 2

DateTime    : Friday, January 13, 2012 8:06:31 PM

Date        : 1/13/2012 8:00:00 AM

Day         : 13

DayOfWeek   : 5

DayOfYear   : 13

Hour        : 20

Kind        : 2

Millisecond : 400

Minute      : 6

Month       : 1

Second      : 31

Ticks       : 634620819914009002

TimeOfDay   : @{Ticks=723914009002; Days=0; Hours=20; Milliseconds=400;

 Minutes=6; Seconds=31; TotalDays=0.83786343634490734;
               TotalHours=20.108722472277776; TotalMilliseconds=72391400.900200009;
 TotalMinutes=1206.5233483366667;

              TotalSeconds=72391.4009002}

Year        : 2012
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx XxxxxxxXx$Xxxx xxx XxxxxxxXxxx$Xxxx xxxxxx xx xxxxxxx xx xxxxxx xx x XXXX xxxxxx xxx x XXXX xxxxxx.

### Xxxxxxx 0
```
PS C:\>$JsonSecurityHelp = Get-Content $pshome\Modules\Microsoft.PowerShell.Security\en-US\Microsoft.PowerShell.Security.dll-Help.xml | ConvertTo-Json
```

Xxxx xxxxxxx xxxx xxx XxxxxxxXx$Xxxx xxxxxx xx xxxxxxx x Xxxxxxx XxxxxXxxxx xxxx xxxx xxxx XXX xxxxxx xx XXXX xxxxxx.
Xxx xxx xxx x xxxxxxx xxxx xxxx xx xxx xxx xxxx xxxxx xxxxxxx xx x xxx xxxxxxx xxxxxxxxxxx.

## XXXXXXXXXX

### $Xxxxxxxx
Xxxxx xxxxx xxxxx xxx xxxxxxxx xxxxxxxxxx xx xxx xxxxxx xxxxxx.

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
Xxxxxxxxx xxx xxxx xxxxxx xx xxxxxxxxx xxxxxxx xxx xxxxxxxx xx xxx XXXX xxxxxxxxxxxxxx.
Xxx xxxxxxx xxxxx xx 0.

```yaml
Type: Int32
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

### $XxxxxXxxxxx
Xxxxxxxxx xxx xxxxxxx xx xxxxxxx xx XXXX xxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx$ xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.
Xxx xxx xxxx xxxx xx xxxxxx xx XxxxxxxXx$Xxxx.

Xxx XxxxxXxxxxx xxxxxxxxx xx xxxxxxxx$ xxx xxx xxxxx xxx xx xxxx $$xxxx$ xx xx xxxxx xxxxxx.
Xxxx xxx xxxxx xxxxxx xx $xxxx$ XxxxxxxXx$Xxxx xxxx xxx xxxxxxxx xxx xxxxxx.
Xxxx xxx xxxxx xxxxxx xx xx xxxxx xxxxxx$ XxxxxxxXx$Xxxx xxxxxxx xx xxxxx xxxxxx.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxx
Xxx xxx xxxx xxx xxxxxx xx XxxxxxxXx$Xxxx.

## XXXXXXX

### Xxxxxx.Xxxxxx

## XXXXX
Xxx XxxxxxxXx$Xxxx xxxxxx xx xxxxxxxxxxx xx xxxxx xxx XxxxXxxxxxXxxxxxxxxx xxxxx $xxxx$$$xxxx.xxxxxxxxx.xxx$xx$xx$xxxxxxx$xxxxxx.xxx.xxxxxx.xxxxxxxxxxxxx.xxxxxxxxxxxxxxxxxxxx$XX.000$.xxxx$.

## XXXXXXX XXXXX

[Xx Xxxxxxxxxxxx xx XxxxXxxxxx Xxxxxx Xxxxxxxx $XXXX$ xx XxxxXxxxxx xxx .XXX]()

[XxxxxxxXxxx$Xxxx]()

[Xxxxxx$XxxXxxxxxx]()

[Xxxxxx$XxxxXxxxxx]()

