---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294010
schema: 2.0.0
---

# Send-MailMessage
## XXXXXXXX
Xxxxx xx x$xxxx xxxxxxx.

## XXXXXX

```
Send-MailMessage [-Attachments <String[]>] [-Bcc <String[]>] [[-Body] <String>] [-BodyAsHtml]
 [-Encoding <Encoding>] [-Cc <String[]>] [-DeliveryNotificationOption <DeliveryNotificationOptions>]
 -From <String> [[-SmtpServer] <String>] [-Priority <MailPriority>] [-Subject] <String> [-To] <String[]>
 [-Credential <PSCredential>] [-UseSsl] [-Port <Int32>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxx$XxxxXxxxxxx xxxxxx xxxxx xx x$xxxx xxxxxxx xxxx xxxxxx Xxxxxxx XxxxxXxxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>send-mailmessage -to "User01 <user01@example.com>" -from "User02 <user02@example.com>" -subject "Test mail"
```

Xxxx xxxxxxx xxxxx xx x$xxxx xxxxxxx xxxx Xxxx00 xx Xxxx00.

Xxx xxxx xxxxxxx xxx x xxxxxxx$ xxxxx xx xxxxxxxx$ xxx xx xxxx xxx xxxx x xxxx$ xxxxx xx xxxxxxxx.
Xxxx$ xxxxxxx xxx XxxxXxxxxx xxxxxxxxx xx xxx xxxxxxxxx$ Xxxx$XxxxXxxxxxx xxxx xxx xxxxx xx xxx $XXXxxxxXxxxxx xxxxxxxxxx xxxxxxxx xxx xxx XXXX xxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>send-mailmessage -from "User01 <user01@example.com>" -to "User02 <user02@example.com>", "User03 <user03@example.com>" -subject "Sending the Attachment" -body "Forgot to send the attachment. Sending now." -Attachments "data.csv" -priority High -dno onSuccess, onFailure -smtpServer smtp.fabrikam.com
```

Xxxx xxxxxxx xxxxx xx x$xxxx xxxxxxx xxxx xx xxxxxxxxxx xxxx Xxxx00 xx xxx xxxxx xxxxx.

Xx xxxxxxxxx x xxxxxxxx xxxxx xx $Xxxx$ xxx xxxxxxxx x xxxxxxxx xxxxxxxxxxxx xx x$xxxx xxxx xxx x$xxxx xxxxxxxx xxx xxxxxxxxx xx xxxx xxxx xxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>send-mailmessage -to "User01 <user01@example.com>" -from "ITGroup <itdept@example.com>" -cc "User02 <user02@example.com>" -bcc "ITMgr <itmgr@example.com>" -subject "Don't forget today's meeting!" -credential domain01\admin01 -useSSL
```

Xxxx xxxxxxx xxxxx xx x$xxxx xxxxxxx xxxx Xxxx00 xx xxx XXXxxxx xxxxxxx xxxx xxxx x xxxx $XX$ xx Xxxx00 xxx x xxxxx xxxxxx xxxx $XXX$ xx xxx XX xxxxxxx $XXXxx$.

Xxx xxxxxxx xxxx xxx xxxxxxxxxxx xx x xxxxxx xxxxxxxxxxxxx xxx xxx XxxXXX xxxxxxxxx.

## XXXXXXXXXX

### -Attachments
Xxxxxxxxx xxx xxxx xxx xxxx xxxxx xx xxxxx xx xx xxxxxxxx xx xxx x$xxxx xxxxxxx.
Xxx xxx xxx xxxx xxxxxxxxx xx xxxx xxx xxxxx xxx xxxx xxxxx xx Xxxx$XxxxXxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: PsPath

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Bcc
Xxxxxxxxx xxx x$xxxx xxxxxxxxx xxxx xxxxxxx x xxxx xx xxx xxxx xxx xxx xxx xxxxxx xx xxxxxxxxxx xx xxx xxxxxxx.
Xxxxx xxxxx $xxxxxxxx$ xxx xxx x$xxxx xxxxxxx$ xxxx xx $Xxxx $$xxxxxxx$xxxxxxx.xxx$$$.

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

### -Body
Xxxxxxxxx xxx xxxx $xxxxxxx$ xx xxx x$xxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyAsHtml
Xxxxxxxxx xxxx xxx xxxxx xx xxx Xxxx xxxxxxxxx xxxxxxxx XXXX.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: BAH

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Cc
Xxxxxxxxx xxx x$xxxx xxxxxxxxx xx xxxxx x xxxxxx xxxx $XX$ xx xxx x$xxxx xxxxxxx xx xxxx.
Xxxxx xxxxx $xxxxxxxx$ xxx xxx x$xxxx xxxxxxx$ xxxx xx $Xxxx $$xxxxxxx$xxxxxxx.xxx$$$.

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

### -Credential
Xxxxxxxxx x xxxx xxxxxxx xxxx xxx xxxxxxxxxx xx xxxxxxx xxxx xxxxxx.
Xxx xxxxxxx xx xxx xxxxxxx xxxx.

