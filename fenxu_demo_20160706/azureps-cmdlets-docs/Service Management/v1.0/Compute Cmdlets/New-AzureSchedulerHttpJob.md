---
external help file: SMAzure_Compute.xml
online version: 23b849a7-7403-491a-9d21-2104137052ec
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# New-AzureSchedulerHttpJob
## XXXXXXXX
Xxxxxxx x xxxxxxxxx xxx xxxx xxx xx XXXX xxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
New-AzureSchedulerHttpJob [-ClientCertificatePassword <String>] [-ClientCertificatePfx <Object>]
 [-ErrorActionHeaders <Hashtable>] [-Headers <Hashtable>] [-JobState <String>] -HttpAuthenticationType <String>
```

### UNNAMED_PARAMETER_SET_2
```
New-AzureSchedulerHttpJob [-ClientCertificatePassword <String>] [-ClientCertificatePfx <Object>]
 [-EndTime <DateTime>] [-ErrorActionHeaders <Hashtable>] [-ErrorActionMethod <String>]
 [-ErrorActionQueueMessageBody <String>] [-ErrorActionRequestBody <String>] [-ErrorActionSASToken <String>]
 [-ErrorActionStorageAccount <String>] [-ErrorActionStorageQueue <String>] [-ErrorActionURI <Uri>]
 [-ExecutionCount <Int32>] [-Frequency <String>] [-Headers <Hashtable>] [-HttpAuthenticationType <String>]
 [-Interval <Int32>] [-JobState <String>] [-RequestBody <String>] [-StartTime <DateTime>]
 -JobCollectionName <String> -JobName <String> -Location <String> -Method <String> -URI <Uri>
```

### UNNAMED_PARAMETER_SET_3
```
New-AzureSchedulerHttpJob [-EndTime <DateTime>] [-ErrorActionHeaders <Hashtable>] [-ExecutionCount <Int32>]
 [-Frequency <String>] [-Headers <Hashtable>] [-Interval <Int32>] [-JobState <String>]
```

### UNNAMED_PARAMETER_SET_4
```
New-AzureSchedulerHttpJob [-ErrorActionHeaders <Hashtable>] [-Headers <Hashtable>] [-JobState <String>]
 [-RequestBody <String>]
```

## XXXXXXXXXXX
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.00 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $Xxx$Xxxxxx $Xxxx Xxxxx$.Xxxxxxx.

Xxx Xxx$XxxxxXxxxxxxxxXxxxXxx xxxxxx xxxxxxx x xxxxxxxxx xxx xxxx xxx xx XXXX xxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx xx XXXX xxx
```
PS C:\>New-AzureSchedulerHttpJob -JobCollectionName "JobCollection01" -JobName "Job01" -Location "North Central US" -Method "GET" -URI http://www.contoso.com
```

Xxxx xxxxxxx xxxxxxx x xxxxxxxxx XXXX xxx xx xxx xxx xxxxxxxxxx xxxxx XxxXxxxxxxxxx00.
Xxx xxxxxxx xxxxxxxxx x XXX xxx xxxxxxxxx XXX xx xxx xxxxxx.

### Xxxxxxx 0$ Xxxxxx xx XXXX xxx xxx x xxxxxxxx xxx xxxxx
```
PS C:\>New-AzureSchedulerHttpJob -JobCollectionName "JobCollection01 -JobName "Job23" -Location "North Central US" -Method "GET" -URI http://www.contoso.com -ExecutionCount 20
```

Xxxx xxxxxxx xxxxxxx xxxxxxxxx xxxx xxx xx xxx xxx xxxxxxxxxx xxxxx XxxXxxxxxxxxx00.
Xxx xxxxxxx xxxxxxxxx x XXX xxx xxxxxxxxx XXX xx xxx xxxxxx.
Xxxx xxxxxxx xxxxxx xxx xxx xx xxx 00 xxxxx.

## XXXXXXXXXX

### -ClientCertificatePassword
$$Xxxx$$

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClientCertificatePfx
$$Xxxx$$

```yaml
Type: Object
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndTime
Xxxxxxxxx x xxxx$ xx x XxxxXxxx xxxxxx$ xxx xxx xxxxxxxxx xx xxxx xxxxxxxxxx xxxx.
Xx xxxxxx x XxxxXxxx xxxxxx$ xxx xxx Xxx$Xxxx xxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxxx Xxx$Xxxx Xxx$Xxxx.

