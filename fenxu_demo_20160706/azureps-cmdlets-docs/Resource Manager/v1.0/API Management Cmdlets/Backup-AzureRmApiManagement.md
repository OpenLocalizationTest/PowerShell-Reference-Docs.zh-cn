---
external help file: RMAzure_Apimanagement.xml
online version: e067ded3-a2e3-4d53-8628-0ebbafa62721
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Backup-AzureRmApiManagement
## XXXXXXXX
Xxxxx xx xx XXX Xxxxxxxxxx xxxxxxx.

## XXXXXX

```
Backup-AzureRmApiManagement [-PassThru] [-TargetBlobName <String>] -Name <String> -ResourceGroupName <String>
 -StorageContext <AzureStorageContext> -TargetContainerName <String>
```

## XXXXXXXXXXX
Xxx $$Xxxxxx$XxxxxXxXxxXxxxxxxxxx$$ xxxxxx xxxxx xx xx xxxxxxxx xx xx xxxxx$0 XXX Xxxxxxxxxx xxxxxxx.
Xxxx xxxxxx xxxxxx xxx xxxxxx xx xx xxxxx$0 Xxxxxxx xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxx xx xx XXX Xxxxxxxxxx xxxxxxx
```
PS C:\>Backup-AzureRmApiManagement -ResourceGroupName "ContosoGroup02" -Name "ContosoApi" -StorageContext $StorageContext -TargetContainerName "ContosoBackups" -TargetBlobName "ContosoBackup.apimbackup"
```

Xxxx xxxxxxx xxxxx xx xx XXX Xxxxxxxxxx xxxxxxx xx x Xxxxxxx xxxx.

## XXXXXXXXXX

### -Name
Xxxxxxxxx xxx xxxx xx xxx XXX Xxxxxxxxxx xxxxxxxxxx xxxx xxxx xxxxxx xxxxx xx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx xxx xxxxxx xx $$XxXxxXxxxxxxxxx$$ xxxxxx$ xx xxx xxxxxxxxx xxxxxxxx.

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

### -ResourceGroupName
Xxxxxxxxx xxx xxxx xx xxx xx xxxxxxxx xxxxx xxxxx xxxxx xxx XXX Xxxxxxxxxx xxxxxxxxxx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -StorageContext
Xxxxxxxxx x xxxxxxx xxxxxxxxxx xxxxxxx.

```yaml
Type: AzureStorageContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -TargetBlobName
Xxxxxxxxx xxx xxxx xx xxx xxxx xxx xxx xxxxxx.
Xx xxx xxxx xxxx xxx xxxxx$ xxxx xxxxxx xxxxxxx xx.
Xxxx xxxxxx xxxxxxxxx x xxxxxxx xxxxx xxxxx xx xxx xxxxxxxxx xxxxxxx$ 

$Xxxx$$$xxxx$XX$xx$XX$xx$.xxxxxxxxxx

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

### -TargetContainerName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxx xx xxx xxxx xxx xxx xxxxxx.
Xx xxx xxxxxxxxx xxxx xxx xxxxx$ xxxx xxxxxx xxxxxxx xx.

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

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-AzureRmApiManagement](e067ded3-a2e3-4d53-8628-0ebbafa62721)

[New-AzureRmApiManagement](6b5595ca-246e-4381-a37e-24dfae307109)

[Remove-AzureRmApiManagement](9a2c4617-9870-4d9c-92fa-2af03211d931)

[Restore-AzureRmApiManagement](b0ff412d-269a-472f-8d79-9c0b9f0ebac2)


