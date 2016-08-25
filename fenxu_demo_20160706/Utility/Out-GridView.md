---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293997
schema: 2.0.0
---

# Out-GridView
## XXXXXXXX
Xxxxx xxxxxx xx xx xxxxxxxxxxx xxxxx xx x xxxxxxxx xxxxxx.

## XXXXXX

### PassThru (Default)
```
Out-GridView [-InputObject <PSObject>] [-Title <String>] [-PassThru] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### Wait
```
Out-GridView [-InputObject <PSObject>] [-Title <String>] [-Wait] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### OutputMode
```
Out-GridView [-InputObject <PSObject>] [-Title <String>] [-OutputMode <OutputModeOption>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxx$XxxxXxxx xxxxxx xxxxx xxx xxxxxx xxxx x xxxxxxx xx x xxxx xxxx xxxxxx xxxxx xxx xxxxxx xx xxxxxxxxx xx xx xxxxxxxxxxx xxxxx.

Xxxxxxx xxxx xxxxxx xxxxxxxx x xxxx xxxxxxxxx$ xx xxxx xxx xxxx xx Xxxxxx Xxxx xxxxxxxxxxxxx xx Xxxxxxx Xxxxxx.

Xxx xxx xxx xxx xxxxxxxxx xxxxxxxx xx xxx xxxxx xx xxxxxxx xxxx xxxx$

$$ Xxxx$ Xxxx$ xxx Xxxxxxx Xxxxxxx$ Xx xxxx$ xxxx$ xx xxxxxxx x xxxxxx$ xxxxx$xxxxx x xxxxxx xxxxxx xxx xxxx xxxxx $Xxxxxx Xxxxxxx.$
$$ Xxxx. Xx xxxx xxx xxxx$ xxxxx x xxxxxx xxxxxx. Xxxxx xxxxx xx xxxxxx xxxx xxxxxxxxx xx xxxxxxxxxx xxxxx.
$$ Xxxxx Xxxxxx. Xxx xxx $Xxxxxx$ xxx xx xxx xxx xx xxx xxxxxx xx xxxxxx xxx xxxx xx xxx xxxxx. Xxx xxx xxxxxx xxx xxxx xx x xxxxxxxxxx xxxxxx$ xxxxxx xxx xxxxxxxx$ xxx xxxxxx xxx xxxxxxxx xxxxx.
$$ Xxxxxxxx Xxxxxx. Xxx xxx $Xxx xxxxxxxx$ xxxx$xxxx xxxx xx xxxxxx xxxxx xx xxxxxx xxx xxxx. Xxxx xx xxxx xxxxxx xxx xxxx xxxxx xxxx xxxx$ xxxx xx xxxxx xxxx.
$$ Xxxx xxx xxxxx. Xx xxxx xxxx xx xxxx xxxx Xxx$XxxxXxxx$ xxxxx XXXX$X $xxxx$. Xxx xxx xxxxx xxx xxxx xxxx xxx xxxx xx xxxxxxxxxxx xxxxxxx.

Xxx xxxxxxxxxxxx xxx xxxxx xxxxx xxxxxxxx$ xxxx $Xxx$Xxxx Xxx$XxxxXxxx $Xxxx$ xxx xxx $Xxx xx Xxx xxx Xxxx Xxxx Xxxxxx Xxxxxxxx$ xx xxx XXXXX xxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Process | Out-GridView
```

Xxxx xxxxxxx xxxx xxx xxxxxxxxx xxxxxxx xx xxx xxxxx xxxxxxxx xxx xxxxx xxxx xx x xxxx xxxx xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$p = Get-Process
PS C:\>$p | Out-GridView
```

Xxxx xxxxxxx xxxx xxxx xxx xxxxxxxxx xxxxxxx xx xxx xxxxx xxxxxxxx xxx xxxxx xxxx xx x xxxx xxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxxxx xx xxx xxxxxxxx xxx xxxx xxxxx xxx xxxxxxx xxxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx xx xxxx xxx $x xxxxxxxx xx Xxx$XxxxXxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Process | Select-Object -Property Name, WorkingSet, PeakWorkingSet | Sort-Object -Property WorkingSet -Descending | Out-GridView
```

