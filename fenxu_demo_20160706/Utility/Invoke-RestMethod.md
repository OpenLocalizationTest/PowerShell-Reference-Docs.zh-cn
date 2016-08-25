---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293987
schema: 2.0.0
---

# Invoke-RestMethod
## XXXXXXXX
Xxxxx xx XXXX xx XXXXX xxxxxxx xx x XXXXxxx xxx xxxxxxx.

## XXXXXX

```
Invoke-RestMethod [-Method <WebRequestMethod>] [-UseBasicParsing] [-Uri] <Uri>
 [-WebSession <WebRequestSession>] [-SessionVariable <String>] [-Credential <PSCredential>]
 [-UseDefaultCredentials] [-CertificateThumbprint <String>] [-Certificate <X509Certificate>]
 [-UserAgent <String>] [-DisableKeepAlive] [-TimeoutSec <Int32>] [-Headers <IDictionary>]
 [-MaximumRedirection <Int32>] [-Proxy <Uri>] [-ProxyCredential <PSCredential>] [-ProxyUseDefaultCredentials]
 [-Body <Object>] [-ContentType <String>] [-TransferEncoding <String>] [-InFile <String>] [-OutFile <String>]
 [-PassThru] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XxxxXxxxxx xxxxxx xxxxx XXXX xxx XXXXX xxxxxxxx xx Xxxxxxxxxxxxxxxx Xxxxx Xxxxxxxx $XXXX$ xxx xxxxxxxx xxxx xxxxxxx xxxxxx xxxxxxxxxx xxxx.

Xxxxxxx XxxxxXxxxx xxxxxxx xxx xxxxxxxx xxxxx xx xxx xxxx xxxx.
Xxx xx XXX xx XXXX xxxx$ Xxxxxxx XxxxxXxxxx xxxxxxx xxx Xxxx xx Xxxxx XXX xxxxx.
Xxx XxxxXxxxxx Xxxxxx Xxxxxxxx $XXXX$ xx XXX$ Xxxxxxx XxxxxXxxxx xxxxxxxx $xx xxxxxxxxxxxx$ xxx xxxxxxx xxxx xxxxxxx.

Xxxx xxxxxx xx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

## XXXXXXXX

### Xxxxxxx 0
```
PS C:\>Invoke-RestMethod -Uri http://blogs.msdn.com/powershell/rss.aspx | Format-Table -Property Title, pubDate
Title                                                                 pubDate-----------
Another Holiday Gift from the PowerShell Team: PowerShell 3.0 CTP2... Thu, 22 Dec 2011 00:46:00 GMT
More Videos from the First PowerShell Deep Dive                       Mon, 10 Oct 2011 19:59:00 GMT
PowerShell Deep Dive Lineup                                           Thu, 06 Oct 2011 00:42:00 GMT
Windows Management Framework 3.0 Community Technology Preview (CTP... Mon, 19 Sep 2011 23:56:26 GMT
Get-Help -Online Fails in German                                      Tue, 23 Aug 2011 15:02:00 GMT
PowerShell Deep Dive Registration Info & Call for Session Proposals   Wed, 20 Jul 2011 00:25:00 GMT
Invoke-Expression considered harmful                                  Fri, 03 Jun 2011 15:43:00 GMT
PowerShell at TechEd 2011                                             Thu, 28 Apr 2011 16:58:36 GMT
PowerShell Language now licensed under the Community Promise          Sat, 16 Apr 2011 00:13:00 GMT
Scaling and Queuing PowerShell Background Jobs                        Mon, 04 Apr 2011 20:30:58 GMT
More Deep Dive Info, Including Abstracts from the PowerShell Team     Sun, 13 Mar 2011 01:35:42 GMT
A Few Deep Dive Abstracts                                             Sat, 05 Mar 2011 00:26:00 GMT
Reminder: Register for the PowerShell Deep Dive Conference & submi... Wed, 23 Feb 2011 17:55:45 GMT
```

Xxxx xxxxxxx xxxx xxx Xxxxxx$XxxxXxxxxx xxxxxx xx xxx xxxxxxxxxxx xxxx xxx Xxxxxxx XxxxxXxxxx Xxxx XXX xxxx.
Xxx xxxxxxx xxxx xxx Xxxxxx$Xxxxx xxxxxx xx xxxxxxx xxx xxxxxx xx xxx Xxxxx xxx xxxXxxx xxxxxxxxxx xx xxxx xxxx xx x xxxxx.

### Xxxxxxx 0
```
PS C:\>$cred = Get-Credential

# Next, allow the use of self-signed SSL certificates.

[System.Net.ServicePointManager]::ServerCertificateValidationCallback = { $true }

# Create variables to store the values consumed by the Invoke-RestMethod command. The search variable contents are later embedded in the body variable.

$server = 'server.contoso.com'
$url = "https://${server}:8089/services/search/jobs/export"
$search = "search index=_internal | reverse | table index,host,source,sourcetype,_raw"

# The cmdlet handles URL encoding. The body variable describes the search criteria, specifies CSV as the output mode, and specifies a time period for returned data that starts two days ago and ends one day ago. The body variable specifies values for parameters that apply to the particular REST API with which Invoke-RestMethod is communicating.

$body = @{
    search = $search
    output_mode = "csv"
    earliest_time = "-2d@d"
    latest_time = "-1d@d"
}

# Now, run the Invoke-RestMethod command with all variables in place, specifying a path and file name for the resulting CSV output file.

Invoke-RestMethod -Method Post -Uri $url -Credential $cred -Body $body -OutFile output.csv
cmdlet Get-Credential at command pipeline position 1

Supply values for the following parameters: 
{"preview":true,"offset":0,"result":{"sourcetype":"contoso1","count":"9624"}}

{"preview":true,"offset":1,"result":{"sourcetype":"contoso2","count":"152"}}

{"preview":true,"offset":2,"result":{"sourcetype":"contoso3","count":"88494"}}

{"preview":true,"offset":3,"result":{"sourcetype":"contoso4","count":"15277"}}
```

Xx xxx xxxxxxxxx xxxxxxx$ x xxxx xxxx Xxxxxx$XxxxXxxxxx xx xxxxxxx x XXXX xxxxxxx xx xx xxxxxxxx xxxxxxx xx xxx xxxx$x xxxxxxxxxxxx.

## XXXXXXXXXX

### -Body
Xxxxxxxxx xxx xxxx xx xxx xxxxxxx.
Xxx xxxx xx xxx xxxxxxx xx xxx xxxxxxx xxxx xxxxxxx xxx xxxxxxx.
Xxx xxx xxxx xxxx x xxxx xxxxx xx Xxxxxx$XxxxXxxxxx.

Xxx Xxxx xxxxxxxxx xxx xx xxxx xx xxxxxxx x xxxx xx xxxxx xxxxxxxxxx xx xxxxxxx xxx xxxxxxx xx xxx xxxxxxxx.

Xxxx xxx xxxxx xx x XXX xxxxxxx$ xxx xxx xxxx xx xx XXxxxxxxxxx $xxxxxxxxx$ x xxxx xxxxx$$ xxx xxxx xx xxxxx xx xxx XXX xx xxxxx xxxxxxxxxx.
Xxx xxxxx xxxxxxx xxxxx $xxxx xx XXXX$$ xxx xxxx xx xxx xx xxx xxxxx xx xxx xxxxxxx xxxx xx xxx xxxxxxxx xxxx$xxxxx xxxxxx.

Xxxx xxx xxxx xx x xxxx$ xx xx xx xxx xxxxxx xx xxxxxxx Xxxxxx$XxxXxxxxxx xxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxxxx xxxxxxx xx xxx xxxx xxxxxx.

Xxx xxxxxxx$

$x $ Xxxxxx$XxxXxxxxxx xxxx$$$xxxxxxx.xxx$xxxxx.xxxx $x.Xxxxx$$0$$.Xxxx $ $XxXxxx$ $x.Xxxxx$$0$$.Xxxxxxxx $ $XxXxxxxxxx$ Xxxxxx$XxxxXxxxxx xxxx$$$xxxxxxx.xxx$xxxxxxx.xxxx $Xxxx $x

- xx $

Xxxxxx$XxxxXxxxxx xxxx$$$xxxxxxx.xxx$xxxxxxx.xxxx $Xxxx $x.Xxxxx$$0\]

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Certificate
Xxxxxxxxx xxx xxxxxx xxxxxxxxxxx xxxx xx xxxx xxx x xxxxxx xxx xxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxxx x xxxxxxxxxxx xx x xxxxxxx xx xxxxxxxxxx xxxx xxxx xxx xxxxxxxxxxx.

Xx xxxx x xxxxxxxxxxx$ xxx Xxx$XxxXxxxxxxxxxx xx xxx xxx Xxx$XxxxxXxxx xxxxxx xx xxx Xxxxxxxxxxx $Xxxx$$ xxxxx.
Xx xxx xxxxxxxxxxx xx xxx xxxxx xx xxxx xxx xxxx xxxxxxxxxx xxxxxxxxx$ xxx xxxxxxx xxxxx.

```yaml
Type: X509Certificate
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertificateThumbprint
Xxxxxxxxx xxx xxxxxxx xxxxxx xxx xxxxxxxxxxx $X000$ xx x xxxx xxxxxxx xxxx xxx xxxxxxxxxx xx xxxx xxx xxxxxxx.
Xxxxx xxx xxxxxxxxxxx xxxxxxxxxx xx xxx xxxxxxxxxxx.

Xxxxxxxxxxxx xxx xxxx xx xxxxxx xxxxxxxxxxx$xxxxx xxxxxxxxxxxxxx.
Xxxx xxx xx xxxxxx xxxx xx xxxxx xxxx xxxxxxxx$ xxxx xx xxx xxxx xxxx xxxxxx xxxxxxxx.

Xx xxx x xxxxxxxxxxx xxxxxxxxxx$ xxx xxx Xxx$Xxxx xx Xxx$XxxxxXxxx xxxxxxx xx xxx Xxxxxxx XxxxxXxxxx Xxxx$ xxxxx.

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

### -ContentType
Xxxxxxxxx xxx xxxxxxx xxxx xx xxx xxx xxxxxxx.

Xx xxxx xxxxxxxxx xx xxxxxxx xxx xxx xxxxxxx xxxxxx xx XXXX$ Xxxxxx$XxxxXxxxxx xxxx xxx xxxxxxx xxxx xx $xxxxxxxxxxx$x$xxx$xxxx$xxxxxxxxxx$.
Xxxxxxxxx$ xxx xxxxxxx xxxx xx xxx xxxxxxxxx xx xxx xxxx.

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

### -Credential
Xxxxxxxxx x xxxx xxxxxxx xxxx xxx xxxxxxxxxx xx xxxx xxx xxxxxxx.
Xxx xxxxxxx xx xxx xxxxxxx xxxx.

Xxxx x xxxx xxxx$ xxxx xx $Xxxx00$ xx $Xxxxxx00$Xxxx00$$ xx xxxxx x XXXxxxxxxxxx xxxxxx$ xxxx xx xxx xxxxxxxxx xx xxx Xxx$Xxxxxxxxxx xxxxxx.

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

### -DisableKeepAlive
Xxxx xxx XxxxXxxxx xxxxx xx xxx XXXX xxxxxx xx Xxxxx.
Xx xxxxxxx$ XxxxXxxxx xx Xxxx.
XxxxXxxxx xxxxxxxxxxx x xxxxxxxxxx xxxxxxxxxx xx xxx xxxxxx xx xxxxxxxxxx xxxxxxxxxx xxxxxxxx.

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

### -Headers
Xxxxxxxxx xxx xxxxxxx xx xxx xxx xxxxxxx.
Xxxxx x xxxx xxxxx xx xxxxxxxxxx.

Xx xxx XxxxXxxxx xxxxxxx$ xxx xxx XxxxXxxxx xxxxxxxxx.
Xxx xxxxxx xxx xxxx xxxxxxxxx xx xxxxxxx XxxxXxxxx xx xxxxxx xxxxxxx.

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

### -InFile
Xxxx xxx xxxxxxx xx xxx xxx xxxxxxx xxxx x xxxx.

Xxxxx x xxxx xxx xxxx xxxx.
Xx xxx xxxx xxx xxxx$ xxx xxxxxxx xx xxx xxxxxxx xxxxxxxx.

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

### -InformationAction
Xxx Xxxx xxxxxxxxx xxx xx xxxx xx xxxxxxx x xxxx xx xxxxx xxxxxxxxxx xx xxxxxxx xxx xxxxxxx xx xxx xxxxxxxx.

Xxxx xxx xxxxx xx x XXX xxxxxxx$ xxx xxx xxxx xx xx XXxxxxxxxxx $xxxxxxxxx$ x xxxx xxxxx$$ xxx xxxx xx xxxxx xx xxx XXX xx xxxxx xxxxxxxxxx.
Xxx xxxxx xxxxxxx xxxxx $xxxx xx XXXX$$ xxx xxxx xx xxx xx xxx xxxxx xx xxx xxxxxxx xxxx xx xxx xxxxxxxx xxxx$xxxxx xxxxxx.

Xxxx xxx xxxx xx x xxxx$ xx xx xx xxx xxxxxx xx xxxxxxx Xxxxxx$XxxXxxxxxx xxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxxxx xxxxxxx xx xxx xxxx xxxxxx.

Xxx xxxxxxx$

$x $ Xxxxxx$XxxXxxxxxx xxxx$$$xxxxxxx.xxx$xxxxx.xxxx $x.Xxxxx$$0$$.Xxxx $ $XxXxxx$ $x.Xxxxx$$0$$.Xxxxxxxx $ $XxXxxxxxxx$ Xxxxxx$XxxxXxxxxx xxxx$$$xxxxxxx.xxx$xxxxxxx.xxxx $Xxxx $x

- xx $

Xxxxxx$XxxxXxxxxx xxxx$$$xxxxxxx.xxx$xxxxxxx.xxxx $Xxxx $x.Xxxxx$$0\]

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
Xxx Xxxx xxxxxxxxx xxx xx xxxx xx xxxxxxx x xxxx xx xxxxx xxxxxxxxxx xx xxxxxxx xxx xxxxxxx xx xxx xxxxxxxx.

