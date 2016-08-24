---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294028
schema: 2.0.0
---

# Xxxxx$Xxxxx
## XXXXXXXX
Xxxxxx xx xxxxxx xx xxx xxxxx xxxxxx.

## XXXXXX

### XxXxxxxxxxx $Xxxxxxx$
```
Write-Error [-Message] <String> [-Category <ErrorCategory>] [-ErrorId <String>] [-TargetObject <Object>]
 [-RecommendedAction <String>] [-CategoryActivity <String>] [-CategoryReason <String>]
 [-CategoryTargetName <String>] [-CategoryTargetType <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### XxxxXxxxxxxxx
```
Write-Error -Exception <Exception> [[-Message] <String>] [-Category <ErrorCategory>] [-ErrorId <String>]
 [-TargetObject <Object>] [-RecommendedAction <String>] [-CategoryActivity <String>] [-CategoryReason <String>]
 [-CategoryTargetName <String>] [-CategoryTargetType <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### XxxxxXxxxxx
```
Write-Error -ErrorRecord <ErrorRecord> [-RecommendedAction <String>] [-CategoryActivity <String>]
 [-CategoryReason <String>] [-CategoryTargetName <String>] [-CategoryTargetType <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxx$Xxxxx xxxxxx xxxxxxxx x xxx$xxxxxxxxxxx xxxxx.
Xx xxxxxxx$ xxxxxx xxx xxxx xx xxx xxxxx xxxxxx xx xxx xxxx xxxxxxx xx xx xxxxxxxxx$ xxxxx xxxx xxxxxx.

Xx xxxxx x xxx$xxxxxxxxxxx xxxxx$ xxxxx xx xxxxx xxxxxxx xxxxxx$ xx XxxxxXxxxxx xxxxxx$ xx xx Xxxxxxxxx xxxxxx. Xxx xxx xxxxx xxxxxxxxxx xx Xxxxx$Xxxxx xx xxxxxxxx xxx xxxxx xxxxxx.

Xxx$xxxxxxxxxxx xxxxxx xxxxx xx xxxxx xx xxx xxxxx xxxxxx$ xxx xxxx xx xxx xxxx xxxxxxx xxxxxxxxxx.
Xx x xxx$xxxxxxxxxxx xxxxx xx xxxxxxxx xx xxx xxxx xx x xxxxxxxxxx xx xxxxx xxxxx$ xxx xxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxx xxxxx xx xxx xxxxxxxxxx.

Xx xxxxxxx x xxxxxxxxxxx xxxxx$ xxx xxx Xxxxx xxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxx xxxxx$Xxxxx $xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000$.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Get-ChildItem | ForEach-Object { if ($_.GetType().ToString() -eq "Microsoft.Win32.RegistryKey") {Write-Error "Invalid object" -ErrorID B1 -Targetobject $_ } else {$_ } }
```

Xxxx xxxxxxx xxxxxxxx x xxx$xxxxxxxxxxx xxxxx xxxx xxx Xxx$XxxxxXxxx xxxxxx xxxxxxx x Xxxxxxxxx.Xxx00.XxxxxxxxXxx xxxxxx$ xxxx xx xxx xxxxxxx xx xxx XXXX$ xx XXXX$ xxxxxx xx xxx Xxxxxxx XxxxxXxxxx Xxxxxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Write-Error "Access denied."
```

Xxxx xxxxxxx xxxxxxxx x xxx$xxxxxxxxxxx xxxxx xxx xxxxxx xx $Xxxxxx xxxxxx$ xxxxx.
Xxx xxxxxxx xxxx xxx Xxxxxxx xxxxxxxxx xx xxxxxxx xxx xxxxxxx$ xxx xxxxx xxx xxxxxxxx Xxxxxxx xxxxxxxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>Write-Error -Message "Error: Too many input values." -Category InvalidArgument
```

Xxxx xxxxxxx xxxxxxxx x xxx$xxxxxxxxxxx xxxxx xxx xxxxxxxxx xx xxxxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$e = [System.Exception]@{$e = [System.Exception]@{Source="Get-ParameterNames.ps1";HelpLink="http://go.microsoft.com/fwlink/?LinkID=113425"}HelpLink="http://go.microsoft.com/fwlink/?LinkID=113425"}
PS C:\> Write-Error $e -Message "Files not found. The $Files location does not contain any XML files."
```

Xxxx xxxxxxx xxxx xx Xxxxxxxxx xxxxxx xx xxxxxxx x xxx$xxxxxxxxxxx xxxxx.

Xxx xxxxx xxxxxxx xxxx x xxxx xxxxx xx xxxxxx xxx Xxxxxx.Xxxxxxxxx xxxxxx.
Xx xxxxx xxx xxxxxxxxx xxxxxx xx xxx $x xxxxxxxx.
Xxx xxx xxx x xxxx xxxxx xx xxxxxx xxx xxxxxx xx x xxxx xxxx xxx x xxxx xxxxxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx Xxxxx$Xxxxx xxxxxx xx xxxxxxx x xxx$xxxxxxxxxxx xxxxx.
Xxx xxxxx xx xxx Xxxxxxxxx xxxxxxxxx xx xxx Xxxxxxxxx xxxxxx xx xxx $x xxxxxxxx.

## XXXXXXXXXX

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxxxxx xx xxx xxxxx.
Xxx xxxxxxx xxxxx xx XxxXxxxxxxxx.

Xxx xxxxxxxxxxx xxxxx xxx xxxxx xxxxxxxxxx$ xxx $XxxxxXxxxxxxx Xxxxxxxxxxx$ xx xxx XXXX $Xxxxxxxxx Xxxxxxxxx Xxxxxxx$ xxxxxxx xx xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXx$000000.

```yaml
Type: ErrorCategory
Parameter Sets: NoException, WithException
Aliases: 
Accepted values: NotSpecified, OpenError, CloseError, DeviceError, DeadlockDetected, InvalidArgument, InvalidData, InvalidOperation, InvalidResult, InvalidType, MetadataError, NotImplemented, NotInstalled, ObjectNotFound, OperationStopped, OperationTimeout, SyntaxError, ParserError, PermissionDenied, ResourceBusy, ResourceExists, ResourceUnavailable, ReadError, WriteError, FromStdErr, SecurityError, ProtocolError, ConnectionError, AuthenticationError, LimitsExceeded, QuotaExceeded, NotEnabled

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxXxxxxxxx
Xxxxxxxxx xxx xxxxxx xxxx xxxxxx xxx xxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Activity

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxXxxxxx
Xxxxxxxx xxx xx xxx xxx xxxxxxxx xxxxxx xxx xxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Reason

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxXxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxx xxx xxxxx xxxxxxxxx xxxx xxx xxxxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: TargetName

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxXxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxx xxxx xxx xxxxx xxxxxxxxx xxxx xxx xxxxx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: TargetType

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXx
Xxxxxxxxx xx XX xxxxxx xx xxxxxxxx xxx xxxxx.
Xxx xxxxxx xxxxxx xx xxxxxx xx xxx xxxxx.

```yaml
Type: String
Parameter Sets: NoException, WithException
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxx
Xxxxxxxxx xx xxxxx xxxxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxx.
Xxx xxx xxxxxxxxxx xx xxx xxxxxx xx xxxxxxxx xxx xxxxx.

Xx xxxxxx xx xxxxx xxxxxx xxxxxx$ xxx xxx Xxx$Xxxxxx xxxxxx xx xxx xx xxxxx xxxxxx xxxxxx xxxx xxx xxxxx xx xxx $Xxxxx xxxxxxxxx xxxxxxxx.

```yaml
Type: ErrorRecord
Parameter Sets: ErrorRecord
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxxx
Xxxxxxxxx xx xxxxxxxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxx.
Xxx xxx xxxxxxxxxx xx xxx xxxxxx xx xxxxxxxx xxx xxxxx.

Xx xxxxxx xx xxxxxxxxx xxxxxx$ xxx x xxxx xxxxx xx xxx xxx Xxx$Xxxxxx xxxxxx.

```yaml
Type: Exception
Parameter Sets: WithException
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxxxXxxxxx
Xxx xxxxxxxxxxx xxxxx xxx xxxxx xxxxxxxxxx$ xxx $XxxxxXxxxxxxx Xxxxxxxxxxx$ xx xxx XXXX $Xxxxxxxxx Xxxxxxxxx Xxxxxxx$ xxxxxxx xx xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXx$000000.

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
Xxx xxxxxxxxxxx xxxxx xxx xxxxx xxxxxxxxxx$ xxx $XxxxxXxxxxxxx Xxxxxxxxxxx$ xx xxx XXXX $Xxxxxxxxx Xxxxxxxxx Xxxxxxx$ xxxxxxx xx xxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXx$000000.

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

### $Xxxxxxx
Xxxxxxxxx xxx xxxxxxx xxxx xx xxx xxxxx. Xx xxx xxxx xxxxxxxx xxxxxx xx xxxxxxx xxxxxxxxxx$ xxxxxxx xx xx xxxxxxxxx xxxxx.
Xxx xxx xxxx xxxx x xxxxxxx xxxxxx xx Xxxxx$Xxxxx.

```yaml
Type: String
Parameter Sets: NoException
Aliases: Msg

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: WithException
Aliases: Msg

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### $XxxxxxxxxxxXxxxxx
Xxxxxxxxx xxx xxxxxx xxxx xxx xxxx xxxxxx xxxx xx xxxxxxx xx xxxxxxx xxx xxxxx.

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

### $XxxxxxXxxxxx
Xxxxxxxxx xxx xxxxxx xxxx xxx xxxxx xxxxxxxxx xxxx xxx xxxxx xxxxxxxx.
Xxxxx xxx xxxxxx $xxxx xx x xxxxxx$$ x xxxxxxxx xxxx xxxxxxxx xxx xxxxxx$ xx x xxxxxxx xxxx xxxx xxx xxxxxx.

```yaml
Type: Object
Parameter Sets: NoException, WithException
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### Xxxxxx.Xxxxxx
Xxx xxx xxxx x xxxxxx xxxx xxxxxxxx xx xxxxx xxxxxxx xx Xxxxx$Xxxxx.

## XXXXXXX

### Xxxxx xxxxxx
Xxxxx$Xxxxx xxxxxx xxxx xx xxx xxxxx xxxxxx.
Xx xxxx xxx xxxxxx xxx xxxxxxx.

## XXXXX

## XXXXXXX XXXXX

[Xxxxx$Xxxxx]()

[Xxxxx$Xxxx]()

[Xxxxx$Xxxxxx]()

[Xxxxx$Xxxxxxxx]()

[Xxxxx$Xxxxxxx]()

[Xxxxx$Xxxxxxx]()

