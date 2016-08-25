---
external help file: SMAzure_Compute.xml
online version: 
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Get-AzureWebsite
## XXXXXXXX
Xxxx Xxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxxxxxxx.

## XXXXXX

```
Get-AzureWebsite [[-Name] <String>] [-Slot <String>]
```

## XXXXXXXXXXX
Xxx Xxx$XxxxxXxxxxxx xxxxxx xxxx xxxxxxxxxxx xxxxx Xxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxxxxxxx.

Xx xxxxxxx$ Xxx$XxxxxXxxxxxx xxxx xxx Xxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxxxxxxx xxx xxxxxxx xx xxxxxx xxxx xxxxxxxx xxxxx xxxxxxxxxxx xxxxx xxx xxxxx.
Xxxx xxx xxx xxx Xxxx xxxxxxxxx$ Xxx$XxxxxXxxxxxx xxxxxxx xx xxxxxx xxxx xxxxxxxxx xxxxxxxxxxx$ xxxxxxxxx xxxxxxxxxxxxx xxxxxxx.

Xxx xxxxxxx xxxxxxxxxxxx xx xxx xxxxxxxxxxxx xxxx xx xxxxxxxxxx xx $xxxxxxx.$ Xx xxxx xxx xxxxxxx xxxxxxxxxxxx$ xxx xxx Xxxxxxx xxxxxxxxx xx xxx Xxx$XxxxxXxxxxxxxxxxxxxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000 xxxxxx.
Xx xxxxxx xxx xxxxxxx xxxxxxxxxxxx$ xxx xxx Xxxxxx$XxxxxXxxxxxxxxxxxxxxx$$$xx.xxxxxxxxx.xxx$xxxxxx$$XxxxXX$000000 xxxxxx.

Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.00 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $Xxx$Xxxxxx $Xxxx Xxxxx$.Xxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxx xxx xxxxxxxx xx xxx xxxxxxxxxxxx
```
PS C:\>Get-AzureWebsite
```

Xxxx xxxxxxx xxxx xxx Xxxxx xxxxxxxx xx xxx xxxxxxx xxxxxxxxxxxx.

### Xxxxxxx 0$ Xxx x xxxxxxx xx xxxx
```
PS C:\>Get-AzureWebsite -Name ContosoWeb
```

Xxxx xxxxxxx xxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx XxxxxxxXxx Xxxxx xxxxxxx$ xxxxxxxxx xxxxxxxxxxxxx xxxxxxxxxxx.
Xxxx xxx xxx xxx Xxxx xxxxxxxxx$ Xxx$XxxxxXxxxxxx xxxxxxx x XxxxXxxxXxxxxx xxxxxx xxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxx.

### Xxxxxxx 0$ Xxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxxx
```
PS C:\>Get-AzureWebsite | ForEach-Object {Get-AzureWebsite -Name $_.Name}
```

Xxxx xxxxxxx xxxx xxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxxx xx xxx xxxxxxxxxxxx.
Xx xxxx x Xxx$XxxxxXxxxxxx xxxxxxx xx xxx xxx xxxxxxxx xxx xxxx xxxx xxx XxxXxxx$Xxxxxx xxxxxx xx xxx xxxx xxxxxxx xx xxxx.

### Xxxxxxx 0$ Xxx xxxxxxxxxxx xxxxx x xxxxxxxxxx xxxx
```
PS C:\>Get-AzureWebsite -Name ContosoWeb -Slot Staging
```

Xxxx xxxxxxx xxxx xxx Xxxxxxx xxxxxxxxxx xxxx xx xxx XxxxxxxXxx xxxxxxx.
Xxxxxxxxxx xxxxx xxx xxx xxxx xxxxxxxxx xxxxxxxx xx xxxx Xxxxx xxxxxxx xxxxxxx xxxxxxxxx xxxx xx xxx xxxxxx.

