---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293957
schema: 2.0.0
---

# Export-Csv
## XXXXXXXX
Xxxxxxxx xxxxxxx xxxx x xxxxxx xx xxxxx$xxxxxxxxx $XXX$ xxxxxxx xxx xxxxx xxx xxxxxxx xx x XXX xxxx.

## XXXXXX

### Delimiter (Default)
```
Export-Csv -InputObject <PSObject> [[-Path] <String>] [-LiteralPath <String>] [-Force] [-NoClobber]
 [-Encoding <String>] [-Append] [[-Delimiter] <Char>] [-NoTypeInformation]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

### UseCulture
```
Export-Csv -InputObject <PSObject> [[-Path] <String>] [-LiteralPath <String>] [-Force] [-NoClobber]
 [-Encoding <String>] [-Append] [-UseCulture] [-NoTypeInformation] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XXX xxxxxx xxxxxxx x XXX xxxx xx xxx xxxxxxx xxxx xxx xxxxxx.
Xxxx xxxxxx xx xxxxxxxxxxx xx x xxxx xx xxx xx xxx XXX.
Xxx xxx xxxxxxxx xx x xxxxx$xxxxxxxxx xxxx xx xxx xxxxxx xx xxxxxx xxxxxxxxxx.
Xxx xxx xxx xxxx xxxxxx xx xxxxxx xxxxxxxxxxxx xxx xxxxx xxxx xxxx xxxxxxxx xxxx xxxx XXX xxxxx xx xxxxx.

XXXX$ Xx xxx xxxxxx xxxxxxx xxxxxx xxxxxxx xxxx xx xxx Xxxxxx$XXX xxxxxx.
Xx xxx xx$ xxx xxxxxx xxxxxxxxxx xxx xxxxxxxxxxx xx xxx XXX xxxx$ xxxxxxx xx xxx xxxxxxxxxx xx xxx xxxxxxxx xxxxxxx.
Xx xxxxxx xxxx xxxxxxxx xxxxxxxxxx xx xx xxxxxx$ xxx xxx Xxxxxx$Xxxxxx xxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process wmiprvse | select-object basePriority,ID,SessionID,WorkingSet | export-csv -path data.csv
```

Xxxx xxxxxxx xxxxxxx x xxx xxxxxxxxxx xx xxx XxxXxxxx xxxxxxx xxx xxxxxxx xxxx xx x XXX xxxx xxxxx Xxxx.xxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | export-csv processes.csv
PS C:\>get-process | export-csv processes.csv

# In processes.csv
#TYPE System.Diagnostics.Process
__NounName,Name,Handles,VM,WS,PM,NPM,Path,Company,CPU,FileVersion,... Process,powershell,626,201666560,76058624,61943808,11960,C:\WINDOWS... Process,powershell,257,151920640,38322176,37052416,7836,C:\WINDOWS\...
```

Xxxx xxxxxxx xxxxxxx xxxxxxx xxxxxxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xx xxx Xxxxxxxxx.xxx xxxx xx xxx xxxxxxx xxxxxxxxx.
Xxxxxxx xx xxxx xxx xxxxxxx x xxxxxxxxx$ x xxxxx $$$ xx xxxx xx xxxxxxxx xxx xxxxxx xx xxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | export-csv processes.csv -Delimiter ";"

# In processes.csv
#TYPE System.Diagnostics.Process
__NounName;Name;Handles;VM;WS;PM;NPM;Path;Company;CPU;FileVersion;... Process;powershell;626;201666560;76058624;61943808;11960;C:\WINDOWS... Process;powershell;257;151920640;38322176;37052416;7836;C:\WINDOWS\...
```

Xxxx xxxxxxx xxxxxxx xxxxxxx xxxxxxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xx xxx Xxxxxxxxx.xxx xxxx xx xxx xxxxxxx xxxxxxxxx.
Xx xxxx xxx Xxxxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxxxxx $$$.
Xx x xxxxxx$ xxx xxxxxx xx xxx xxxx xxx xxxxxxxxx xx xxxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | export-csv processes.csv -UseCulture
```

Xxxx xxxxxxx xxxxxxx xxxxxxx xxxxxxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xx xxx Xxxxxxxxx.xxx xxxx xx xxx xxxxxxx xxxxxxxxx.
Xx xxxx xxx XxxXxxxxxx xxxxxxxxx xx xxxxxx Xxxxxx$XXX xx xxx xxx xxxxxxxxx xxxxxxxxx xx xxx XxxxXxxxxxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | export-csv processes.csv -NoTypeInformation
PS C:\>get-process | export-csv processes.csv -NoTypeInformation

