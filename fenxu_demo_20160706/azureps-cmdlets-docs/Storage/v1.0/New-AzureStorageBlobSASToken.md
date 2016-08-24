---
external help file: RMAzure_Storage.xml
online version: 74bc4494-be41-4493-9939-e51e61dd09e6
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxxxxxxXxxxXXXXxxxx
## XXXXXXXX
Xxxxxxxxx xx XXX xxxxx xxx xx xxxxx$0 xxxxxxx xxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureStorageBlobSASToken [-Container] <String> [-Blob] <String> [-Context <AzureStorageContext>]
 [-ExpiryTime <DateTime]>] [-FullUri] [-IPAddressOrRange <String>] [-Permission <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartTime <DateTime]>]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureStorageBlobSASToken [-Container] <String> [-Blob] <String> [-Context <AzureStorageContext>]
 [-ExpiryTime <DateTime]>] [-FullUri] [-IPAddressOrRange <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartTime <DateTime]>]
 -Policy <String>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureStorageBlobSASToken [-Context <AzureStorageContext>] [-ExpiryTime <DateTime]>] [-FullUri]
 [-IPAddressOrRange <String>] [-Permission <String>]
 [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>] [-StartTime <DateTime]>]
 -CloudBlob <CloudBlob>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
New-AzureStorageBlobSASToken [-Context <AzureStorageContext>] [-ExpiryTime <DateTime]>] [-FullUri]
 [-IPAddressOrRange <String>] [-Protocol <Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]>]
 [-StartTime <DateTime]>] -CloudBlob <CloudBlob> -Policy <String>
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxXXXXxxxx$$ xxxxxx xxxxxxxxx x Xxxxxx Xxxxxx Xxxxxxxxx $XXX$ xxxxx xxx xx xxxxx$0 xxxxxxx xxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxxxx x xxxx XXX xxxxx xxxx xxxx xxxx xxxxxxxxxx
```
PS C:\>New-AzureStorageBlobSASToken -Container "ContainerName" -Blob "BlobName" -Permission rwd
```

Xxxx xxxxxxx xxxxxxxxx x xxxx XXX xxxxx xxxx xxxx xxxx xxxxxxxxxx.

### Xxxxxxx 0$ Xxxxxxxx x xxxx XXX xxxxx xxxx xxxx xxxx
```
PS C:\> $StartTime = Get-Date
PS C:\> $EndTime = $startTime.AddHours(2.0)
PS C:\> New-AzureStorageBlobSASToken -Container "ContainerName" -Blob "BlobName" -Permission rwd -StartTime $StartTime -ExpiryTime $EndTime
```

Xxxx xxxxxxx xxxxxxxxx x xxxx XXX xxxxx xxxx xxxx xxxx.

## XXXXXXXXXX

### $Xxxx
Xxxxxxxxx xxx xxxxxxx xxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxx
Xxxxxxxxx xxx $$XxxxxXxxx$$ xxxxxx.
Xx xxxxxx x $$XxxxxXxxx$$ xxxxxx$ xxx xxx Xxx$XxxxxXxxxxxxXxxx xxxxxx.

```yaml
Type: CloudBlob
Parameter Sets: UNNAMED_PARAMETER_SET_3, UNNAMED_PARAMETER_SET_4
Aliases: ICloudBlob

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxxxx
Xxxxxxxxx xxx xxxxxxx xxxxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxx
Xxxxxxxxx xxx xxxxxxx xxxxxxx.

```yaml
Type: AzureStorageContext
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxxXxxx
Xxxxxxxxx xxxx xxx xxxxxx xxxxxx xxxxxxxxx xxxxxxx.

```yaml
Type: DateTime]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxx
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxx xxx xxxx xxxx XXX xxx xxx xxxxxx xxxxxx xxxxxxxxx xxxxx.

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

### $XXXxxxxxxXxXxxxx
$$Xxxx$$

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
Xxxxxxxxx xxx xxxxxxxxxxx xxx x xxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxx
Xxxxxxxxx xx xxxxx$0 Xxxxxx Xxxxxx Xxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_4
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxx
$$Xxxx$$

```yaml
Type: Nullable [Microsoft.WindowsAzure.Storage.SharedAccessProtocol]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxxxx xxx xxxxxx xxxxxx xxxxxxxxx xxxxxxx xxxxx.

```yaml
Type: DateTime]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Xxx$XxxxxXxxxxxxXxxx](74bc4494-be41-4493-9939-e51e61dd09e6)

[Xxx$XxxxxXxxxxxxXxxxxxxxxXXXXxxxx](dc3564e2-9ede-4901-8d62-f49017a03281)


