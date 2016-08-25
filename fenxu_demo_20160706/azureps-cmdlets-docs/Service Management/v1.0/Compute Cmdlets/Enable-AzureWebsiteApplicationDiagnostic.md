---
external help file: SMAzure_Compute.xml
online version: http://go.microsoft.com/FWLink/p/?LinkID=311701
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Enable-AzureWebsiteApplicationDiagnostic
## XXXXXXXX
Xxxxxxx xxxxxxxxxxx xxxxxxxxxxx xx xx Xxxxx xxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Enable-AzureWebsiteApplicationDiagnostic [[-Name] <String>] [-PassThru] [-Slot <String>] [-File] [-LogLevel]
```

### UNNAMED_PARAMETER_SET_2
```
Enable-AzureWebsiteApplicationDiagnostic [[-Name] <String>] [-PassThru] [-Slot <String>]
 [-StorageAccountName <String>] [-LogLevel] [-Storage]
```

## XXXXXXXXXXX
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.00 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $Xxx$Xxxxxx $Xxxx Xxxxx$.Xxxxxxx.

Xxxxxxx xxxxxxxxxxx xxxxxxxxxxx xx xx Xxxxx xxxxxxx$ xxx xxxxxx xxx xx xxxxxxxxx xxxxxxx xx xxxx xx x xxxx xxxxxx xx xx Xxxxx xxxxxxx.

## XXXXXXXX

### 0$ Xxxxxx xxxxxxxxxxx xxxxx xxxx xxxxxx
```
C:\PS>Enable-AzureWebsiteApplicationDiagnostic -Name MyWebsite -File -LogLevel Verbose
```

Xxxx xxxxxxx xxxxxxx xxxxxxxxxxx xxxxxxx xx xxxx xxxxxx xxxx xxxxxxx xxxxx.

### 0$ Xxxxxx xxxxxxx xxxxx Xxxxx Xxxxxxx
```
C:\PS>Enable-AzureWebsiteApplicationDiagnostic -Name MyWebsite -Storage -LogLevel Information -StorageAccountName myaccount
```

Xxxx xxxxxxx xxxxxxx xxxxxxxxxxx xxxxxxx xxxxx xxxxxxx xxxxxxx xxxxx $$$xxxxxxxxx$$$ xxxx xxxxxxx xxxxx xxx xx $$$xxxxxxxxxxx$$$.

## XXXXXXXXXX

### -File
Xxxxxxxxx xxxx xxx xxxx xx xxx x xxxx xxxxxx xx xxxxx xxx xxx xxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -LogLevel
Xxx xxx xxxxx xx xxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Error, Warning, Information, Verbose

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Xxx xxxx xx xxx Xxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
Xxxx xx xxxxxx xxxx xx xxx xxxxxxx xxxxxxxx.

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

### -Slot
Xxxxxxxxx xxx xxxx xx xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Storage
Xxxxxxxxx xxxx xxx xxxx xx xxx Xxxxx xx xxxxx xxx xxx xxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -StorageAccountName
Xxx xxxxxxx xxxxxxx xx xxx xxx xxxxxxx xxx xxxx.
Xx xxx xxxxxxxxx$ xxx XxxxxxxXxxxxxxXxxxxxx xx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Disable-AzureWebsiteApplicationDiagnostic](40b3665f-ec67-4ee7-9349-d16c0b2e2495)

[Get-AzureWebsite](0c2a5092-db45-4ce7-b39b-d1e499b4a867)

[New-AzureWebsite](498c1abd-298b-43e9-ac53-bc57054a5387)

[Remove-AzureWebsite](3997c3b8-37ce-4135-a17d-63ae3bdd8e74)

[Start-AzureWebsite](d6ee400f-4a92-4f2f-83bb-70188bb2000d)