Xxxx xxxxxxx xxxxxxxx x xxxxxxxxx xxxxx xx x xxxx xxxx xxxxxx.

Xx xxxx xxx Xxx$Xxxxxxx xxxxxx xx xxx xxx xxxxxxxxx xx xxx xxxxxxxx.

Xxxx$ xx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxx xxxxxxx xx xxx Xxxxxx$Xxxxxx xxxxxx.
Xxx xxxxxxx xxxx xxx Xxxxxxxx xxxxxxxxx xx Xxxxxx$Xxxxxx xx xxxxxx xxx Xxxx$ XxxxxxxXxx$ xxx XxxxXxxxxxxXxx xxxxxxxxxx xx xx xxxxxxxxx xx xxx xxxxx.

Xxxxxxx xxxxxxxx xxxxxxxx xxxxx xxx xxxxxxxx xxxxxxx xx xxx Xxxx$Xxxxxx xxxxxx$ xxxxx xxxxx xxxx xx xxxxxxxxxx xxxxx xx xxx xxxxx xx xxx XxxxxxxXxx xxxxxxxx.

Xxx xxxxx xxxx xx xxx xxxxxxx xxxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxxxxx xxxxx xx Xxx$XxxxXxxx.

Xxx xxx xxx xxx xxx xxxxxxxx xx xxx xxxx xxxx xx xxxxxx$ xxxx$ xxx xxxxxx xxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>($a = Get-ChildItem -Path $pshome -Recurse) | Out-GridView
```

Xxxx xxxxxxx xxxxx xxx xxxxxx xx x xxxxxxxx xxx xxxxx xx xx Xxx$XxxxXxxx.

Xxx xxxxxxx xxxx xxx Xxx$XxxxxXxxx xxxxxx xx xxx xxx xxxxx xx xxx Xxxxxxx XxxxxXxxxx xxxxxxxxxxxx xxxxxxxxx xxx xxx xxxxxxxxxxxxxx.
Xxx xxxx xx xxx xxxxxxxxxxxx xxxxxxxxx xx xxxxx xx xxx $xxxxxx xxxxxxxxx xxxxxxxx.

Xxx xxxxxxx xxxx xxx xxxxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xx xxx $x xxxxxxxx xxx xxx xxxxxxxx xxxxxxxx $$$ xx xxxx xxx xxxxxx xx Xxx$XxxxXxxx.

Xxx xxxxxxxxxxx xx xxx xxxxxxx xxxxxxxxx xxx xxxxx xx xxxxxxxxxx.
Xx x xxxxxx$ xxx xxxxxx xxxx xxx Xxx$XxxxxXxxx xxxxxxx xx xxxxx xx xxx $x xxxxxxxx xxxxxx xx xx xxxx xx Xxx$XxxxXxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Process -ComputerName Server01| ogv -Title "Processes - Server01"
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxxxxx xxxx xxx xxxxxxx xx xxx Xxxxxx00 xxxxxxxx xx x xxxx xxxx xxxxxx.

Xxx xxxxxxx xxxx $xxx$$ xxxxx xx xxx xxxxx$xx xxxxx xxx xxx Xxx$XxxxXxxx xxxxxx$ xx xxxx xxx Xxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxx xxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Invoke-Command -ComputerName S1, S2, S3 -ScriptBlock {Get-Culture} | Out-GridView
```

Xxxx xxxxxxx xxxxx xxx xxxxxxx xxxxxx xxx xxxxxxx xxxx xxxxxxxxx xxxx xxxxxx xxxxxxxxx xx xxx Xxx$XxxxXxxx xxxxxx.

Xxx xxxxxxx xxxx xxx Xxxxxx$Xxxxxxx xxxxxx xx xxx x Xxx$Xxxxxxx xxxxxxx xx xxxxx xxxxxx xxxxxxxxx.
Xx xxxx x xxxxxxxx xxxxxxxx xx xxxx xxx xxxx xxxx xx xxxxxxxx xx xxx Xxx$XxxxXxxx xxxxxx.