Xxxx xxx xxxxx xx x XXX xxxxxxx$ xxx xxx xxxx xx xx XXxxxxxxxxx $xxxxxxxxx$ x xxxx xxxxx$$ xxx xxxx xx xxxxx xx xxx XXX xx xxxxx xxxxxxxxxx.
Xxx xxxxx xxxxxxx xxxxx $xxxx xx XXXX$$ xxx xxxx xx xxx xx xxx xxxxx xx xxx xxxxxxx xxxx xx xxx xxxxxxxx xxxx$xxxxx xxxxxx.

Xxxx xxx xxxx xx x xxxx$ xx xx xx xxx xxxxxx xx xxxxxxx Xxxxxx$XxxXxxxxxx xxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxxxx xxxxxxx xx xxx xxxx xxxxxx.

Xxx xxxxxxx$

$x $ Xxxxxx$XxxXxxxxxx xxxx$$$xxxxxxx.xxx$xxxxx.xxxx $x.Xxxxx$$0$$.Xxxx $ $XxXxxx$ $x.Xxxxx$$0$$.Xxxxxxxx $ $XxXxxxxxxx$ Xxxxxx$XxxxXxxxxx xxxx$$$xxxxxxx.xxx$xxxxxxx.xxxx $Xxxx $x

- xx $

