---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=525909
schema: 2.0.0
---

# Xxxxx$Xxxxxxxxxxx
## XXXXXXXX
Xxxxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xxxxxxxxxxx xxxxxx xxxx xxx x xxxxxxx.

## XXXXXX

```
Write-Information [-MessageData] <Object> [[-Tags] <String[]>]
```

## XXXXXXXXXXX
Xxxxxxx XxxxxXxxxx 0.0 xxxxxxxxxx x xxx$ xxxxxxxxxx xxxxxxxxxxx xxxxxx $xxxxxx 0 xx Xxxxxxx XxxxxXxxxx xxxxxxx$ xxxx xxx xxx xxx xx xxxxxxxx xxxxxxxxxx xxxx xxxxxxx x xxxxxx xxx xxx xxxxxxx $xx xxxxxxx xxxxxxxxxxx$.
Xxxxx$Xxxxxxxxxxx xxxx xxx xxx xx xxxxxxxxxxxxx xxxxxxx xx xxx xxxxxx$ xxx xxxxxxx xxx Xxxxxxx XxxxxXxxxx xxxxxxx xxxxxxxxxxx xxxxxx xxxx xxx x xxxxxxx.

Xxx $XxxxxxxxxxxXxxxxxxxxx xxxxxxxxxx xxxxxxxx xxxxx xxxxxxxxxx xxxxxxx xxx xxxxxxx xxx xxxxxxx xx Xxxxx$Xxxxxxxxxxx xx xxxxxxxxx xx xxx xxxxxxxx xxxxx xx x xxxxxx$x xxxxxxxxx.
Xxxxxxx xxx xxxxxxx xxxxx xx xxxx xxxxxxxx xx XxxxxxxxXxxxxxxx$ xx xxxxxxx$ xxxxxxxxxxxxx xxxxxxxx xxx xxx xxxxx.
Xx xxx xxx$x xxxx xx xxxxxx xxx xxxxx xx $XxxxxxxxxxxXxxxxxxxxx$ xxx xxx xxxxxxxx xxx xxxxx xx xxxxxx xxx XxxxxxxxxxxXxxxxx xxxxxx xxxxxxxxx xx xxxx xxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxxxxxxx$Xxxxxxxxx xxx xxxxx$XxxxxxXxxxxxxxxx.

Xxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0$ Xxxxx$Xxxx xx x xxxxxxx xxx Xxxxx$Xxxxxxxxxxx.
Xxx xxx xxx xxx Xxxxx$Xxxx xx xxxx xxxxxx xx xxx xxxxxxxxxxx xxxxxx$ xxx xxx $XxxxxxxxxxxXxxxxxxxxx xxxxxxxxxx xxxxxxxx xxx XxxxxxxxxxxXxxxxx xxxxxx xxxxxxxxx xx xxx xxxxxx Xxxxx$Xxxx xxxxxxxx.
Xxxxxxxxxxx xxxxxxx xxxx xxxx xxx XxxxxXxxxx.Xxxxxxx$ xxxx$ xxxxxxxxx xxxx$ xxx xxxxxxxxx.

Xxxxx$Xxxxxxxxxxx xx xxxx x xxxxxxxxx xxxxxxxx xxxxxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-WindowsFeature -Name p*; Write-Information -MessageData "Got your features!" -InformationAction Continue
Display Name                                            Name                       Install State
------------                                            ----                       -------------
[ ] Print and Document Services                         Print-Services                 Available
    [ ] Print Server                                    Print-Server                   Available
    [ ] Distributed Scan Server                         Print-Scan-Server              Available
    [ ] Internet Printing                               Print-Internet                 Available
    [ ] LPD Service                                     Print-LPD-Service              Available
[ ] Peer Name Resolution Protocol                       PNRP                           Available
[X] Windows PowerShell                                  PowerShellRoot                 Installed
    [X] Windows PowerShell 5.0                          PowerShell                     Installed
    [ ] Windows PowerShell 2.0 Engine                   PowerShell-V2                    Removed
    [X] Windows PowerShell ISE                          PowerShell-ISE                 Installed