```yaml
Type: DateTime
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -ErrorActionHeaders
Xxxxxxxxx xxxxxxx xx x xxxxxxxxx.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionMethod
Xxxxxxxxx xxx xxxxxx xxx XXXX xxx XXXXX xxxxxx xxxxx.
Xxxxx xxxxxx xxx$ 

$$ XXX $$ XXX $$ XXXX $$ XXXX $$ XXXXXX

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

### -ErrorActionQueueMessageBody
Xxxxxxxxx xxx xxxx xxx xxxxxxx xxx xxxxxxx.

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

### -ErrorActionRequestBody
Xxxxxxxxx xxx xxxx xxx XXX xxx XXXX xxx xxxxxxx.

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

### -ErrorActionSASToken
Xxxxxxxxx xxx Xxxxxx Xxxxxx Xxxxxxxxx $XXX$ xxxxx xxx xxx xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionStorageAccount
Xxxxxxxxx xxx xxxx xx xxx xxxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionStorageQueue
Xxxxxxxxx xxx xxxx xx xxx xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionURI
Xxxxxxxxx xxx XXX xxx xxx xxxxx xxx xxxxxx.

```yaml
Type: Uri
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExecutionCount
Xxxxxxxxx xxx xxxxxx xxxxxxxxxxx xx x xxx xxxx xxx.
Xx xxxxxxx$ x xxx xxxxxx xxxxxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Frequency
Xxxxxxxxx xxx xxxxxxx xxxxxxxxx xxx xxxx xxxxxxxxx xxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Headers
Xxxxxxxxx xxx xxxxxxx xx x xxxxxxxxx.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -HttpAuthenticationType
$$Xxxx$$

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

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

### -Interval
Xxxxxxxxx xxx xxxxxxxx xx xxxxxxxxxx xx xxx xxxxxxxxx xxxxxxxxx xx xxxxx xxx Xxxxxxxxx xxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -JobCollectionName
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxxx xx xxxxxxx xxx xxxxxxxxx xxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobName
Xxxxxxxxx xxx xxxx xxx xxx xxxxxxxxx xxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobState
Xxxxxxxxx xxx xxxxx xxx xxx xxxxxxxxx xxx.

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

### -Location
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx xxxx xxxxx xxx xxxxx xxxxxxx.
Xxxxx xxxxxx xxx$ 

$$ Xxxxxxxx Xxxx $$ Xxxxxxxx Xxxxxx $$ Xxxxxxxx XX $$ Xxxx Xxxx $$ Xxxx XX $$ Xxxxx Xxxxxxx XX $$ Xxxxx Xxxxxx $$ Xxxxx Xxxxxxx XX $$ Xxxxxxxxx Xxxx $$ Xxxx Xxxxxx $$ Xxxx XX

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Method
Xxxxxxxxx xxx xxxxxx xxx XXXX xxx XXXXX xxxxxx xxxxx.
Xxxxx xxxxxx xxx$ 

$$ XXX $$ XXX $$ XXXX $$ XXXX $$ XXXXXX

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -RequestBody
Xxxxxxxxx xxx xxxx xxx XXX xxx XXXX xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2, UNNAMED_PARAMETER_SET_4
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartTime
Xxxxxxxxx x xxxx$ xx x XxxxXxxx xxxxxx$ xxx xxx xxx xx xxxxx.

```yaml
Type: DateTime
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -URI
Xxxxxxxxx x XXX xxx x xxx xxxxxx.

```yaml
Type: Uri
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Set-AzureSchedulerHttpJob](23b849a7-7403-491a-9d21-2104137052ec)