Xxxxxx xxxx xxx xxxxxx xxxxx xxxx xxxxxxxx xxx xxxxxxxx xxxx xxx xxx xxxxxxxx xxxx xxx xxxxxxx xxx Xxx$XxxxXxxx xxxxxxx.
Xx xx xxx$ xxx xxxxxxx xxxxx xxxx xxxx xx xxxxx xx xxxx x xxxx xxxx xxxxxx xx xxxx xx xxx xxxxxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-Process | Out-GridView -PassThru | Export-Csv -Path .\ProcessLog.csv
```

Xxxx xxxxxxx xxxx xxx xxxxxx xxxxxxxx xxxxxxxxx xxxx xxx Xxx$XxxxXxxx xxxxxx.
Xxx xxxxxxxxx xxxx xxx xxxxxx xxx xxxxxx xx xxx Xxxxxx$Xxx xxxxxxx xxx xxxxxxx xx xxx XxxxxxxXxx.xxx xxxx.

Xxx xxxxxxx xxxx xxx XxxxXxxx xxxxxxxxx xx Xxx$XxxxXxxx$ xxxxx xxxx xxx xxxx xxxxxxxx xxxxx xxxx xxx xxxxxxxx.
Xxx XxxxXxxx xxxxxxxxx xx xxxxxxxxxx xx xxxxx xxx Xxxxxxxx xxxxx xx xxx XxxxxxXxxx xxxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Powershell.exe -Command "Get-Service | Out-GridView -Wait"
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx Xxxx xxxxxxxxx xx Xxx$XxxxXxxx xx xxxxxx x Xxxxxxx xxxxxxxx xx xxx Xxx$XxxxXxxx xxxxxx.
Xxxxxxx xxx Xxxx xxxxxxxxx$ Xxxxxxx XxxxxXxxxx xxxxx xxxx xx xxxx xx xxx Xxx$XxxxXxxx xxxxxx xxxxxx$ xxxxx xxxxx xxxxx xxx Xxx$XxxxXxxx xxxxxx xxxxxx xxxxxxxxxxx.

## XXXXXXXXXX

### -InformationAction
Xxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxx x xxxxxxxxxx $xxxx xxxx xxx$ xx xxxxxxx xx Xxx$XxxxXxxx$ Xxx$XxxxXxxx xxxxxx xxx xxxxxxxxxx xx xxx xxxxxxxxxx xxxxxx$ xxx xx xxxxxxxx xxx xxx xxxx xxxxxxxxxx xxx xxxxxxxxxx. Xx xxxxxxx xxx xxxx xxxxxx xx xxx xxxxxxxxxx$ xxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxxxxxx xx Xxx$XxxxXxxx.

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
Xxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxx x xxxxxxxxxx $xxxx xxxx xxx$ xx xxxxxxx xx Xxx$XxxxXxxx$ Xxx$XxxxXxxx xxxxxx xxx xxxxxxxxxx xx xxx xxxxxxxxxx xxxxxx$ xxx xx xxxxxxxx xxx xxx xxxx xxxxxxxxxx xxx xxxxxxxxxx. Xx xxxxxxx xxx xxxx xxxxxx xx xxx xxxxxxxxxx$ xxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxxxxxx xx Xxx$XxxxXxxx.

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
Xxxxxxx xxxxx xxx Xxx$XxxxXxxx.

Xxxx xxx xxx xxx XxxxxXxxxxx xxxxxxxxx xx xxxx x xxxxxxxxxx $xxxx xxxx xxx$ xx xxxxxxx xx Xxx$XxxxXxxx$ Xxx$XxxxXxxx xxxxxx xxx xxxxxxxxxx xx xxx xxxxxxxxxx xxxxxx$ xxx xx xxxxxxxx xxx xxx xxxx xxxxxxxxxx xxx xxxxxxxxxx. Xx xxxxxxx xxx xxxx xxxxxx xx xxx xxxxxxxxxx$ xxx x xxxxxxxx xxxxxxxx $$$ xx xxxx xxxxxxx xx Xxx$XxxxXxxx.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Title
Xxxxxxxxx xxx xxxx xxxx xxxxxxx xx xxx xxxxx xxx xx xxx Xxx$XxxxXxxx xxxxxx.

Xx xxxxxxx$ xxx xxxxx xxx xxxxxxxx xxx xxxxxxx xxxx xxxxxxx Xxx$XxxxXxxx.

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

### -OutputMode
Xxxx xxxxx xxxx xxx xxxxxxxxxxx xxxxxx xxxx xxx xxxxxxxx xx xxxxx xx xxxxx xxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.
Xx xxxx xxxxx xxxx xxx xxxxxxxxxxx xxxxxx xxxx xxx xxxxxxxx$ xxxxx xx xxxxxx xxx xxxxx xxx xxxx xxxxx XX.

Xxx xxxxxx xx xxxx xxxxxxxxx xxxxxxxxx xxx xxxx xxxxx xxx xxx xxxx xxxx xxx xxxxxxxx.

$$ Xxxx$  Xx xxxxx. Xxxx xx xxx xxxxxxx xxxxx.
$$ Xxxxxx$  Xxxx xxxxx xx xxx xxxx. Xxx xxxx xxxxx xxxx xxx xxxx xxxxxxx xxx xxxx xxxx xxx xxxxx xxxxxx.
$$ Xxxxxxxx$  Xxxx$ xxx$ xx xxxx xxxxx.  Xxx xxxx xxxxx xxxx xxx xxxx xxxxxxx xxx xxxx xxxxxxxx xxxxx xxxxxxx. Xxxx xxxxx xx xxxxxxxxxx xx xxx Xxxxxxxx xxxxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: OutputModeOption
Parameter Sets: OutputMode
Aliases: 
Accepted values: None, Single, Multiple

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Xxxxx xxxxx xxxx xxx xxxxxxxxxxx xxxxxx xxxx xxx xxxxxxxx xx xxxxx xx xxxxx xxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxxxx xx xxxxx xxx Xxxxxxxx xxxxx xx xxx XxxxxxXxxx xxxxxxxxx.

Xx xxxx xxxxx xxxx xxx xxxxxxxxxxx xxxxxx xxxx xxx xxxxxxxx$ xxxxx xx xxxxxx xxx xxxxx xxx xxxx xxxxx XX.
Xxxxx$xxxxx xxx Xxxx$xxxxx xxx xxxxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: SwitchParameter
Parameter Sets: PassThru
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Wait
Xxxxxxxxxx xxx xxxxxxx xxxxxx xxx xxxxxxxx Xxxxxxx XxxxxXxxxx xxxx xxxxxxx xxxxx xxx  Xxx$XxxxXxxx xxxxxx xx xxxxxx.
Xx xxxxxxx$ xxx xxxxxxx xxxxxx xxxxxxx xxxx xxx Xxx$XxxxXxxx xxxxxx xxxxx.

Xxxx xxxxxxx xxxx xxx xxx xxx Xxx$XxxxXxxx xxxxxxx xx Xxxxxxx xxxxxxxxx.
Xxxx Xxx$XxxxXxxx xx xxxx xx x xxxxxxxx xxxxxxx xxx Xxxx xxxxxxxxx$ xxx Xxx$XxxxXxxx xxxxxx xxxxxxx xxxx xxxxxxxxxxx xxxxxx Xxxxxxx XxxxxXxxxx xxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

```yaml
Type: SwitchParameter
Parameter Sets: Wait
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.Management.Automation.PSObject
Xxx xxx xxxx xxx xxxxxx xx Xxx$XxxxXxxx.

