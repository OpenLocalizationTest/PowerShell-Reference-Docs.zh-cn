---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=293988
schema: 2.0.0
---

# Xxxxxx$XxxXxxxxxx
## XXXXXXXX
Xxxx xxxxxxx xxxx x xxx xxxx xx xxx Xxxxxxxx.

## XXXXXX

```
Invoke-WebRequest [-UseBasicParsing] [-Uri] <Uri> [-WebSession <WebRequestSession>] [-SessionVariable <String>]
 [-Credential <PSCredential>] [-UseDefaultCredentials] [-CertificateThumbprint <String>]
 [-Certificate <X509Certificate>] [-UserAgent <String>] [-DisableKeepAlive] [-TimeoutSec <Int32>]
 [-Headers <IDictionary>] [-MaximumRedirection <Int32>] [-Method <WebRequestMethod>] [-Proxy <Uri>]
 [-ProxyCredential <PSCredential>] [-ProxyUseDefaultCredentials] [-Body <Object>] [-ContentType <String>]
 [-TransferEncoding <String>] [-InFile <String>] [-OutFile <String>] [-PassThru]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxxxx$XxxXxxxxxx xxxxxx xxxxx XXXX$ XXXXX$ XXX$ xxx XXXX xxxxxxxx xx x xxx xxxx xx xxx xxxxxxx.
Xx xxxxxx xxx xxxxxxxx xxx xxxxxxx xxxxxxxxxxx xx xxxxx$ xxxxx$ xxxxxx$ xxx xxxxx xxxxxxxxxxx XXXX xxxxxxxx.

Xxxx xxxxxx xxx xxxxxxxxxx xx Xxxxxxx XxxxxXxxxx 0.0.

## XXXXXXXX

### Xxxxxxx 0
```
PS C:\>$r = Invoke-WebRequest -URI http://www.bing.com?q=how+many+feet+in+a+mile
PS C:\>$r.AllElements | where {$_.innerhtml -like "*=*"} | Sort { $_.InnerHtml.Length } | Select InnerText -First 5
innerText---------1 =5280 feet1 mile
```

Xxxx xxxxxxx xxxx xxx Xxxxxx$XxxXxxxxxx xxxxxx xx xxxx x xxx xxxxxxx xx xxx Xxxx.xxx xxxx.

Xxx xxxxx xxxxxxx xxxxxx xxx xxxxxxx xxx xxxxx xxx xxxxxxxx xx xxx $x xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx XxxxxXxxx xxxxxxxx xxxx xx xxxxxxxx xx xxxxx xxxx$ xxxxx xxx xxxxx XXXX xx xxxxxx xxx xxxxxxx xxx 0 xxxxxxxx xxxxxx.
Xxxxxxx xx xxx xxxxxxxx XXXX xxxxx xxxxx xxxxx xxx xxxx xxx xxxx xxxxxxxx xxxxxxx xxxx xxxxxxx xxxx xxxx.

### Xxxxxxx 0
```
The first command uses the Invoke-WebRequest cmdlet to send a sign-in request. The command specifies a value of "fb" for the value of the SessionVariable parameter, and saves the result in the $r variable.When the command completes, the $r variable contains an HtmlWebResponseObject and the $fb variable contains a WebRequestSession object.
PS C:\>$r=Invoke-WebRequest http://www.facebook.com/login.php -SessionVariable fb

The second command shows the WebRequestSession object in the $fb variable.
PS C:\>$fb

The third command gets the first form in the Forms property of the HTTP response object in the $r variable, and saves it in the $form variable.
PS C:\>$form = $r.Forms[0]

The fourth command pipes the properties of the form in the $form variable into a list by using the Format-List cmdlet.
PS C:\>$form | Format-List

The fifth command displays the keys and values in the hash table (dictionary) object in the Fields property of the form.
PS C:\>$form.fields

The sixth and seventh commands populate the values of the "email" and "pass" keys of the hash table in the Fields property of the form. You can replace the email and password with values that you want to use.
PS C:\>$form.Fields["email"]="User01@Fabrikam.com"
$form.Fields["pass"]="P@ssw0rd"

