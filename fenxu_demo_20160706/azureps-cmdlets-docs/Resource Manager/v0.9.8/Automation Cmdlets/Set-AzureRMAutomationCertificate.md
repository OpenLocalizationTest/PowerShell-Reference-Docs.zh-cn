---
external help file: RMAzure_Automation.xml
online version: 7e2d3105-ae14-40c6-a715-57d63c178cde
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Set-AzureRMAutomationCertificate
## XXXXXXXX
Xxxxxxxx xxx xxxxxxxxxxxxx xx xx Xxxxxxxxxx xxxxxxxxxxx.

## XXXXXX

```
Set-AzureRMAutomationCertificate [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-Name] <String> [-Description <String>] [-Exportable <Boolean]>] [-Password <SecureString>] [-Path <String>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxXxxxxxxxxxXxxxxxxxxxx$$ xxxxxx xxxxxxxx xxx xxxxxxxxxxxxx xx x xxxxxxxxxxx xx xxxxx$0 Xxxxxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxxxxxxx
```
PS C:\>$Password = ConvertTo-SecureString -String "Password" -AsPlainText -Force
PS C:\> Set-AzureAutomationCertificate -AutomationAccountName "Contos17" -Name "ContosoCertificate" -Path "./cert.pfx" -Password $Password -ResourceGroupName "ResourceGroup01"
```

Xxx xxxxx xxxxxxx xxxxxxxx x xxxxx xxxx xxxxxxxx xx xx x xxxxxx xxxxxx xx xxxxx xxx XxxxxxxXx$XxxxxxXxxxxx xxxxxx.
Xxx xxxxxxx xxxxxx xxxx xxxxxx xx xxx $Xxxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxxx x xxxxxxxxxxx xxxxx XxxxxxxXxxxxxxxxxx.
Xxx xxxxxxx xxxx xxx xxxxxxxx xxxxxx xx $Xxxxxxxx.
Xxx xxxxxxx xxxxxxxxx xxx xxxxxxx xxxx xxx xxx xxxx xx xxx xxxx xxxx xx xxxxxxx.

## XXXXXXXXXX

### -AutomationAccountName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxxxxx xxxxxxx xxx xxxxx xxxx xxxxxx xxxxxxxx x xxxxxxxxxxx.

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
Xxxxxxxxx x xxxxxxxxxxx xxx xxx xxxxxxxxxxx xxxx xxxx xxxxxx xxxxxxxx.

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

### -Exportable
Xxxxxxxxx xxxxxxx xxx xxxxxxxxxxx xxx xx xxxxxxxx.

```yaml
Type: Boolean]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxxxx xxxx xxxx xxxxxx xxxxxxxx.

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

### -Password
Xxxxxxxxx xxx xxxxxxxx xxx xxx xxxxxxxxxxx xxxx.

```yaml
Type: SecureString
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Path
Xxxxxxxxx xxx xxxx xx x xxxxxx xxxx xx xxxxxx.
Xxx xxxx xxx xx x .xxx xxxx xx x .xxx xxxx.

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

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx xxxxx xxx xxxxx xxxx xxxxxx xxxxxxxx x xxxxxxxxxxx.

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

## XXXXXX

## XXXXXXX

### Microsoft.Azure.Commands.Automation.Model.CertificateInfo

## XXXXX

## XXXXXXX XXXXX

[Get-AzureRmAutomationCertificate](7e2d3105-ae14-40c6-a715-57d63c178cde)

[New-AzureRmAutomationCertificate](4316d596-2954-42e8-905f-840853dab7d5)

[Remove-AzureRmAutomationCertificate](1ed3a0d7-541d-4a07-b0d6-4538f98450f7)


