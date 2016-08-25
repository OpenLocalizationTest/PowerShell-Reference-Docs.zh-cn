---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293983
schema: 2.0.0
---

# Import-Csv
## XXXXXXXX
Xxxxxxx xxxxx$xxxx xxxxxx xxxxxxx xxxx xxx xxxxx xx x XXX xxxx.

## XXXXXX

### Delimiter (Default)
```
Import-Csv [[-Delimiter] <Char>] [[-Path] <String[]>] [-LiteralPath <String[]>] [-Header <String[]>]
 [-Encoding <String>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### UseCulture
```
Import-Csv [[-Path] <String[]>] [-LiteralPath <String[]>] [-UseCulture] [-Header <String[]>]
 [-Encoding <String>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$Xxx xxxxxx xxxxxxx xxxxx$xxxx xxxxxx xxxxxxx xxxx xxx xxxxx xx XXX xxxxx.
Xxxx xxxxxx xx xxx XXX xxxx xxxxxxx x xxxxxxxx xx xxx xxxxxx xxxxxx xxx  xxx xxxxx xx xxxx xxxxxx xxx xxxxxxxx xxxxxx.
Xxxxxx$Xxx xxxxx xx xxx XXX xxxx$ xxxxxxxxx xxxxx xxxx xxx xxxxxxxxx xx xxx Xxxxxx$Xxx xxxxxx.

Xxx xxx xxx xxx xxxxxxxxxx xx xxx Xxxxxx$Xxx xxxxxx xx xxxxxxx xxx xxxxxx xxxxxx xxx xxx xxx xxxx xxxxxxxxx$ xx xxxxxx Xxxxxx$Xxx xx xxx xxx xxxx xxxxxxxxx xxx xxx xxxxxxx xxxxxxx xx xxx xxxx xxxxxxxxx.

Xxx xxx xxxx xxx xxx XxxxxxxXx$Xxx xxx XxxxxxxXxxx$Xxx xxxxxxx xx xxxxxxx xxxxxxx xx XXX xxxxxxx $xxx xxxx$.
Xxxxx xxxxxxx xxx xxx xxxx xx xxx Xxxxxx$XXX xxx Xxxxxx$Xxx xxxxxxx$ xxxxxx xxxx xxxx xx xxx xxxx xxxx xxxxx.

Xxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ xx x xxxxxx xxx xxxxx xx x XXX xxxx xxxxxxxx xx xxxxx xx xxxx xxxxx$ Xxxxxxx XxxxxXxxxx xxxxxxx x xxxxxxx xxxxxx xxx xxxx xxx xxxxxxxx x xxxxxxx xxxxxxx.
Xx xxxxxxxx xxxxxxxx xx Xxxxxxx XxxxxXxxxx$ xx x xxxxxx xxx xxxxx xx x XXX xxxx xxxxxxxx xx xxxxx xx xxxx xxxxx$ xxx Xxxxxx$Xxx xxxxxxx xxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
This example shows how to export and then import a CSV file of objects.The first command uses the Get-Process cmdlet to get the process on the local computer. It uses a pipeline operator (|) to send the process objects to the Export-CSV cmdlet, which exports the process objects to the Processes.csv file in the current directory.
PS C:\>get-process | export-csv processes.csv

The second command uses the Import-Csv cmdlet to import the processes in the Import-Csv file. Then it saves the resulting process objects in the $p variable.
PS C:\>$p = Import-Csv processes.csv

The third command uses a pipeline operator to pipe the imported objects to the Get-Member cmdlets. The result shows that they are CSV:System.Diagnostic.Process objects, not the System.Diagnostic.Process objects that Get-Process returns.Also, because there is no entry type in the formatting files for the CSV version of the process objects, these objects are not formatted in the same way that standard process objects are formatted.To display the objects, use the formatting cmdlets, such as Format-Table and Format-List, or pipe the objects to Out-GridView.
PS C:\>$p | get-member
TypeName: CSV:System.Diagnostics.Process
Name                       MemberType   Definition
----                       ----------   ----------
Equals                     Method       System.Boolean Equals(Object obj)
GetHashCode                Method       System.Int32 GetHashCode()
GetType                    Method       System.Type GetType()
ToString                   Method       System.String ToString()
BasePriority               NoteProperty System.String BasePriority=8
Company                    NoteProperty System.String Company=Microsoft Corporation
...
PS C:\>$p | out-gridview
```

Xxxx xxxxxxx xxxxx xxx xx xxxxxx xxx xxxx xxxxxx x XXX xxxx xx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>get-process | export-csv processes.csv -Delimiter :
PS C:\>$p = Import-Csv processes.csv -Delimiter :
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx Xxxxxxxxx xxxxxxxxx xx xxx Xxxxxx$Xxx xxxxxx.
Xx xxxx xxxxxxx$ xxx xxxxxxxxx xxx xxxxxxxx xx x xxxx xxxx xxxx x xxxxx $$$ xx x xxxxxxxxx.

Xxxx xxxxxxxxx$ xxx Xxxxxx$Xxx xxxx xxxx xxx Xxxxxxxxx xxxxxxxxx xx xxxxxxxx xxx xxxxxxxxx xxxx xx xxxx xx xxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$p = Import-Csv processes.csv -UseCulture
PS C:\>(get-culture).textinfo.listseparator
,
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx XxxXxxxxxx xxxxxxxxx xx xxx Xxxxxx$Xxx xxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx xxx xxxxxxx xx xxx Xxxxxxxxx.xxx xxxx xxxx xxx $x xxxxxxxx.
Xx xxxx xxx XxxXxxxxxx xxxxxxxxx xx xxxxxx Xxxxxx$Xxx xx xxx xxx xxxx xxxxxxxxx xxxxxxx xxx xxx xxxxxxx xxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxxx xxx xxxx xxxxxxxxx xxx xxx xxxxxxx xxxxxxx.
Xx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxx xxxxxxx.
Xx xxxx xxx xxx $.$ xxxxxx xx xxx xxx XxxxXxxx xxxxxxxx xx xxx xxxxxxx xxxxxxx xxx xxx XxxxXxxxxxxxx xxxxxxxx xx xxx xxxxxx xx XxxxXxxx.
Xx xxxx xxxxxxx$ xxx xxxxxxx xxxxxxx x xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command uses the Start-Job cmdlet to start a background job that runs a Get-Process command on the local computer. A pipeline operator (|) sends the resulting job object to the Export-CSV cmdlet, which converts the job object to CSV format. An assignment operator (=) saves the resulting CSV in the Jobs.csv file.
PS C:\>start-job -scriptblock { get-process } | export-csv jobs.csv

The second command saves a header in the $header variable. Unlike the default header, this header uses "MoreData" instead of "HasMoreData" and "State" instead of "JobStateInfo".
PS C:\>$header = "MoreData","StatusMessage","Location","Command","State","Finished","InstanceId","SessionId","Name","ChildJobs","Output","Error","Progress","Verbose","Debug","Warning","StateChanged"

The next three commands delete the original header (the second line) from the Jobs.csv file.
PS C:\># Delete header from file

PS C:\>$a = (get-content jobs.csv)
PS C:\>$a = $a[0], $a[2..($a.count - 1)]
PS C:\>$a > jobs.csv

The sixth command uses the Import-Csv cmdlet to import the Jobs.csv file and convert the CSV strings into a CSV version of the job object. The command uses the Header parameter to submit the alternate header. The results are stored in the $j variable.
PS C:\>$j = Import-Csv jobs.csv -header $header

The seventh command displays the object in the $j variable. The resulting object has "MoreData" and "State" properties, as shown in the command output.
PS C:\>$j

MoreData      : True
StatusMessage :
Location      : localhost
Command       : get-process
State         : Running
Finished      : System.Threading.ManualResetEvent
InstanceId    : 135bdd25-40d6-4a20-bd68-05282a59abd6
SessionId     : 1
Name          : Job1
ChildJobs     : System.Collections.Generic.List`1[System.Management.Automation.Job]
Output        : System.Management.Automation.PSDataCollection`1[System.Management.Automation.PSObject]
Error         : System.Management.Automation.PSDataCollection`1[System.Management.Automation.ErrorRecord]
Progress      : System.Management.Automation.PSDataCollection`1[System.Management.Automation.ProgressRecord]
Verbose       : System.Management.Automation.PSDataCollection`1[System.String]
Debug         : System.Management.Automation.PSDataCollection`1[System.String]
Warning       : System.Management.Automation.PSDataCollection`1[System.String]
StateChanged  :
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx Xxxxxx xxxxxxxxx xx Xxxxxx$Xxx xx xxxxxx xxx xxxxx xx xxxxxxxxxx xx xxx xxxxxxxxx xxxxxxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command uses the Get-Content cmdlet to get the Links.csv file.
PS C:\>Get-Content .\Links.csv
113207,about_Aliases113208,about_Arithmetic_Operators113209,about_Arrays113210,about_Assignment_Operators113212, 
about_Automatic_Variables113213,about_Break113214,about_Command_Precedence113215,about_Command_Syntax144309, 
about_Comment_Based_Help113216,about_CommonParameters113217,about_Comparison_Operators113218,about_Continue113219, 
about_Core_Commands113220,about_Data_Section…

The second command uses the Import-Csv cmdlet to import the Links.csv file. The command uses the Header parameter to specify LinkId and TopicTitle as property names for the new custom objects. The command saves the imported objects in the $a variable.
PS C:\>$a = Import-Csv -Path .\Links.csv -Header LinkID, TopicTitle

The third command uses the Get-Member cmdlet to get the type and members of the custom objects in the $a variable.The output shows that Import-Csv returns a collection of custom objects (PSCustomObject). In addition to some default properties, the custom objects have LinkID and TopicTitle note properties.
PS C:\>$a | Get-Member
   TypeName: System.Management.Automation.PSCustomObject
Name                      MemberType   Definition
----                      ----------   ----------
Equals                    Method       bool 
Equals(System.Object obj) 
GetHashCode Method       int 
GetHashCode()GetType     Method       type 
GetType()ToString    Method       string 
ToString()LinkID      NoteProperty System.String 
LinkID=113207TopicTitle  NoteProperty System.String 
TopicTitle=about_Aliases

This command shows that you can use the custom object like you would any object in Windows PowerShell.The command pipes the custom objects in the $a variable to the Where-Object cmdlet, which gets only objects with a TopicTitle property that includes "alias".The Where-Object command uses the new simplified command format that does not require symbols, script blocks, or curly braces.
PS C:\>$a | Where-Object TopicTitle -like "*alias*"
LinkID            TopicTitle
------            ----------
113207            about_Aliases
113432            Alias Provider
113296            Export-Alias
113306            Get-Alias
113339            Import-Alias
113352            New-Alias
113390            Set-Alias
```

Xxxx xxxxxxx xxxxx xxx xx xxxxxx x xxxxxx xxxxxx xx Xxxxxxx XxxxxXxxxx xx xxxxx x XXX xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
The first command uses the Get-Content cmdlet to get the Projects.csv file on the Server02 remote computer. The output shows that the header row of the file is missing a value between "ProjectName" and "Completed."
PS C:\>Get-Content "\\Server2\c$\Test\Projects.csv"
ProjectID, ProjectName,,Completed13, Inventory, Redmond, True440, , FarEast, True469, Marketing, Europe, False

The second command uses the Import-Csv cmdlet to import the Projects.csv file.The output shows that Import-Csv generates a warning and substitutes a default name, H1, for the missing header row value. H1 is also used for the name of the object property.
PS C:\>Import-Csv "\\Server2\c$\Test\Projects.csv"
PS C:\>WARNING: One or more headers were not specified. Default names starting with "H" have been used in place of any missing headers. 
ProjectID     ProjectName       H1               Completed
---------     -----------       --               ---------
13            Inventory         Redmond          True
440                             FarEast          True
469           Marketing         Europe           False

The third command uses the dot method to get the value of the H1 property of the object that Import-Csv creates.
PS C:\>(Import-Csv "\\Server2\c$\Test\Projects.csv").H1
RedmondFarEastEurope
```

Xxxx xxxxxxx xxxxx xxx xxx Xxxxxx$Xxx xxxxxx xx Xxxxxxx XxxxxXxxxx 0.0 xxxxxxxx xxxx xxx xxxxxx xxx xx x XXX xxxx xxxxxxxx x xxxx xx xxxxx xxxxx.
Xxxxxx$Xxx xxxxxxxxxxx x xxxxxxx xxxx xxx xxx xxxxxx xxx.
Xxx xxxxxxx xxxx xxxxxxx xxx xxxx xx xxx xxxxxxxx xx xxx xxxxxx xxxx Xxxxxx$Xxx xxxxxxx.

## XXXXXXXXXX

### -Delimiter
Xxxxxxxxx xxx xxxxxxxxx xxxx xxxxxxxxx xxx xxxxxxxx xxxxxx xx xxx XXX xxxx.
Xxx xxxxxxx xx x xxxxx $$$.
Xxxxx x xxxxxxxxx$ xxxx xx x xxxxx $$$.
Xx xxxxxxx x xxxxxxxxx $$$$ xxxxxxx xx xx xxxxxxxxx xxxxx.

Xx xxx xxxxxxx x xxxxxxxxx xxxxx xxxx xxx xxxxxx xxxxxx xxxxxxxxx xx xxx xxxx$ Xxxxxx$Xxx xxxxxx xxxxxx xxxxxxx xxxx xxx XXX xxxxxxx.
Xxxxxxx$ xx xxxxxxx xxx xxxxxxx.

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
Xxxxxxxxx xxx xxxx xx xxxxxxxxx xxxxxxxx xxxx xxx xxxx xx xxx XXX xxxx.
Xxxxx xxxxxx xxx Xxxxxxx$ XXX0$ XXX0$ XXXXX$ XXX00$ XxxXxxxxxXxxxxxx$ Xxxxxxx$ xxx XXX.
Xxx xxxxxxx xx XXXXX.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

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

### -Header
Xxxxxxxxx xx xxxxxxxxx xxxxxx xxxxxx xxx xxx xxx xxxxxxxx xxxx.
Xxx xxxxxx xxxxxx xxxxxxxxxx xxx xxxxx xx xxx xxxxxxxxxx xx xxx xxxxxx xxxx Xxxxxx$Xxx xxxxxxx.

Xxxxx x xxxxx$xxxxxxxxx xxxx xx xxx xxxxxx xxxxxxx.
Xxxxxxx xxxx xxxx xx xxxxxxxxx xxxxx $xxxxxx xx xxxxxx$.
Xx xxx xxxxxxx xxx xxxxxx xxxxxx xx xxxxxxxxx xxxxx.
Xx xxx xxxxx xxxxx xxxxxx xxxxxxx xxxx xxxxx xxx xxxxxxx$ xxx xxxxxxxxx xxxxxxx xxxx xxxx xx xxxxxx.
Xx xxx xxxxx xxxx xxxxxxx xxxx xxxxx xxx xxxxxxx$ xxx xxxxx xxxxxxx xxx xxxxxxx.

Xxxx xxxxx xxx Xxxxxx xxxxxxxxx$ xxxxxx xxx xxxxxxxx xxxxxx xxx xxxx xxx XXX xxxx.
Xxxxxxxxx$ Xxxxxx$Xxx xxxxxxx xx xxxxx xxxxxx xxxx xxx xxxxx xx xxx xxxxxx xxx.

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

### -InformationAction
Xx xxx xxxxxxx x xxxxxxxxx xxxxx xxxx xxx xxxxxx xxxxxx xxxxxxxxx xx xxx xxxx$ Xxxxxx$Xxx xxxxxx xxxxxx xxxxxxx xxxx xxx XXX xxxxxxx.
Xxxxxxx$ xx xxxxxxx xxx xxxxxxx.

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
Xx xxx xxxxxxx x xxxxxxxxx xxxxx xxxx xxx xxxxxx xxxxxx xxxxxxxxx xx xxx xxxx$ Xxxxxx$Xxx xxxxxx xxxxxx xxxxxxx xxxx xxx XXX xxxxxxx.
Xxxxxxx$ xx xxxxxxx xxx xxxxxxx.

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

### -Path
Xxxxxxxxx xxx xxxx xx xxx XXX xxxx xx xxxxxx.
Xxx xxx xxxx xxxx x xxxx xx Xxxxxx$Xxx.

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

### -UseCulture
Xxx xxx xxxx xxxxxxxxx xxx xxx xxxxxxx xxxxxxx xx xxx xxxx xxxxxxxxx.
Xxx xxxxxxx xx x xxxxx $$$.

Xx xxxx xxx xxxx xxxxxxxxx xxx x xxxxxxx$ xxx xxx xxxxxxxxx xxxxxxx$ $Xxx$Xxxxxxx$.XxxxXxxx.XxxxXxxxxxxxx.
Xx xxx xxxxxxx x xxxxxxxxx xxxxx xxxx xxx xxxxxxxxx xxxx xx xxx XXX xxxxxxx$ XxxxxxxXxxx$XXX xxxxxx xxxxxx xxxxxxx xxxx xxx XXX xxxxxxx.
Xxxxxxx$ xx xxxxxxx xxx xxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UseCulture
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LiteralPath
Xxxxxxxxx xxx xxxx xx xxx XXX xxxx xx xxxxxx.
Xxxxxx Xxxx$ xxx xxxxx xx xxx XxxxxxxXxxx xxxxxxxxx xx xxxx xxxxxxx xx xx xx xxxxx.
Xx xxxxxxxxxx xxx xxxxxxxxxxx xx xxxxxxxxx.
Xx xxx xxxx xxxxxxxx xxxxxx xxxxxxxxxx$ xxxxxxx xx xx xxxxxx xxxxxxxxx xxxxx.
Xxxxxx xxxxxxxxx xxxxx xxxx Xxxxxxx XxxxxXxxxx xxx xx xxxxxxxxx xxx xxxxxxxxxx xx xxxxxx xxxxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: PSPath

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

### System.String
Xxx xxx xxxx x xxxxxx xxxx xxxxxxxx x xxxx xx Xxxxxx$Xxx.

## XXXXXXX

### Object.
Xxxxxx$Xxx xxxxxxx xxx xxxxxxx xxxxxxxxx xx xxx xxxxxxx xx xxx XXX xxxx.

## XXXXX
Xxxxxxx xxx xxxxxxxx xxxxxxx xxx XXX xxxxxxxx xx xxx xxxxxx xxxx$ xxxx xxx xxx xxxxxxxxxx xxx xxxxxxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxx xxxxxxxxxx xxxxxxx xxxx xxxxxx xxx xxx$XXX xxxxxxxx xx xxx xxxxxx xxxx.

Xxx xxxxxx xx xx Xxxxxx$Xxx xxxxxxx xx x xxxxxxxxxx xx xxxxxxx xxxx xxxx x xxxxx$xxxx xxxxxx xxxxxx.
Xxxx xxx xx x xxxxxxxx xxxxxx$ xx xxx xxx xxx xxx Xxxxx xxxxxxxx xx xxx xxxxxx xx xxxxx xxx xxxxx xxxx.
Xxx xxxxxxx xxx xxx xxxxxxxxxx xx xxx xxxxxx xxx xxxxx xx xxx xxxx xxx xxx xxxxxxxx xxxxxx.

Xxx xxxxxx xxxxxx xxx xxxxxxxxxx xxx xxxxxx xx xxxxxxx xxx xxx xxxxxx xxxxx.
Xxx xxxxxx xxxxx xxx xxxx xxx xxxxx xx xxx xxxxxxxxxx xx xxx xxxxxxx.
Xxx xxxxx xxx xx xxxxxxxxxxx xx xx xxx xxxxxx xxxxxxx$ xxxxxx xxx xxx xxx Xxxxxx xxxxxxxxx xx xxxxxxx xxxxxx xxxxxxx.
Xx xxx xxx xxx xxxx xxxxxx xxxx xxx xxxxxx xxx$ xxx xxxxxxxxxx xxxxxx xxx xxxxxxx.

Xx xxx xxxxxx xxxxxx xxx xx xxxxxxx x xxxxx xx xxxxxxxx x xxxx xx xxxxx xxxxx$ Xxxxxx$Xxx xxxx $X$ xxxxxxxx xx x xxxxxx xxx xxx xxxxxxx xxxxxx xxxxxx xxx xxxxxxxx xxxx.

Xx xxx XXX xxxx$ xxxx xxxxxx xx xxxxxxxxxxx xx x xxxxx$xxxxxxxxx xxxx xx xxx xxxxxxxx xxxxxx xx xxx xxxxxx.
Xxx xxxxxxxx xxxxxx xxx xxxxxxxxx xx xxxxxxx $xx xxxxx xxx XxXxxxxx$$ xxxxxx xx xxx xxxxxx$$ xx xxxx xxx xxxxxxxxx xxxxxxxxxxx xx xxx xxxx xx xxx xxxxxxxx xxxxx.
Xxxxxx$XXX xxxx xxx xxxxxx xxx xxxxxxx xx xxx xxxxxx.

## XXXXXXX XXXXX

[ConvertFrom-Csv]()

[ConvertTo-Csv]()

[Export-Csv]()