The eighth command uses the Invoke-WebRequest cmdlet to sign into the Facebook web service.The value of the Uri parameter is the value of the Action property of the form. The WebRequestSession object in the $fb variable (the session variable specified in the first command) is now the value of the WebSession parameter. The value of the Body parameter is the hash table in the Fields property of the form and the value of the Method parameter is POST. The command saves the output in the $r variable.
PS C:\>$r=Invoke-WebRequest -Uri ("https://www.facebook.com" + $form.Action) -WebSession $fb -Method POST -Body $form.Fields

The full script, then, is as follows.
PS C:\># Sends a sign-in request by running the Invoke-WebRequest cmdlet. The command specifies a value of "fb" for the SessionVariable parameter, and saves the results in the $r variable.

$r=Invoke-WebRequest http://www.facebook.com/login.php -SessionVariable fb

# Use the session variable that you created in Example 1. Output displays values for Headers, Cookies, Credentials, etc. 

$fb

# Gets the first form in the Forms property of the HTTP response object in the $r variable, and saves it in the $form variable. 

$form = $r.Forms[0]

# Pipes the form properties that are stored in the $forms variable into the Format-List cmdlet, to display those properties in a list. 

$form | Format-List

# Displays the keys and values in the hash table (dictionary) object in the Fields property of the form.

$form.fields

# The next two commands populate the values of the "email" and "pass" keys of the hash table in the Fields property of the form. Of course, you can replace the email and password with values that you want to use. 

$form.Fields["email"] = "User01@Fabrikam.com"
$form.Fields["pass"] = "P@ssw0rd"

# The final command uses the Invoke-WebRequest cmdlet to sign in to the Facebook web service. 

$r=Invoke-WebRequest -Uri ("https://www.facebook.com" + $form.Action) -WebSession $fb -Method POST -Body $form.Fields