## XXXXXXX

### None
Xxx$XxxxXxxx xxxx xxx xxxxxx xxx xxxxxxx.

## XXXXX
Xx Xxxxxxx XxxxxXxxxx 0.0$ xxx Xxx$XxxxXxxx xxxxxx xx xxxxxxxxx xx xxxxxxx xx xxxxxx xxxxxxxx xx Xxxxxxx$ xxx xx xx xxxxxxxx xxxxxxx xx Xxxxxx xxxxxxxx xx Xxxxxxx.
Xx Xxxxxxx XxxxxXxxxx 0.0$ xx xx xxxxxxxxx xx xxx xxxxxxx xx xxxxxxx.
Xxxxxxx$ xx xxx xxxx xxx xx xxxxxx xxx Xxxxxxx XxxxxXxxxx XXX xxxxxxx$ xxx Xxx$XxxxXxxx xxxxxx xx xxxx xxxxxx xxx xx xxxxxxx.

Xxx xxxxxx xxx x xxxxxx xxxxxxx xx xxxx x xxxx xxxx xxxxxx xx xxxxxxx xxxxxxxx.

Xxx xxxxxxx xxxxxx xxxx xxx xxxx xx Xxx$XxxxXxxx xxxxxx xx xxxxxxxxx$ xxxx xx xx xxxxx xxx Xxxxxx$Xxxxx xx Xxxxxx$Xxxx xxxxxxx.
Xx xxxxxx xxxxxxxxxx$ xxx xxx Xxxxxx$Xxxxxx xxxxxx.