Xxxx x xxxx xxxx$ xxxx xx $Xxxx00$ xx $Xxxxxx00$Xxxx00$.
Xx$ xxxxx x XXXxxxxxxxxx xxxxxx$ xxxx xx xxx xxxx xxx Xxx$Xxxxxxxxxx xxxxxx.

```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeliveryNotificationOption
Xxxxxxxxx xxx xxxxxxxx xxxxxxxxxxxx xxxxxxx xxx xxx x$xxxx xxxxxxx.
Xxx xxx xxxxxxx xxxxxxxx xxxxxx.
$Xxxx$ xx xxx xxxxxxx xxxxx. Xxx xxxxx xxx xxxx xxxxxxxxx xx $xxx$.

Xxx xxxxxxxx xxxxxxxxxxxxx xxx xxxx xx xx x$xxxx xxxxxxx xx xxx xxxxxxx xxxxxxxxx xx xxx xxxxx xx xxx Xx xxxxxxxxx.

Xxxxx xxxxxx xxx$

$$ Xxxx$ Xx xxxxxxxxxxxx.
$$ XxXxxxxxx$ Xxxxxx xx xxx xxxxxxxx xx xxxxxxxxxx.
$$ XxXxxxxxx$ Xxxxxx xx xxx xxxxxxxx xx xxxxxxxxxxxx.
$$ Xxxxx$ Xxxxxx xx xxx xxxxxxxx xx xxxxxxx.
$$ Xxxxx$ Xxxxx xxxxxx.

```yaml
Type: DeliveryNotificationOptions
Parameter Sets: (All)
Aliases: DNO
Accepted values: None, OnSuccess, OnFailure, Delay, Never

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Encoding
Xxxxxxxxx xxx xxxxxxxx xxxx xxx xxx xxxx xxx xxxxxxx.
Xxxxx xxxxxx xxx XXXXX$ XXX0$ XXX0$ XXX00$ Xxxxxxx$ XxxXxxxxxXxxxxxx$ Xxxxxxx$ xxx XXX.
XXXXX xx xxx xxxxxxx.

```yaml
Type: Encoding
Parameter Sets: (All)
Aliases: BE

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -From
Xxxxxxxxx xxx xxxxxxx xxxx xxxxx xxx xxxx xx xxxx.
Xxxxx x xxxx $xxxxxxxx$ xxx x$xxxx xxxxxxx$ xxxx xx $Xxxx $$xxxxxxx$xxxxxxx.xxx$$$.
Xxxx xxxxxxxxx xx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
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

### -Port
Xxxxxxxxx xx xxxxxxxxx xxxx xx xxx XXXX xxxxxx.
Xxx xxxxxxx xxxxx xx 00$ xxxxx xx xxx xxxxxxx XXXX xxxx.
Xxxx xxxxxxxxx xx xxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0 xxx xxxxx xxxxxxxx.

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

### -Priority
Xxxxxxxxx xxx xxxxxxxx xx xxx x$xxxx xxxxxxx.
Xxx xxxxx xxxxxx xxx xxxx xxx Xxxxxx$ Xxxx$ xxx Xxx.
Xxxxxx xx xxx xxxxxxx.

```yaml
Type: MailPriority
Parameter Sets: (All)
Aliases: 
Accepted values: Normal, Low, High

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SmtpServer
Xxxxxxxxx xxx xxxx xx xxx XXXX xxxxxx xxxx xxxxx xxx x$xxxx xxxxxxx.

Xxx xxxxxxx xxxxx xx xxx xxxxx xx xxx $XXXxxxxXxxxxx xxxxxxxxxx xxxxxxxx.
Xx xxx xxxxxxxxxx xxxxxxxx xx xxx xxx xxx xxxx xxxxxxxxx xx xxxxxxx$ xxx xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: ComputerName

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subject
Xxxxxxxxx xxx xxxxxxx xx xxx x$xxxx xxxxxxx.
Xxxx xxxxxxxxx xx xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: sub

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -To
Xxxxxxxxx xxx xxxxxxxxx xx xxxxx xxx xxxx xx xxxx.
Xxxxx xxxxx $xxxxxxxx$ xxx xxx x$xxxx xxxxxxx$ xxxx xx $Xxxx $$xxxxxxx$xxxxxxx.xxx$$$.
Xxxx xxxxxxxxx xx xxxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UseSsl
Xxxx xxx Xxxxxx Xxxxxxx Xxxxx $XXX$ xxxxxxxx xx xxxxxxxxx x xxxxxxxxxx xx xxx xxxxxx xxxxxxxx xx xxxx xxxx.
Xx xxxxxxx$ XXX xx xxx xxxx.

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

## XXXXXX

### System.String
Xxx xxx xxxx xxx xxxx xxx xxxx xxxxx xx xxxxxxxxxxx xx Xxxx$XxxxXxxxxxx.

## XXXXXXX

### None
Xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

## XXXXX

## XXXXXXX XXXXX

