---
external help file: RMAzure_Automation.xml
online version: ea09d4b6-ff25-4b91-b957-328222844689
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# New-AzureRMAutomationCredential
## XXXXXXXX
Xxxxxxx xx Xxxxxxxxxx xxxxxxxxxx.

## XXXXXX

```
New-AzureRMAutomationCredential [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-Name] <String> [-Value] <PSCredential> [-Description <String>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxxxxxxxx$$ xxxxxx xxxxxxx x xxxxxxxxxx xx x $$XXXxxxxxxxxx$$ xxxxxx xx xxxxx$0 Xxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxxxxxx
```
PS C:\>$User = "Contoso\PFuller"
PS C:\> $Password = ConvertTo-SecureString "Password" -AsPlainText -Force
PS C:\> $Credential = New-Object -TypeName System.Management.Automation.PSCredential -ArgumentList $User, $Password
PS C:\> New-AzureRmAutomationCredential -AutomationAccountName "Contoso17" -Name "ContosoCredential" -Value $Credential -ResourceGroupName "ResourceGroup01"
```

Xxx xxxxx xxxxxxx xxxxxxx x xxxx xxxx xx xxx $Xxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxxx x xxxxx xxxx xxxxxxxx xxxx x xxxxxx xxxxxx xx xxxxx xxx XxxxxxxXx$XxxxxxXxxxxx xxxxxx.
Xxx xxxxxxx xxxxxx xxxx xxxxxx xx xxx $Xxxxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxxxxxxxx xxxxx xx $Xxxx xxx $Xxxxxxxx$ xxx xxxx xxxxxx xx xx xxx $Xxxxxxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx xx Xxxxxxxxxx xxxxxxxxxx xxxxx XxxxxxxXxxxxxxxxx xxxx xxxx $Xxxxxxxxxx.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xx xxxxx xxxx xxxxxx xxxxxx xxx xxxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Description
Xxxxxxxxx x xxxxxxxxxxx xxx xxx xxxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx x xxxx xxx xxx xxxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Xxxxxxxxx x xxxxxxxxxxx xxx xxx xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxxxxx x xxxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Value
Xxxxxxxxx xxx xxxxxxxxxxx xx x $$XXXxxxxxxxxx$$ xxxxxx.

```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

### Microsoft.Azure.Commands.Automation.Model.CredentialInfo

## XXXXX

## XXXXXXX XXXXX

[Get-AzureRmAutomationCredential](ea09d4b6-ff25-4b91-b957-328222844689)

[Remove-AzureRmAutomationCredential](6a171b2b-1fdc-4642-a3d5-495b39fa7cff)

[Set-AzureRmAutomationCredential](f0f039fd-2b0b-4993-8408-471e0f7ad10b)


