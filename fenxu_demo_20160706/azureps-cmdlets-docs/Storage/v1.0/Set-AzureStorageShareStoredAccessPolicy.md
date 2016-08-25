---
external help file: RMAzure_Storage.xml
online version: d3ad790c-c75f-4243-b128-7c778422ac64
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Set-AzureStorageShareStoredAccessPolicy
## XXXXXXXX
Xxxxxxx x xxxxxx xxxxxx xxxxxx xx x Xxxxxxx xxxxx.

## XXXXXX

```
Set-AzureStorageShareStoredAccessPolicy [-ShareName] <String> [-Policy] <String>
 [-ClientTimeoutPerRequest <Nullable [System.Int32]>] [-ConcurrentTaskCount <Nullable [System.Int32]>]
 [-Context <AzureStorageContext>] [-ExpiryTime <Nullable [System.DateTime]>] [-NoExpiryTime] [-NoStartTime]
 [-Permission <String>] [-ServerTimeoutPerRequest <Nullable [System.Int32]>]
 [-StartTime <Nullable [System.DateTime]>]
```

## XXXXXXXXXXX
Xxx $$Xxx$XxxxxXxxxxxxXxxxxXxxxxxXxxxxxXxxxxx$$ xxxxxx xxxxxxx xxxxxx xxxxxx xxxxxx xx xx xxxxx$0 Xxxxxxx xxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxx xxxxxx xxxxxx xx Xxxxxxx xxxxx
```
PS C:\>Set-AzureStorageShareStoredAccessPolicy -ShareName "ContosoShare" -Policy "GeneralPolicy" -Permission "rwdl"
```

Xxxx xxxxxxx xxxxxxx x xxxxxx xxxxxx xxxxxx xxxx xxx xxxx xxxxxxxxxx xx x xxxxx.

## XXXXXXXXXX

### -ClientTimeoutPerRequest
$$Xxxx$$

```yaml
Type: Nullable [System.Int32]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConcurrentTaskCount
$$Xxxx$$

```yaml
Type: Nullable [System.Int32]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Context
$$Xxxx$$

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

### -ExpiryTime
$$Xxxx$$

```yaml
Type: Nullable [System.DateTime]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoExpiryTime
$$Xxxx$$

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

### -NoStartTime
$$Xxxx$$

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

### -Permission
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

### -Policy
$$Xxxx$$

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServerTimeoutPerRequest
$$Xxxx$$

```yaml
Type: Nullable [System.Int32]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ShareName
Xxxxxxxxx xxx xxxx xx xxx Xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: N,Name

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

### -StartTime
$$Xxxx$$

```yaml
Type: Nullable [System.DateTime]
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

[Get-AzureStorageShareStoredAccessPolicy](d3ad790c-c75f-4243-b128-7c778422ac64)

[New-AzureStorageContext](671aeec8-b7f9-49c5-866f-da84f189ab5b)

[New-AzureStorageShareStoredAccessPolicy](d5b956f0-92ca-4246-9860-dfa96f17ed8a)

[Remove-AzureStorageShareStoredAccessPolicy](af46a7c9-dd40-4d0d-9950-56f661dada33)


