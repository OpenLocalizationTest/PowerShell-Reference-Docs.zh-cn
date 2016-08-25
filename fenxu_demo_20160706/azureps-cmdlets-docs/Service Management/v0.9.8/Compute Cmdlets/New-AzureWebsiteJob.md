---
external help file: SMAzure_Compute.xml
online version: 498c1abd-298b-43e9-ac53-bc57054a5387
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# New-AzureWebsiteJob
## XXXXXXXX
Xxxxxxx xxx xxx xxx xxx x xxxxxxx

## XXXXXX

```
New-AzureWebsiteJob [[-Name] <String>] [-Slot <String>] -JobFile <String> -JobName <String> [-JobType]
```

## XXXXXXXXXXX
Xxxxxxx xxx xxx xxx xxx x xxxxxxx

## XXXXXXXX

### $$$$$$$$$$$$$$  Xxxxxx xxx xxx xxx xxx x xxxxxxx $$$$$$$$$$$$$$
```
C:\PS>New-AzureWebsiteJob -Name MyWebsite -JobName MyWebJob -JobType Continuous -JobFile job.bat
```

Xxxxxxx x xxxxxxxxxx xxx xx xxxx xxx.xxx xx xxxxxxx XxXxxxxxx

## XXXXXXXXXX

### -JobFile
Xxx xxx xxx xxxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobName
Xxx xxx xxx xxxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobType
Xxx xxx xxx xxxx.
Xxx xx $xxxxxxxxx$ xx $xxxxxxxxxx$

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Triggered, Continuous

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxx xxxx xx xxx Xxxxx xxxxxxx

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

### -Slot
Xxx xxxx xxxx xx xxx Xxxxx xxxxxxx

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

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[New-AzureWebsite](498c1abd-298b-43e9-ac53-bc57054a5387)

[Get-AzureWebsiteJob](5ef76b84-385f-419e-8aba-228d53ce2232)

[Remove-AzureWebsiteJob](e25091a2-2472-4674-978c-ec1522631bc1)

[Start-AzureWebsiteJob](33bc54a9-76a7-45cd-92d5-662e16354fa3)

[Stop-AzureWebsiteJob](9698753f-0bfc-4845-b74e-6c6bed38a430)