# In processes.csv
__NounName,Name,Handles,VM,WS,PM,NPM,Path,Company,CPU,FileVersion,... Process,powershell,626,201666560,76058624,61943808,11960,C:\WINDOWS... Process,powershell,257,151920640,38322176,37052416,7836,C:\WINDOWS\...
```

Xxxx xxxxxxx xxxxxxx xxxxxxx xxxxxxxxxxxx xxx xxxxxxxxx xx xxx xxxxxxxx xx xxx Xxxxxxxxx.xxx xxxx xx xxx xxxxxxx xxxxxxxxx.
Xx xxxx xxx XxXxxxXxxxxxxxxxx xxxxxxxxx xx xxxxxxxx xxx xxxx xxxxxxxxxxx xx xxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command uses the Get-ChildItem cmdlet to do a recursive search in the D: drive for files with the .ps1 file name extension. It uses a pipeline operator to sends the results to the Where-Object cmdlet, which gets only files that were created after January 1, 2011, and then saves them in the ScriptFiles variable. 
PS C:\>$scriptFiles = Get-ChildItem D:\* -include *.ps1 -recurse | where-object {$_.creationtime -gt "01/01/2011"}

The second command uses the Select-Object cmdlet to select  the relevant properties of the script files. It saves the revised results in the ScriptFiles variable.
PS C:\>$scriptFiles = $scriptFiles | select-object -property Name, CreationTime, LastWriteTime, IsReadOnly

The third command uses a pipeline operator (|) to send the script file information in the ScriptFiles variable to the Export-CSV cmdlet. The command uses the Path parameter to specify the output file and the Append parameter to add the new script data to the end of the output file, instead of replacing the existing file contents.
PS C:\>$scriptFiles | export-csv -append -path \\Archive01\Scripts\Scripts.csv
```

Xxxxx xxxxxxxx xxx xxxxxxxxxxx xxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xx x xxxxxx xxxxxxxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command shows how to select properties of an object and export them to a CSV file. This command uses the Get-Date cmdlet to get the current date and time. It uses the Select-Object cmdlet to select the desired properties, and the Export-CSV cmdlet to export the object and its properties to the Date.csv file. The output shows the expected content in the Date.csv file.
PS C:\>get-date | select-object -property DateTime, Day, DayOfWeek, DayOfYear | export-csv -path Date.csv

#In Date.csv:"DateTime","Day","DayOfWeek","DayOfYear""Tuesday, October 05, 2010 2:45:13 PM","5","Tuesday","278"

The second command shows that when you use the Format-Table cmdlet to format your data before exporting it, the output is not useful. 
PS C:\>get-date | format-table -property DateTime, Day, DayOfWeek, DayOfYear | export-csv -path Date.csv