### Xxxxxxx 0$ Xxx xxxxxxx xxxxxxxxx
```
PS C:\>(Get-AzureWebsite -Name ContosoWeb).Instances

InstanceId
----------
2d8e712fb8f85d061c30fd793a534e6700a175f9a9ab12ca55cb3b0edfcc10ee
5834916b8cef49249b18187708223a33fbbc4352d33b48369f3166644bdd3445

PS C:\>(Get-AzureWebsite -Name ContosoWeb).Instances.Count
2
```

Xxx xxxxxxxx xx xxxx xxxxxxx xxx xxx Xxxxxxxxx xxxxxxxx xx xx Xxxxx xxxxxxx xx xxx xxxxxxxxxxx xxxxx xxxxxxxxx xxxxxxx xxxxxxx xxxxxxxxx.
Xxx Xxxxxxxxx xxxxxxxx xxx xxxxx xx xxx XxxxXxxxXxxxxx xxxxxx xx xxxxxxx 0.0.0 xx xxx Xxxxx xxxxxx.

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxxx XXx xx xxx xxxxxxxxx xxxxxxx xxxxxxxxx xx x xxxxxxx.
Xxx xxxxxx xxxxxxx xxxx xxx xxxxxx xx xxxxxxx xxxxxxxxx xx xxx xxxxxxx.
$Xxx xxx xxx xxx Xxxxx xxxxxxxx xx xxx xxxxx.$

## XXXXXXXXXX

### -Name
Xxxx xxxxxxxx xxxxxxxxxxxxx xxxxxxxxxxx xxxxx xxx xxxxxxxxx xxxxxxx.
Xxxxx xxx xxxx xx xxx xxxxxxx xx xxx xxxxxxxxxxxx.
Xx xxxxxxx$ Xxx$XxxxxXxxxxxx xxxx xxx xxxxxxxx xx xxx xxxxxxx xxxxxxxxxxxx.
Xxx Xxxx xxxxx xxxx xxx xxxxxxx xxxxxxxx xxxxxxxxxx.

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
Xxxx xxx xxxxxxxxx xxxxxxxxxx xxxx xx xxx xxxxxxx.
Xxxxx xxx xxxx xxxx$ xxxx xx $Xxxxxxx$ xx $Xxxxxxxxxx$.
Xxx xxxx xxxxxxxxxxx xxxxx xxxxxxxxxx xxxxx$ xxx Xxxxxx Xxxxxxxxxx xx Xxxxxxxxx Xxxxx Xxx Xxxxxxxxx$$$xxxxx.xxxxxxxxx.xxx$xx$xx$xxxxxxxxxxxxx$xxxxxxxx$xxx$xxxxx$xxxxxx$xxxxxxxxxx$.
Xx xxx x xxxxxxxxxx xxxx xx xx xxxxxxxx Xxxxx xxxxxxx$ xxx xxx Xxx$XxxxxXxxxxxx xxxxxx.

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

### None
Xxx xxx xxxx xxxxx xx xxxx xxxxxx xx xxxxxxxx xxxx$ xxx xxx xx xxxxx.

## XXXXXXX

### Microsoft.WindowsAzure.Commands.Utilities.Websites.Services.WebEntities.Site
Xx xxxxxxx$ Xxx$XxxxxXxxxxxx xxxxxxx xx xxxxx xx Xxxx xxxxxxx.

### Microsoft.WindowsAzure.Commands.Utilities.Websites.Services.WebEntities.SiteWithConfig
Xxxx xxx xxx xxx Xxxx xxxxxxxxx$ Xxx$XxxxxXxxxxxx xxxxxxx x XxxxXxxxXxxxxx xxxxxx.

## XXXXX

## XXXXXXX XXXXX

[New-AzureWebsite](498c1abd-298b-43e9-ac53-bc57054a5387)

[Remove-AzureWebsite](3997c3b8-37ce-4135-a17d-63ae3bdd8e74)

[Start-AzureWebsite](d6ee400f-4a92-4f2f-83bb-70188bb2000d)

[Stop-AzureWebsite](62c5de93-e58b-4e57-85d0-8b7e75df1f31)

[Show-AzureWebsite](3b828275-d62a-4c04-9767-15d6f743557c)


