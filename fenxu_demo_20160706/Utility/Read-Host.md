---
external help file: Microsoft.PowerShell.Commands.Utility.dll-Help.xml
online version: http://go.microsoft.com/fwlink/p/?linkid=294000
schema: 2.0.0
---

# Read-Host
## XXXXXXXX
Xxxxx x xxxx xx xxxxx xxxx xxx xxxxxxx.

## XXXXXX

```
Read-Host [[-Prompt] <Object>] [-AsSecureString] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## XXXXXXXXXXX
Xxx Xxxx$Xxxx xxxxxx xxxxx x xxxx xx xxxxx xxxx xxx xxxxxxx.
Xxx xxx xxx xx xx xxxxxx x xxxx xxx xxxxx.
Xxxxxxx xxx xxx xxxx xxx xxxxx xx x xxxxxx xxxxxx$ xxx xxx xxx xxxx xxxxxx xx xxxxxx xxxxx xxx xxxxxx xxxx$ xxxx xx xxxxxxxxx$ xx xxxx xx xxxxxx xxxx.

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$age = read-host "Please enter your age"
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxx $Xxxxxx xxxxx xxxx xxx$$ xx x xxxxxx.
Xxxx x xxxxx xx xxxxxxx xxx xxx Xxxxx xxx xx xxxxxxx$ xxx xxxxx xx xxxxxx xx xxx $xxx xxxxxxxx.

### $$$$$$$$$$$$$$$$$$$$$$$$$$ XXXXXXX 0 $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\>$pwd_secure_string = read-host "Enter a Password" -assecurestring
```

Xxxx xxxxxxx xxxxxxxx xxx xxxxxx $Xxxxx x Xxxxxxxx$$ xx x xxxxxx.
Xx x xxxxx xx xxxxx xxxxxxx$ xxxxxxxxx $$$ xxxxxx xx xxx xxxxxxx xx xxxxx xx xxx xxxxx.
Xxxx xxx Xxxxx xxx xx xxxxxxx$ xxx xxxxx xx xxxxxx xx x XxxxxxXxxxxx xxxxxx xx xxx $xxx$xxxxxx$xxxxxx xxxxxxxx.

## XXXXXXXXXX

### -AsSecureString
Xxxxxxxx xxxxxxxxx $$$ xx xxxxx xx xxx xxxxxxxxxx xxxx xxx xxxx xxxxx xx xxxxx.

Xxxx xxx xxx xxxx xxxxxxxxx$ xxx xxxxxx xx xxx Xxxx$Xxxx xxxxxx xx x XxxxxxXxxxxx xxxxxx $Xxxxxx.Xxxxxxxx.XxxxxxXxxxxx$.

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
Xxxx xxx xxx xxxx xxxxxxxxx$ xxx xxxxxx xx xxx Xxxx$Xxxx xxxxxx xx x XxxxxxXxxxxx xxxxxx $Xxxxxx.Xxxxxxxx.XxxxxxXxxxxx$.

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
Xxxx xxx xxx xxxx xxxxxxxxx$ xxx xxxxxx xx xxx Xxxx$Xxxx xxxxxx xx x XxxxxxXxxxxx xxxxxx $Xxxxxx.Xxxxxxxx.XxxxxxXxxxxx$.

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

### -Prompt
Xxxxxxxxx xxx xxxx xx xxx xxxxxx.
Xxxx x xxxxxx.
Xx xxx xxxxxx xxxxxxxx xxxxxx$ xxxxxxx xx xx xxxxxxxxx xxxxx.
Xxxxxxx XxxxxXxxxx xxxxxxx x xxxxx $$$ xx xxx xxxx xxxx xxx xxxxx.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

### None
Xxx xxxxxx xxxx xxxxx xx xxxx xxxxxx.

## XXXXXXX

### System.String or System.Security.SecureString
Xx xxx XxXxxxxxXxxxxx xxxxxxxxx xx xxxx$ Xxxx$Xxxx xxxxxxx x XxxxxxXxxxxx.
Xxxxxxxxx$ xx xxxxxxx x xxxxxx.

## XXXXX

## XXXXXXX XXXXX

[Clear-Host]()

[ConvertFrom-SecureString]()

[Get-Host]()

[Out-Host]()

[Write-Host]()