Xxxxxxxxxxxx xxxxxx xxxx xxxxxx xxxxxxxx xxxxx xxx xx xxxxxxxxx xxxxxxxxx xx xxx xxxx xxxx xxxxxx.

XXXXXXXX XXXXXXXXX XXX XXX$XXXXXXXX

-----------------------------------

Xx xxxxx xxx xxxxxxxxx xxxxxxxx xxxxxxxxx$ xxx xxx xxxxxxx xxxx xxxxx xxxxxxx.

Xxx xxxx xxx$     Xx xxxxxxx xxxx xxxxxx$

-------------     ----------------------------------------------------------------

XXX               Xxxxx xxx xxxxxx xxxx xxx Xxxxxx xxx xx xxx Xxx xxxxxxxx xxxx xx xxx xxxxx xxx xxxx.

XX XXXXX          Xxxx xx xxx xxx.
Xxxx xxxx xx xxxxxx xxxxxxx.

XXXX XXXXX        Xxxx xxxx xxx xxx.

XXXX XXXXX        Xx xxxxxx xxxxxx xxx$ xxxx xxxx xxx xxxxxx.

XXXXX XXXXX       Xx xxxxxx xxxxxx xxx$ xxxx xxxxx xxx xxxxxx.

XXXXXXX XXXX XXX  Xx xxxxxx xxxxxx xxx$ xxxxxxxx xxx $Xxxxxx Xxxxxxx$ xxxxxx.

XXXXX xx XXXXXXXX Xx xxxxxx xxxxxx xxx$ xxxx xxxxxx xxxx $xxxxxx X$X$ X$X$.

XXX XX XXX XXX XXXX XXXX XXXXXX XXXXXXXX

----------------------------------------

Xxx xxxxxxxxx xxxxxx xxxxxxx xxx xx xxx xxx xxxxxxxx xx xxx xxxxxx xxxx Xxx$XxxxXxxx xxxxxxxx.

Xxx xx Xxxx$ Xxxx$ xxx Xxxxxxx Xxxxxxx

--------------------------------------

Xx xxxx xx xxxx x xxxxxx$

1.
Xxxxx xxxxx xxx xxxxxx xxxxxx xxx xxxxx $Xxxxxx Xxxxxxx$.

2.
Xx xxx $Xxxxxx Xxxxxxx$ xxxxxx xxx$ xxx xxx xxxxx xxxx xx xxxx xxx xxxxxxx xxxxxxx xxx $Xxxxxxxx xxxxxxx$ xx xxx $Xxxxxxxxx xxxxxxx$ xxxxx.
Xxxx xxxxxxx xx xxx $Xxxxxxxx Xxxxxxx$ xxx xxxxxx xx xxx xxxx xxxx xxxxxx.

Xx xxxxxxx xxxxxxx$

$$ Xxxx xxx xxxx xxx xxxxxx xxxx xxx xxxxxxx xxxxxxxx.
- xx$

1.
Xxxxx xxxxx xxx xxxxxx xxxxxx xxx xxxxx $Xxxxxx Xxxxxxx$.

2.
Xx xxx $Xxxxxx Xxxxxxx$ xxxxxx xxx$ xxx xxx $Xxxx xx$ xxx $Xxxx xxxx$ xxxxxxx xx xxxxxxx xxx xxxxxxx.
Xxxxxxx xx xxx xxx xx xxx xxxx xxxxxx xx xxx xxxx xx xxxxxxx xx xxx xxxxxx xx xxx xxxx xx xxx xxxx xxxx xxxxxx.

Xxx xx Xxxx Xxxxx Xxxx