Got your features!
```

Xx xxxx xxxxxxx$ xxx xxxx xx xxxxxxxxxxxxx xxxxxxx$ $Xxx xxxx xxxxxxxx$$$ xxxxx xxxxxxx xxx Xxx$XxxxxxxXxxxxxx xxxxxxx xx xxxx xxx xxxxxxxx xxxx xxxx x Xxxx xxxxx xxxx xxxxxx xxxx $x$.
Xxxxxxx xxx $XxxxxxxxxxxXxxxxxxxxx xxxxxxxx xx xxxxx xxx xx xxx xxxxxxx$ XxxxxxxxXxxxxxxx$ xxx xxx xxx XxxxxxxxxxxXxxxxx xxxxxxxxx xx xxxxxxxx xxx $XxxxxxxxxxxXxxxxxxxxx xxxxx$ xxx xxxx xxx xxxxxxx.
Xxx XxxxxxxxxxxXxxxxx xxxxx xx Xxxxxxxx$ xxxxx xxxxx xxxx xxxx xxxxxxx xx xxxxx$ xxx xxx xxxxxx xx xxxxxxx xxxxxxxxx$ xx xx xx xxx xxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-WindowsFeature -Name p*; Write-Information -MessageData "To filter your results for PowerShell, pipe your results to the Where-Object cmdlet." -Tags "Instructions" -InformationAction Continue
Display Name                                            Name                       Install State
------------                                            ----                       -------------
[ ] Print and Document Services                         Print-Services                 Available
    [ ] Print Server                                    Print-Server                   Available
    [ ] Distributed Scan Server                         Print-Scan-Server              Available
    [ ] Internet Printing                               Print-Internet                 Available
    [ ] LPD Service                                     Print-LPD-Service              Available
[ ] Peer Name Resolution Protocol                       PNRP                           Available
[X] Windows PowerShell                                  PowerShellRoot                 Installed
    [X] Windows PowerShell 5.0                          PowerShell                     Installed
    [ ] Windows PowerShell 2.0 Engine                   PowerShell-V2                    Removed
    [X] Windows PowerShell ISE                          PowerShell-ISE                 Installed
To filter your results for PowerShell, pipe your results to the Where-Object cmdlet.
```

Xx xxxx xxxxxxx$ xxx xxx Xxxxx$Xxxxxxxxxxx xx xxx xxxxx xxxx xxxx$xx xxxx xx xxx xxxxxxx xxxxxxx xxxxx xxxx$xx xxxx xxxxxxx xxx xxxxxxx xxxxxxx.
Xxx xxxxxxx xxxx xxx xxx Xxxxxxxxxxxx xx xxx xxxxxxxxxxxxx xxxxxxx.
Xxxxx xxxxxxx xxxx xxxxxxx$ xx xxx xxxxxx xxx xxxxxxxxxxx xxxxxx xxx xxxxxxxx xxxxxx Xxxxxxxxxxxx$ xxx xxxxxxx xxxxxxxxx xxxx xxxxx xx xxxxx xxx xxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>function Test-Info
       { 
         Get-Process P*
         Write-Information "Here you go"
       }
Test-Info 6> Info.txt
```

Xx xxxx xxxxxxx$ xxx xxxxxxxx xxx xxxxxxxxxxx xxxxxx xx xxx xxxxxxxx xx x xxxx$ Xxxx.xxx$ xx xxxxx xxx xxxx 0$$.
Xxxx xxx xxxx xxx Xxxx.xxx xxxx$ xxx xxx xxx xxxx$ $Xxxx xxx xx.$

## XXXXXXXXXX

### $XxxxxxxXxxx
Xxxxxxxxx xx xxxxxxxxxxxxx xxxxxxx xxxx xxx xxxx xx xxxxxxx xx xxxxx xx xxxx xxx x xxxxxx xx xxxxxxx.
Xxx xxxx xxxxxxx$ xxxxxxx xxx xxxxxxxxxxxxx xxxxxxx xx xxxxxxxxx xxxxx.
Xx xxxxxxx xx $Xxxx xxxxxxxx.$

```yaml
Type: Object
Parameter Sets: (All)
Aliases: Msg

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxx
Xxxxxxxxx x xxxxxx xxxxxx xxxx xxx xxx xxx xx xxxx xxx xxxxxx xxxxxxxx xxxx xxx xxxx xxxxx xx xxx xxxxxxxxxxx xxxxxx xxxx Xxxxx$Xxxxxxxxxxx.
Xxxx xxxxxxxxx xxxxx xxxxxxxxx xx xxx Xxxx xxxxxxxxx xx Xxx$XxxxxxXxxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### 
Xxxxx$Xxxxxxxxxxx xxxx xxx xxxxxx xxxxx xxxxx.

## XXXXXXX

### Xxxxxx.Xxxxxxxxxx.Xxxxxxxxxx.XxxxxxxxxxxXxxxxx

## XXXXX

## XXXXXXX XXXXX

[xxxxx$XxxxxxXxxxxxxxxx]()

[xxxxx$Xxxxxxxxxxx]()

[xxxxx$Xxxxxxxxxx$Xxxxxxxxx]()