Xxxxxx$XxxxXxxxxx xxxx$$$xxxxxxx.xxx$xxxxxxx.xxxx $Xxxx $x.Xxxxx$$0\]

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

### -MaximumRedirection
Xxxxxxxxxx xxx xxxx xxxxx Xxxxxxx XxxxxXxxxx xxxxxxxxx x xxxxxxxxxx xx xx xxxxxxxxx Xxxxxxx Xxxxxxxx Xxxxxxxxxx $XXX$ xxxxxx xxx xxxxxxxxxx xxxxx.
Xxx xxxxxxx xxxxx xx 0.
X xxxxx xx 0 $xxxx$ xxxxxxxx xxx xxxxxxxxxxx.

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

### -Method
Xxxxxxxxx xxx xxxxxx xxxx xxx xxx xxx xxxxxxx.
Xxxxx xxxxxx xxx Xxxxxxx$ Xxxxxx$ Xxx$ Xxxx$ Xxxxx$ Xxxxxxx$ Xxxxx$ Xxxx$ Xxx$ xxx Xxxxx.

```yaml
Type: WebRequestMethod
Parameter Sets: (All)
Aliases: 
Accepted values: Default, Get, Head, Post, Put, Delete, Trace, Options, Merge, Patch

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutFile
Xxxxx xxx xxxxxxxx xxxx xx xxx xxxxxxxxx xxxxxx xxxx.
Xxxxx x xxxx xxx xxxx xxxx.
Xx xxx xxxx xxx xxxx$ xxx xxxxxxx xx xxx xxxxxxx xxxxxxxx.

Xx xxxxxxx$ Xxxxxx$XxxxXxxxxx xxxxxxx xxx xxxxxxx xx xxx xxxxxxxx.
Xx xxxx xxx xxxxxxx xx x xxxx xxx xx xxx xxxxxxxx$ xxx xxx Xxxxxxxx xxxxxxxxx.

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

### -PassThru
Xxxxxxx xxx xxxxxxx$ xx xxxxxxxx xx xxxxxxx xxxx xx x xxxx.
Xxxx xxxxxxxxx xx xxxxx xxxx xxxx xxx XxxXxxx xxxxxxxxx xx xxxx xxxx xx xxx xxxxxxx.

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

### -Proxy
Xxxx x xxxxx xxxxxx xxx xxx xxxxxxx$ xxxxxx xxxx xxxxxxxxxx xxxxxxxx xx xxx Xxxxxxxx xxxxxxxx.
Xxxxx xxx XXX xx x xxxxxxx xxxxx xxxxxx.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProxyCredential
Xxxxxxxxx x xxxx xxxxxxx xxxx xxx xxxxxxxxxx xx xxx xxx xxxxx xxxxxx xxxx xx xxxxxxxxx xx xxx Xxxxx xxxxxxxxx.
Xxx xxxxxxx xx xxx xxxxxxx xxxx.

Xxxx x xxxx xxxx$ xxxx xx $Xxxx00$ xx $Xxxxxx00$Xxxx00$$ xx xxxxx x XXXxxxxxxxxx xxxxxx$ xxxx xx xxx xxxxxxxxx xx xxx Xxx$Xxxxxxxxxx xxxxxx.

Xxxx xxxxxxxxx xx xxxxx xxxx xxxx xxx Xxxxx xxxxxxxxx xx xxxx xxxx xx xxx xxxxxxx.
Xxx xxxxxx xxx xxx XxxxxXxxxxxxxxx xxx XxxxxXxxXxxxxxxXxxxxxxxxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

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

### -ProxyUseDefaultCredentials
Xxxx xxx xxxxxxxxxxx xx xxx xxxxxxx xxxx xx xxxxxx xxx xxxxx xxxxxx xxxx xx xxxxxxxxx xx xxx Xxxxx xxxxxxxxx.

Xxxx xxxxxxxxx xx xxxxx xxxx xxxx xxx Xxxxx xxxxxxxxx xx xxxx xxxx xx xxx xxxxxxx.
Xxx xxxxxx xxx xxx XxxxxXxxxxxxxxx xxx XxxxxXxxXxxxxxxXxxxxxxxxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

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

### -SessionVariable
Xxxxxxx x xxx xxxxxxx xxxxxxx xxx xxxxx xx xx xxx xxxxx xx xxx xxxxxxxxx xxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxx xxx xxxxxx xxxx $$$ xxxxxx.

Xxxx xxx xxxxxxx x xxxxxxx xxxxxxxx$ Xxxxxx$XxxxXxxxxx xxxxxxx x xxx xxxxxxx xxxxxxx xxxxxx xxx xxxxxxx xx xx x xxxxxxxx xxxx xxx xxxxxxxxx xxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
Xxx xxx xxx xxx xxxxxxxx xx xxxx xxxxxxx xx xxxx xx xxx xxxxxxx xxxxxxxxx.

Xxxxxx x xxxxxx xxxxxxx$ xxx xxx xxxxxxx xxxxxxx xx xxx x xxxxxxxxxx xxxxxxxxxx.
Xx xx xx xxxxxx xxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxxxxx xxx xxx xxxxxxx$ xxxxxxxxx xxxxxxx$ xxxxxxxxxxx$ xxx xxxxxxx xxxxxxxxxxx xxxxx$ xxx xxx xxxx xxxxx xxxxxx.
Xxx xxx xxx xx xx xxxxx xxxxx xxx xxxx xxxxx xxx xxxxxxxx.

Xx xxx xxx xxx xxxxxxx xxxxxxx xx xxxxxxxxxx xxx xxxxxxxx$ xxxxxxx xxx xxxxxxx xxxxxxxx xx xxx xxxxx xx xxx XxxXxxxxxx xxxxxxxxx.
Xxxxxxx XxxxxXxxxx xxxx xxx xxxx xx xxx xxx xxxxxxx xxxxxxx xxxxxx xxxx xxxxxxxxxxxx xxx xxx xxxxxxxxxx.
Xx xxxxxxxx x xxxxx xx xxx xxx xxxxxxx xxxxxxx$ xxx x xxxxxx xxxxxxxxx$ xxxx xx XxxxXxxxx xx Xxxxxxxxxx.
Xxxxxxxxx xxxxxx xxxx xxxxxxxxxx xxxx xxxxxx xx xxx xxx xxxxxxx xxxxxxx.

Xxx xxxxxx xxx xxx XxxxxxxXxxxxxxx xxx XxxXxxxxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: SV

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeoutSec
Xxxxxxxxx xxx xxxx xxx xxxxxxx xxx xx xxxxxxx xxxxxx xx xxxxx xxx.
Xxxxx x xxxxx xx xxxxxxx.
Xxx xxxxxxx xxxxx$ 0$ xxxxxxxxx xx xxxxxxxxxx xxxx$xxx.

X Xxxxxx Xxxx Xxxxxx $XXX$ xxxxx xxx xxxx xx xx 00 xxxxxxx xx xxxxxx xx xxxx xxx.
Xx xxxx xxxxxxx xxxxxxxx x xxxx xxxx xxxx xxxxxxxx xxxxxxxxxx$ xxx xxx xxx XxxxxxxXxx xx x xxxxx xxxxxxx xxxx xxxx$ xxx xxxx xxxx 00 xxxxxxx$ xx xxx xxxx 00 xxxxxxx xx xxxx xxxxxx x XxxXxxxxxxxx xx xxxxxx$ xxx xxxx xxxxxxx xxxxx xxx.

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

### -TransferEncoding
Xxxxxxxxx x xxxxx xxx xxx xxxxxxxx$xxxxxxxx XXXX xxxxxxxx xxxxxx.
Xxxxx xxxxxx xxx Xxxxxxx$ Xxxxxxxx$ Xxxxxxx$ XXxx xxx Xxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: chunked, compress, deflate, gzip, identity

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Uri
Xxxxxxxxx xxx Xxxxxxx Xxxxxxxx Xxxxxxxxxx $XXX$ xx xxx Xxxxxxxx xxxxxxxx xx xxxxx xxx xxx xxxxxxx xx xxxx.
Xxxx xxxxxxxxx xxxxxxxx XXXX$ XXXXX$ XXX$ xxx XXXX xxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxx.
Xxx xxxxxxxxx xxxx $$Xxx$ xx xxxxxxxx.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UseDefaultCredentials
Xxxx xxx xxxxxxxxxxx xx xxx xxxxxxx xxxx xx xxxx xxx xxx xxxxxxx.

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

### -UserAgent
Xxxxxxxxx x xxxx xxxxx xxxxxx xxx xxx xxx xxxxxxx.

Xxx xxxxxxx xxxx xxxxx xx xxxxxxx xx $Xxxxxxx$0.0 $Xxxxxxx XX$ Xxxxxxx XX 0.0$ xx$XX$ XxxxxxxXxxxxXxxxx$0.0$ xxxx xxxxxx xxxxxxxxxx xxx xxxx xxxxxxxxx xxxxxx xxx xxxxxxxx.

Xx xxxx x xxxxxxx xxxx xxx xxxxxxxx xxxx xxxxx xxxxxx xxxx xx xxxx xx xxxx Xxxxxxxx xxxxxxxx$ xxx xxx xxxxxxxxxx xx xxx XXXxxxXxxxx xxxxx$ xxxx xx Xxxxxx$ XxxxXxx$ XxxxxxxxXxxxxxxx$ Xxxxx$ xxx Xxxxxx.

Xxx xxxxxxx$ xxx xxxxxxxxx xxxxxxx xxxx xxx xxxx xxxxx xxxxxx xxx Xxxxxxxx.

Xxxxxx$XxxXxxxxxx $Xxx xxxx$$$xxxxxxx.xxx$ $XxxxXxxxx $$$Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.XXXxxxXxxxx$$$$XxxxxxxxXxxxxxxx$

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

### -WebSession
Xxxxxxxxx x xxx xxxxxxx xxxxxxx.
Xxxxx xxx xxxxxxxx xxxx$ xxxxxxxxx xxx xxxxxx xxxx $$$.

Xx xxxxxxxx x xxxxx xx xxx xxx xxxxxxx xxxxxxx$ xxx x xxxxxx xxxxxxxxx$ xxxx xx XxxxXxxxx xx Xxxxxxxxxx.
Xxxxxxxxx xxxxxx xxxx xxxxxxxxxx xxxx xxxxxx xx xxx xxx xxxxxxx xxxxxxx.

Xxxxxx x xxxxxx xxxxxxx$ xxx xxx xxxxxxx xxxxxxx xx xxx x xxxxxxxxxx xxxxxxxxxx.
Xx xx xx xxxxxx xxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxxxxx xxx xxx xxxxxxx$ xxxxxxxxx xxxxxxx$ xxxxxxxxxxx$ xxx xxxxxxx xxxxxxxxxxx xxxxx$ xxx xxx xxxx xxxxx xxxxxx.
Xxx xxx xxx xx xx xxxxx xxxxx xxx xxxx xxxxx xxx xxxxxxxx.

Xx xxxxxx x xxx xxxxxxx xxxxxxx$ xxxxx x xxxxxxxx xxxx $xxxxxxx x xxxxxx xxxx$ xx xxx xxxxx xx xxx XxxxxxxXxxxxxxx xxxxxxxxx xx xx Xxxxxx$XxxxXxxxxx xxxxxxx.
Xxxxxx$XxxxXxxxxx xxxxxxx xxx xxxxxxx xxx xxxxx xx xx xxx xxxxxxxx.
Xx xxxxxxxxxx xxxxxxxx$ xxx xxx xxxxxxxx xx xxx xxxxx xx xxx XxxXxxxxxx xxxxxxxxx.

Xxx xxxxxx xxx xxx XxxxxxxXxxxxxxx xxx XxxXxxxxxx xxxxxxxxxx xx xxx xxxx xxxxxxx.

```yaml
Type: WebRequestSession
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UseBasicParsing
$$Xxxx XxxXxxxxXxxxxxx Xxxxxxxxxxx$$

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### System.Object
Xxx xxx xxxx xxx xxxx xx x xxx xxxxxxx xx Xxxxxx$Xxxx$Xxxxxx.

## XXXXXXX

### System.Xml.XmlDocument, Microsoft.PowerShell.Commands.HtmlWebResponseObject, System.String
Xxx xxxxxx xx xxx xxxxxx xxxxxxx xxxx xxx xxxxxx xx xxx xxxxxxx xxxx xx xxxxxxxxx.

### PSObject
Xx xxx xxxxxxx xxxxxxx XXXX xxxxxxx$ Xxxxxx$XxxxXxxxxx xxxxxxx x XXXxxxxx xxxx xxxxxxxxxx xxx xxxxxxx.

## XXXXX

## XXXXXXX XXXXX

[ConvertTo-Json]()

[ConvertFrom-Json]()

[Invoke-WebRequest]()