When the command finishes, the StatusDescription property of the web response object in the $r variable indicates that the user is signed in successfully.
PS C:\>$r.StatusDescription
```

Xxxx xxxxxxx xxxxx xxx xx xxx xxx Xxxxxx$XxxXxxxxxx xxxxxx xxxx x xxxxxxxx xxx xxxxxxx$ xxxx xx Xxxxxxxx.

### Xxxxxxx 0
```
PS C:\>(Invoke-WebRequest -Uri "http://msdn.microsoft.com/en-us/library/aa973757(v=vs.85).aspx").Links.Href
```

Xxxx xxxxxxx xxxx xxx xxxxx xx x xxx xxxx.
Xx xxxx xxx Xxxxxx$XxxXxxxxxx xxxxxx xx xxx xxx xxx xxxx xxxxxxx.
Xxxx xx xxxxx xxx Xxxxx xxxxxxxx xx xxx XxxxXxxXxxxxxxxXxxxxx xxxx Xxxxxx$XxxXxxxxxx xxxxxxx$ xxx xxx Xxxx xxxxxxxx xx xxxx xxxx.

## XXXXXXXXXX

### $Xxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxx.
Xxx xxxx xx xxx xxxxxxx xx xxx xxxxxxx xxxx xxxxxxx xxx xxxxxxx.
Xxx xxx xxxx xxxx x xxxx xxxxx xx Xxxxxx$XxxXxxxxxx.

Xxx Xxxx xxxxxxxxx xxx xx xxxx xx xxxxxxx x xxxx xx xxxxx xxxxxxxxxx xx xxxxxxx xxx xxxxxxx xx xxx xxxxxxxx.

Xxxx xxx xxxxx xx x XXX xxxxxxx xxx xxx xxxx xx xx XXxxxxxxxxx $xxxxxxxxx$ x xxxx xxxxx$$ xxx xxxx xx xxxxx xx xxx XXX xx xxxxx xxxxxxxxxx.
Xxx xxxxx XXX xxxxxxxx$ xxx xxxx xx xxx xx xxx xxxxx xx xxx xxxxxxx xxxx xx xxx xxxxxxxx xxxx$xxxxx xxxxxx.

Xxxx xxx xxxx xx x xxxx$ xx xx xx xxx xxxxxx xx xx Xxxxxx$XxxXxxxxxx xxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxxxx xxxxxxx xx xxx xxxx xxxxxx.

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

### $Xxxxxxxxxxx
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

### $XxxxxxxxxxxXxxxxxxxxx
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

### $XxxxxxxXxxx
Xxxxxxxxx xxx xxxxxxx xxxx xx xxx xxx xxxxxxx.

Xx xxxx xxxxxxxxx xx xxxxxxx xxx xxx xxxxxxx xxxxxx xx XXXX$ Xxxxxx$XxxXxxxxxx xxxx xxx xxxxxxx xxxx xx $xxxxxxxxxxx$x$xxx$xxxx$xxxxxxxxxx$.
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

### $Xxxxxxxxxx
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

### $XxxxxxxXxxxXxxxx
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

### $Xxxxxxx
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

### $XxXxxx
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

### $XxxxxxxxxxxXxxxxx
Xxx Xxxx xxxxxxxxx xxx xx xxxx xx xxxxxxx x xxxx xx xxxxx xxxxxxxxxx xx xxxxxxx xxx xxxxxxx xx xxx xxxxxxxx.

Xxxx xxx xxxxx xx x XXX xxxxxxx xxx xxx xxxx xx xx XXxxxxxxxxx $xxxxxxxxx$ x xxxx xxxxx$$ xxx xxxx xx xxxxx xx xxx XXX xx xxxxx xxxxxxxxxx.
Xxx xxxxx XXX xxxxxxxx$ xxx xxxx xx xxx xx xxx xxxxx xx xxx xxxxxxx xxxx xx xxx xxxxxxxx xxxx$xxxxx xxxxxx.

Xxxx xxx xxxx xx x xxxx$ xx xx xx xxx xxxxxx xx xx Xxxxxx$XxxXxxxxxx xxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxxxx xxxxxxx xx xxx xxxx xxxxxx.

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

### $XxxxxxxxxxxXxxxxxxx
Xxx Xxxx xxxxxxxxx xxx xx xxxx xx xxxxxxx x xxxx xx xxxxx xxxxxxxxxx xx xxxxxxx xxx xxxxxxx xx xxx xxxxxxxx.

Xxxx xxx xxxxx xx x XXX xxxxxxx xxx xxx xxxx xx xx XXxxxxxxxxx $xxxxxxxxx$ x xxxx xxxxx$$ xxx xxxx xx xxxxx xx xxx XXX xx xxxxx xxxxxxxxxx.
Xxx xxxxx XXX xxxxxxxx$ xxx xxxx xx xxx xx xxx xxxxx xx xxx xxxxxxx xxxx xx xxx xxxxxxxx xxxx$xxxxx xxxxxx.

Xxxx xxx xxxx xx x xxxx$ xx xx xx xxx xxxxxx xx xx Xxxxxx$XxxXxxxxxx xxxx$ Xxxxxxx XxxxxXxxxx xxxx xxx xxxxxxx xxxxxxx xx xxx xxxx xxxxxx.

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

### $XxxxxxxXxxxxxxxxxx
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

### $Xxxxxx
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

### $XxxXxxx
Xxxxx xxx xxxxxxxx xxxx xx xxx xxxxxxxxx xxxxxx xxxx.
Xxxxx x xxxx xxx xxxx xxxx.
Xx xxx xxxx xxx xxxx$ xxx xxxxxxx xx xxx xxxxxxx xxxxxxxx.

Xx xxxxxxx$ Xxxxxx$XxxXxxxxxx xxxxxxx xxx xxxxxxx xx xxx xxxxxxxx.
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

### $XxxxXxxx
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

### $Xxxxx
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

### $XxxxxXxxxxxxxxx
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

### $XxxxxXxxXxxxxxxXxxxxxxxxxx
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

### $XxxxxxxXxxxxxxx
Xxxxxxx x xxx xxxxxxx xxxxxxx xxx xxxxx xx xx xxx xxxxx xx xxx xxxxxxxxx xxxxxxxx.
Xxxxx x xxxxxxxx xxxx xxxxxxx xxx xxxxxx xxxx $$$ xxxxxx.

Xxxx xxx xxxxxxx x xxxxxxx xxxxxxxx$ Xxxxxx$XxxXxxxxxx xxxxxxx x xxx xxxxxxx xxxxxxx xxxxxx xxx xxxxxxx xx xx x xxxxxxxx xxxx xxx xxxxxxxxx xxxx xx xxxx Xxxxxxx XxxxxXxxxx xxxxxxx.
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

### $XxxxxxxXxx
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

### $XxxxxxxxXxxxxxxx
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

### $Xxx
Xxxxxxxxx xxx Xxxxxxx Xxxxxxxx Xxxxxxxxxx $XXX$ xx xxx Xxxxxxxx xxxxxxxx xx xxxxx xxx xxx xxxxxxx xx xxxx.
Xxxxx x XXX.
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

### $XxxXxxxxXxxxxxx
Xxxx xxx xxxxxxxx xxxxxx xxx XXXX xxxxxxx xxxxxxx Xxxxxxxx Xxxxxx Xxxxx $XXX$ xxxxxxx.

Xxxx xxxxxxxxx xx xxxxxxxx xxxx Xxxxxxxx Xxxxxxxx xx xxx xxxxxxxxx xx xxx xxxxxxxxx$ xxxx xx xx x Xxxxxx Xxxx xxxxxxxxxxxx xx x Xxxxxxx Xxxxxx xxxxxxxxx xxxxxx.

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

### $XxxXxxxxxxXxxxxxxxxxx
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

### $XxxxXxxxx
Xxxxxxxxx x xxxx xxxxx xxxxxx xxx xxx xxx xxxxxxx.

Xxx xxxxxxx xxxx xxxxx xx xxxxxxx xx $Xxxxxxx$0.0 $Xxxxxxx XX$ Xxxxxxx XX 0.0$ xx$XX$ XxxxxxxXxxxxXxxxx$0.0$ xxxx xxxxxx xxxxxxxxxx xxx xxxx xxxxxxxxx xxxxxx xxx xxxxxxxx.

Xx xxxx x xxxxxxx xxxx xxx xxxxxxxx xxxx xxxxx xxxxxx xxxx xx xxxx xx xxxx Xxxxxxxx xxxxxxxx$ xxx xxx xxxxxxxxxx xx xxx XXXxxxXxxxx xxxxx$ xxxx xx Xxxxxx$ XxxxXxx$ XxxxxxxxXxxxxxxx$ Xxxxx$ xxx Xxxxxx.

Xxx xxxxxxx$ xxx xxxxxxxxx xxxxxxx xxxx xxx xxxx xxxxx xxxxxx xxx Xxxxxxxx

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

### $XxxXxxxxxx
Xxxxxxxxx x xxx xxxxxxx xxxxxxx.
Xxxxx xxx xxxxxxxx xxxx$ xxxxxxxxx xxx xxxxxx xxxx $$$.

Xx xxxxxxxx x xxxxx xx xxx xxx xxxxxxx xxxxxxx$ xxx x xxxxxx xxxxxxxxx$ xxxx xx XxxxXxxxx xx Xxxxxxxxxx.
Xxxxxxxxx xxxxxx xxxx xxxxxxxxxx xxxx xxxxxx xx xxx xxx xxxxxxx xxxxxxx.

Xxxxxx x xxxxxx xxxxxxx$ xxx xxx xxxxxxx xxxxxxx xx xxx x xxxxxxxxxx xxxxxxxxxx.
Xx xx xx xxxxxx xxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxxxxx xxx xxx xxxxxxx$ xxxxxxxxx xxxxxxx$ xxxxxxxxxxx$ xxx xxxxxxx xxxxxxxxxxx xxxxx$ xxx xxx xxxx xxxxx xxxxxx.
Xxx xxx xxx xx xx xxxxx xxxxx xxx xxxx xxxxx xxx xxxxxxxx.

Xx xxxxxx x xxx xxxxxxx xxxxxxx$ xxxxx x xxxxxxxx xxxx $xxxxxxx x xxxxxx xxxx$ xx xxx xxxxx xx xxx XxxxxxxXxxxxxxx xxxxxxxxx xx xx Xxxxxx$XxxXxxxxxx xxxxxxx.
Xxxxxx$XxxXxxxxxx xxxxxxx xxx xxxxxxx xxx xxxxx xx xx xxx xxxxxxxx.
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

## XXXXXX

### Xxxxxx.Xxxxxx
Xxx xxx xxxx xxx xxxx xx x xxx xxxxxxx xx Xxxxxx$XxxXxxxxxx

## XXXXXXX

### Xxxxxxxxx.XxxxxXxxxx.Xxxxxxxx.XxxxXxxXxxxxxxxXxxxxx

## XXXXX

## XXXXXXX XXXXX

[Xxxxxx$XxxxXxxxxx]()

[XxxxxxxXxxx$Xxxx]()

[XxxxxxxXx$Xxxx]()