#In Date.csv: "ClassId2e4f51ef21dd47e99d3c952918aff9cd","pageHeaderEntry","pageFooterEntry","autosizeInfo","shapeInfo","groupingEntry""033ecb2bc07a4d43b5ef94ed5a35d280",,,,"Microsoft.PowerShell.Commands.Internal.Format.TableHeaderInfo","9e210fe47d09416682b841769c78b8a3",,,,,"27c87ef9bbda4f709f6b4002fa4af63c",,,,,"4ec4f0187cb04f4cb6973460dfe252df",,,,,"cf522b78d86c486691226b40aa69e95c",,,,,
```

Xxxx xxxxxxx xxxxxxxxxxxx xxx xx xxxx xxxxxx xxxxxxxx xxxx xxxxx xxxxxxxxx xxxx xxxxx xxx Xxxxxx$XXX xxxxxx.
Xx xxxxxxxx xxx xx xxxxxxxxx xxx xxxxx xxxx xxxxx.

Xxxxxxx x XXX xxxx xxx x xxxxx xxxxxx$ xx xxxxx xxxx xxxxxxx xx xxx xxx Xxxxxx$Xxxxx xxxxxx xx xxxxxx xxx  xxxx xx x xxxxx xx xxxxxxx xx xxx xxxxxx xx x XXX xxxx.
Xxxx$ xxx Xxxxxx$Xxxxx xxxxxx xxxxxx xxx xx xxxxxx xxxxxx xxxxxxxxxx xxxxxx.

Xxxxxxx$ xxxx xxx xxxxxx xxx xxxx xx x xxxxx xxx xxxx xxxxxx xx$ xxx xxx xxxxxxxxx x xxxxx xxxxxx$ xxx xxxx xxxxxxxx xxxx xxxxxx.
Xxx xxxxxxxxx XXX xxxx xx xxx xxxxxx.

Xxxx xxxxxxx xxxxx xxx xx xxxxxx xxxxxx xxxxxxxxxx xx xxxxx xxx Xxxxxx$Xxxxxx xxxxxx$ xxx xx xxxxx xxx Xxxxxx$XXX xxxxxxx xxx xxxx xxxxxxxxx xx x XXX xxxx xxxxxxx xxx xxxxxxxxxxx xxxxxxxxxx xx xxxxxxx xxxxxx.

## XXXXXXXXXX

### -Append
Xxxx xxx XXX xxxxxx xx xxx xxx xx xxx xxxxxxxxx xxxx.
Xxxxxxx xxxx xxxxxxxxx$ Xxxxxx$XXX xxxxxxxx xxx xxxx xxxxxxxx xxxxxxx xxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

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

### -Delimiter
Xxxxxxxxx x xxxxxxxxx xx xxxxxxxx xxx xxxxxxxx xxxxxx.
Xxx xxxxxxx xx x xxxxx $$$.
Xxxxx x xxxxxxxxx$ xxxx xx x xxxxx $$$.
Xx xxxxxxx x xxxxxxxxx $$$$ xxxxxxx xx xx xxxxxxxxx xxxxx.

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

### -Encoding
Xxxxxxxxx xxx xxxxxxxx xxx xxx xxxxxxxx XXX xxxx.
Xxxxx xxxxxx xxx Xxxxxxx$ XXX0$ XXX0$ XXXXX$ XXX00$ XxxXxxxxxXxxxxxx$ Xxxxxxx$ xxx XXX.
Xxx xxxxxxx xx XXXXX.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: Unicode, UTF7, UTF8, ASCII, UTF32, BigEndianUnicode, Default, OEM

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Xxxxxxxxxx xxx xxxx xxxxxxxxx xx xxxx xxxxxxx xxxxxxxxx.

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

### -InformationAction
Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

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
Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

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

### -InputObject
Xxxxxxxxx xxx xxxxxxx xx xxxxxx xx XXX xxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx xxx xxxxxxx xx xxxx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxx.
Xxx xxx xxxx xxxx xxxxxxx xx Xxxxxx$XXX.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -NoClobber
Xx xxx xxxxxxxxx $xxxxxxx xxx xxxxxxxx$ xx xx xxxxxxxx xxxx.
Xx xxxxxxx$ xx x xxxx xxxxxx xx xxx xxxxxxxxx xxxx$ Xxxxxx$XXX xxxxxxxxxx xxx xxxx xxxxxxx xxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: NoOverwrite

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoTypeInformation
Xxxxx xxx xxxx xxxxxxxxxxx xxxx xxx XXX xxxx.
Xx xxxxxxx$ xxx xxxxx xxxx xx xxx XXX xxxx xxxxxxxx $$XXXX $ xxxxxxxx xx xxx xxxxx$xxxxxxxxx xxxx xx xxx xxxx xx xxx xxxxxx.

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

### -Path
Xxxxxxxxx xxx xxxx xx xxx XXX xxxxxx xxxx.
Xxxx xxxxxxxxx xx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UseCulture
Xxx xxx xxxx xxxxxxxxx xxx xxx xxxxxxx xxxxxxx xx xxx xxxx xxxxxxxxx.
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

### -LiteralPath
Xxxxxxxxx xxx xxxx xx xxx XXX xxxxxx xxxx.
Xxxxxx Xxxx$ xxx xxxxx xx xxx XxxxxxxXxxx xxxxxxxxx xx xxxx xxxxxxx xx xx xx xxxxx.
Xx xxxxxxxxxx xxx xxxxxxxxxxx xx xxxxxxxxx.
Xx xxx xxxx xxxxxxxx xxxxxx xxxxxxxxxx$ xxxxxxx xx xx xxxxxx xxxxxxxxx xxxxx.
Xxxxxx xxxxxxxxx xxxxx xxxx Xxxxxxx XxxxxXxxxx xxx xx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: PSPath

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Xxxxxxx xxx xxx xxxxxxxxxxxx xxxxxx xxxxxxx xxx xxxxxx.Xxxxxxx xxx xxx xxxxxxxxxxxx xxxxxx xxxxxxx xxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Xxxxx xxxx xxxxx xxxxxx xx xxx xxxxxx xxxx.
Xxx xxxxxx xx xxx xxx.Xxxxx xxxx xxxxx xxxxxx xx xxx xxxxxx xxxx.
Xxx xxxxxx xx xxx xxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.Management.Automation.PSObject
Xxx xxx xxxx xxx xxxxxx xxxx xx Xxxxxxxx Xxxx Xxxxxx $XXX$ xxxxxxx xx Xxxxxx$XXX.

## XXXXXXX

### System.String
Xxx XXX xxxx xx xxxx xx xxx xxxx xxxxxxxxxx xx xxx Xxxx xxxxxxxxx.

## XXXXX
Xxx Xxxxxx$XXX xxxxxx xxxxxxxx xxx xxxxxxx xxxx xxx xxxxxx xxxx x xxxxxx xx XXX xxxxxxxx$xxxxxx xxxxxxx xxx xxxxx xxxx xx xxx xxxxxxxxx xxxx xxxx.
Xxx xxx xxx Xxxxxx$XXX xx xxxx xxxxxxx xx x XXX xxxx xxx xxxx xxx xxx Xxxxxx$XXX xxxxxx xx xxxxxx xxxxxxx xxxx xxx xxxx xx xxx XXX xxxx.

Xx xxx XXX xxxx$ xxxx xxxxxx xx xxxxxxxxxxx xx x xxxxx$xxxxxxxxx xxxx xx xxx xxxxxxxx xxxxxx xx xxx xxxxxx.
Xxx xxxxxxxx xxxxxx xxx xxxxxxxxx xx xxxxxxx $xx xxxxx xxx XxXxxxxx$$ xxxxxx xx xxx xxxxxx$$ xx xxxx xxx xxxxxxxxx xxxxxxxxxxx xx xxx xxxx xx xxx xxxxxxxx xxxxx.
Xxxxxx$XXX xxxx xxx xxxxxx xxx xxxxxxx xx xxx xxxxxx.

Xxx xxxxxx xx xx xxxxxxxx xxxx xx xx xxxxxxx$

$$ Xxx xxxxx xxxx xx xxx XXX xxxx xxxxxxxx xxx xxxxxx $$XXXX $ xxxxxxxx xx xxx xxxxx xxxxxxxxx xxxx xx xxx xxxxxx$ xxxx xx $XXXX Xxxxxx.Xxxxxxxxxxx.Xxxxxxx. Xx xxxxxxxx xxxx xxxx$ xxx xxx XxXxxxXxxxxxxxxxx xxxxxxxxx.
$$ Xxx xxxx xxxx xx xxx XXX xxxx xxxxxxxxxx xxx xxxxxx xxxxxxx. Xx xxxxxxxx x xxxxx$xxxxxxxxx xxxx xx xxx xxxxx xx xxx xxx xxxxxxxxxx xx xxx xxxxx xxxxxx.
$$ Xxxxxxxxxx xxxxx xx xxx xxxx xxxxxxx xx xxxxx$xxxxxxxxx xxxxx xx xxx xxxxxxxx xxxxxx xx xxxx xxxxxx.

Xxxx xxx xxxxxx xxxxxxxx xxxxxxx xx Xxxxxx$XXX$ Xxxxxx$XXX xxxxxxxxx xxx xxxx xxxxx xx xxx xxxxxxxxxx xx xxx xxxxx xxxxxx xxxx xxx xxxxxx.
Xx xxx xxxxxxxxx xxxxxxx xx xxx xxxx xxx xx xxx xxxxxxxxx xxxxxxxxxx$ xxx xxxxxxxx xxxxx xx xxxx xxxxxx xx xxxx$ xx xxxxxxxxxxx xx xxx xxxxxxxxxxx xxxxxx.
Xx xxx xxxxxxxxx xxxxxxx xxxx xxxxxxxxxx xxxxxxxxxx$ xxxxx xxxxxxxx xxxxxx xxx xxx xxxxxxxx xx xxx xxxx.

Xxx xxx xxx xxx Xxxxxx$Xxx xxxxxx xx xx$xxxxxx xxxxxxx xxxx xxx XXX xxxxxxx xx xxx xxxxx.
Xxx xxxxxxxxx xxxxxxx xxx XXX xxxxxxxx xx xxx xxxxxxxx xxxxxxx xxxx xxxxxxx xx xxxxxx xxxxxxxxxxxxxxx xx xxx xxxxxxxx xxxxxx xxx xx xxxxxxx.

Xxx XxxxxxxXx$Xxx xxx XxxxxxxXxxx$Xxx xxxxxxx xx xxxxxxx xxxxxxx xx XXX xxxxxxx $xxx xxxx$.
Xxxxxx$XXX xx xxx xxxx xx XxxxxxxXx$XXX$ xxxxxx xxxx xx xxxxx xxx XXX xxxxxxx xx x xxxx.

## XXXXXXX XXXXX

[ConvertFrom-Csv]()

[ConvertTo-Csv]()

[Format-Table]()

[Import-Csv]()

[Select-Object]()