----------------------
$$ Xx xxxx xxx xxxx$ xxxxx x xxxxxx xxxxxx.
$$ Xx xxxxxx xxx xxxx xxxxx$ xxxxx xxx xxxxxx xxxxxx xxxxx. Xxxx xxxx xxx xxxxx xxx xxxx xxxxxx$ xxx xxxx xxxxx xxxxxxx xxxxxxx xxxxxxxxx xx xxxxxxxxxx xxxxx. Xxx xxxxxxx xxxxx xx xxxxxxxxx xx x xxxxxxxx xx xxx xxxxxx xxxxxx.

Xxx xx Xxxxxx Xxxxx Xxxx

------------------------
$$ Xx xxxxxx x xxx$ xxxxx xxx xxx xx xxx xxx xx xx xxxx xxxxx xx xxxxxxxx xx xxx xxx.
$$ Xx xxxxxx xxx xxxx $xxxxxx xxx xxx xxxxxx xxx$$ xxxxx XXXX$X.
$$ Xx xxxxxx xxxxxxxxxxx xxxx$ xxxxx xxx xxxx xxx XXXXX xxx xxxxx xxxxxxxx xxx xxxx xx xxxxx xxx xxxxx xxxx.
$$ Xx xxxxxx xxxxxxxxxxxxxx xxxx$ xxxxx xxx XXXX xxx xxx xxxxx xx xxx x xxx xx xxx xxxxxxxxx.

Xxx xxxxxx xxxxxx xxxxxxx$ xxx xxx xxxxxx xxxxxx xxx xxxxxx xxxxxx xxxxxx xxx.

Xxx xx Xxxx Xxxx

----------------------
$$ Xx xxxx xxx xx xxxx xxxx xxxx xxx xxxxx$ xxxxxx xxx xxxx xxx xxxx xxxxx XXXX$X.

Xxx xxx xxxxx xxx xxxx xxxx xxx xxxx xx xxxxxxxxxxx xxxxxxx.
Xxx xxxxxx xxxx xxxxxxx xx xxxxx xx xxxx xxx xxx xxxxxx xxxx xxx xxxxxx xxxxxx xxx.

Xxx xx Xxxxxx xx xxx Xxxxx  $Xxxxx Xxxxxx$

---------------------------------

Xxx xxx $Xxxxxx$ xxx xx xxxxxx xxx xxxx xx xxx xxxxx.
Xxxx xxx xxxx xx xxx xxx$ xxxx xxxxx xxxx xxxxxxx xxx xxxxx xxxx xxxxxx xx xxx xxxxx.

$$ Xxxxxx xxx xxxx. Xx xxxxxx xxx xxxx xx xxx xxxxx$ xx xxx $Xxxxxx$ xxx$ xxxx xxx xxxx xx xxxx.
$$ Xxxxxx xxx xxxxxxxx xxxxx. Xx xxxxxx xxx xxxxxxxx xxxxx xx xxx xxxxx$ xxxx xxx xxxxx xxxxxxxxx xx xxxxxx. Xxx$XxxxXxxx xxxxxxxx xxxx xxxx xxxxxxx xxx xx xxx xxxxx $xxxxxxx XXX$.
$$ Xxxxxx xxx xxxxxxx xxxxxxx. Xx xxxxxx xxx xxxxxxx xxxx xxxxxxx xxxxxx xx xxxxxxx xxxxxxxxxx$ xxxxxxx xxx xxxxxx xx xxxxxxxxx xxxxx. Xxx$XxxxXxxx xxxxxxxx xxxx xxxx xxxxxxx xx xxxxx xxxxx xxx xxx xxxxxx.
$$ Xxxxxx xx xxxxxxx. Xx xxxxxx xxx xxxx xx xxx xx xxxx xxxxxxx$ xxx xxx xxxxxxxxx xxxxxx$

\<xxxxxx$$$$$xxxx$$ $$$$xxxxxx$$$$$xxxx$$$$ ...

Xxx xxxxxxx$ xx xxxx $Xxx$ xx xxx XxxxxxxXxxx xxxxxx$ xx xxx $Xxxxxx$ xxx$ xxxx$

xxxxxxxxxxx$xxx

Xx xxxx xxxx xxxx $Xxx$ xx xxx XxxxxxxXxxx xxx Xxxx xxxxxxx$ xx xxx $Xxxxxx$ xxx$ xxxx$

xxxxxxxxxxx$xxx  xxxx$xxx

$$ Xxxx xxx xxxxxx. Xx xxxxxxx xxx xxxxxx xxxxx xxxxx$ xxxxx xxx xxx X xxxxxx xx xxx xxx xxxxx xxxxxx xx xxx $Xxxxxx$ xxx xx xxxxxx xxx xxxx xxxx xxx Xxxxxx xxx.

Xxx Xxxxxxxx xx Xxxxxx xxx Xxxxx

--------------------------------

Xxx xxx xxx xxxxx xx $xxxxxxxx$ xx xxxxxxxxx xxxxx xxxxx xxx xxxxxxxxx xx xxx xxxxx.
Xxxxx xxxxxx xxxx xxxx xxxx xxxxxxx xxx xx xxx xxxxxxxx xxxx xxx xxxxxxxxx.
Xxx xxxxxxxxx xxxxxxxx xxx xxxxxxxxxx xx xxx xxxxxxxxxx xx xxx xxxxxxx xxxxxxxxx xx xxx xxxx xxxx xxxxxx xxx xxx .XXX Xxxxxxxxx xxxxx xx xxxxx xxxxxxxxxx.

Xxxx xxxxxxxxx xxx xxx xxxxxxxxx xxxxxx$

\<xxxxxx$$ $$xxxxxxxx$$ $$xxxxx\>

Xxxxxxxx xxx xxxxxxxxx xxxxxxxxxx xxx xxxxxxxxx xx XXX.
Xxxxxxxx xxx xxx xxxx xxxxxxxx xxx xxxxxxxxx xx XX.
Xxx xxxxxx xxxxxx xxx xxxxxxx xxxxxxxxxx.

Xxx xxxxxxxx xxxx xxxxxxx xxx xxxxxxx.
Xx xxxx xxx xxxxxx xxxxx xxxx xxx xxxxx.

Xxx xx Xxx Xxxxxxxx

---------------------------

1.
Xx xxxxxxx xxx $Xxx xxxxxxxx$ xxxx xxxxxx$ xx xxx xxxxx xxxxx xxxxxx xx xxx xxxxxx$ xxxxx xxx $Xxxxxx$ xxxxx.

2.
Xxxxx xxx $Xxx Xxxxxxxx$ xxxx xxxxxx.

3.
Xxxxx xx xxxxxx xxxxxxx $xxxxxxxxxx$.
Xxx xxx xxxxxx xxx xx xxxx xxxxxxxxxx.

4.
Xxxx xxx xxx xxxxxxxx xxxxxxxxx xxxxxxxxxx$ xxxxx xxx Xxx xxxxxx.

5.
Xx xxxxxx xxx xxxxxxxxx$ xxxxx Xxxxxx.

6.
Xx xxx xxxx xxxxxxxx$ xxxxx xxx Xxx Xxxxxxxx xxxxxx xxxxx.

Xxx xx Xxxx x Xxxxxxxxx

--------------------
$$ Xx xxxxxx xx xxxxxxxx$ xxxxx xxx xxxx xxxxxxxx xxxxx$ xxx xxxx xxxxx xx xxxxxx x xxxxxxxxx

xxxxxxxx xxxx xxx xxxx$xxxx xxxx.

$$ Xx xxxxx xx xxxxxx x xxxxx$ xxxx x xxxxx xx xxx xxxxx xxx. Xx xxx xxxxx x xxxxx xxxx xx xxx xxxxx$ x xxxxxxxx X xxxx xxxxxxx. Xx xxxxxx xx$ xxxxxx xxx xxxxx.
$$ Xx xxxxxx xx XX xxxxxxxxx$ xxx x xxxxxxxx xxxx xxx xxxx xxxxxxxx.

Xxx xx Xxxxxx Xxxxxxxx

-------------------------
$$ Xx xxxxxx xxxxxxxx xxxxxxxx$ xxxxx xxx xxx X xxxxxx xxxx xxxxxxxxx.
$$ Xx xxxxxx xxx xxxxxxxx$ xxxxx xxx $Xxxxx Xxx$ xxxxxx.

## XXXXXXX XXXXX

