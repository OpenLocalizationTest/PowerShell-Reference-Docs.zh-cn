---
external help file: SMAzure_Compute.xml
online version: 5e65fa22-f969-413e-b4a6-62242d022380
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXxxxxxxxxXxxxXxx
## XXXXXXXX
Xxxxxxx x xxxxxxxxx xxx xxxx xxx xx XXXX xxxxxx.

## XXXXXX

### XXXXXXX$XXXXXXXXX$XXX$0
```
Set-AzureSchedulerHttpJob [-ClientCertificatePassword <String>] [-ClientCertificatePfx <Object>]
 [-EndTime <DateTime>] [-ErrorActionHeaders <Hashtable>] [-ErrorActionMethod <String>]
 [-ErrorActionQueueMessageBody <String>] [-ErrorActionRequestBody <String>] [-ErrorActionSASToken <String>]
 [-ErrorActionStorageAccount <String>] [-ErrorActionStorageQueue <String>] [-ErrorActionURI <Uri>]
 [-ExecutionCount <Int32>] [-Frequency <String>] [-Headers <Hashtable>] [-HttpAuthenticationType <String>]
 [-Interval <Int32>] [-JobState <String>] [-Method <String>] [-PassThru] [-RequestBody <String>]
 [-StartTime <DateTime>] [-URI <Uri>] -JobCollectionName <String> -JobName <String> -Location <String>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Set-AzureSchedulerHttpJob [-ClientCertificatePassword <String>] [-ClientCertificatePfx <Object>]
 [-ErrorActionHeaders <Hashtable>] [-Headers <Hashtable>] [-JobState <String>] [-PassThru]
 -HttpAuthenticationType <String>
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Set-AzureSchedulerHttpJob [-EndTime <DateTime>] [-ErrorActionHeaders <Hashtable>] [-ExecutionCount <Int32>]
 [-Frequency <String>] [-Headers <Hashtable>] [-Interval <Int32>] [-JobState <String>] [-PassThru]
```

### XXXXXXX$XXXXXXXXX$XXX$0
```
Set-AzureSchedulerHttpJob [-ErrorActionHeaders <Hashtable>] [-Headers <Hashtable>] [-JobState <String>]
 [-PassThru] [-RequestBody <String>]
```

## XXXXXXXXXXX
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.00 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $Xxx$Xxxxxx $Xxxx Xxxxx$.Xxxxxxx.

Xxx Xxx$XxxxxXxxxxxxxxXxxxXxx xxxxxx xxxxxxx x xxxxxxxxx xxx xxxx xxx xx XXXX xxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx xxx xxxxx xx x xxx xx Xxxxxxxx
```
PS C:\>Set-AzureSchedulerHttpJob -Location "North Central US" -JobCollectionName "JobCollection01" -JobName "Job01" -JobState "Disabled"
```

Xxxx xxxxxxx xxxxxxx xxx xxxxx xx xxx xxx xxxxx Xxx00 xx Xxxxxxxx.
Xxxx xxx xx xxxx xx xxx xxx xxxxxxxxxx xxxxx XxxXxxxxxxxxx00 xxx xxx xxxxxxxxx xxxxxxxx.

### Xxxxxxx 0$ Xxxxxx xxx XXX xx x xxx
```
PS C:\>Set-AzureSchedulerHttpJob -Location "North Central US" -JobCollectionName "JobCollection02" -JobName "Job37" -URI http://www.contoso.com
```

Xxxx xxxxxxx xxxxxxx xxx XXX xx xxx xxx xxxxx Xxx00 xx xx xxxx$$$xxx.xxxxxxx.xxx.

## XXXXXXXXXX

### $XxxxxxXxxxxxxxxxxXxxxxxxx
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

### $XxxxxxXxxxxxxxxxxXxx
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

### $XxxXxxx
Xxxxxxxxx x xxxx$ xx x XxxxXxxx xxxxxx$ xxx xxx xxxxxxxxx xx xxxx xxxxxxxxxx xxxx.
Xx xxxxxx x XxxxXxxx xxxxxx$ xxx xxx Xxx$Xxxx xxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxxx Xxx$Xxxx Xxx$Xxxx.

```yaml
Type: DateTime
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxxXxxxxxx
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

### $XxxxxXxxxxxXxxxxx
Xxxxxxxxx xxx xxxxxx xxx XXXX xxx XXXXX xxxxxx xxxxx.
Xxxxx xxxxxx xxx$ 

$$ XXX $$ XXX $$ XXXX $$ XXXX $$ XXXXXX

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxxXxxxxXxxxxxxXxxx
Xxxxxxxxx xxx xxxx xxx xxxxxxx xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxxXxxxxxxXxxx
Xxxxxxxxx xxx xxxx xxx XXX xxx XXXX xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxxxxXXXXxxxx
Xxxxxxxxx xxx Xxxxxx Xxxxxx Xxxxxxxxx $XXX$ xxxxx xxx xxx xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxxxxXxxxxxxXxxxxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxxxxXxxxxxxXxxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxx xxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxxxXxxxxxXXX
Xxxxxxxxx xxx XXX xxx xxx xxxxx xxx xxxxxx.

```yaml
Type: Uri
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxxxxxXxxxx
Xxxxxxxxx xxx xxxxxx xxxxxxxxxxx xx x xxx xxxx xxx.
Xx xxxxxxx$ x xxx xxxxxx xxxxxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxxxx
Xxxxxxxxx xxx xxxxxxx xxxxxxxxx xxx xxxx xxxxxxxxx xxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $Xxxxxxx
Xxxxxxxxx xxx xxxxxxx xx x xxxx xxxxx.

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

### $XxxxXxxxxxxxxxxxxxXxxx
$$Xxxx$$

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

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

### $Xxxxxxxx
Xxxxxxxxx xxx xxxxxxxx xx xxxxxxxxxx xx xxx xxxxxxxxx xxxxxxxxx xx xxxxx xxx Xxxxxxxxx xxxxxxxxx.

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxXxxxxxxxxxXxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxxxx xxxx xxxxxxxx xxx xxxxxxxxx xxx xx xxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxXxxx
Xxxxxxxxx xxx xxxx xx xxxxxxxxx xxx xx xxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### $XxxXxxxx
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

### $Xxxxxxxx
Xxxxxxxxx xxx xxxx xx xxx xxxxxxxx xxxx xxxxx xxx xxxxx xxxxxxx.
Xxxxx xxxxxx xxx$ 

$$ Xxxxxxxx Xxxx $$ Xxxxxxxx Xxxxxx $$ Xxxxxxxx XX $$ Xxxx Xxxx $$ Xxxx XX $$ Xxxxx Xxxxxxx XX $$ Xxxxx Xxxxxx $$ Xxxxx Xxxxxxx XX $$ Xxxxxxxxx Xxxx $$ Xxxx Xxxxxx $$ Xxxx XX

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

### $Xxxxxx
Xxxxxxxxx xxx xxxxxx xxx XXXX xxx XXXXX xxxxxx xxxxx.
Xxxxx xxxxxx xxx$ 

$$ XXX $$ XXX $$ XXXX $$ XXXX $$ XXXXXX

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxXxxx
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx xx xxxxxx xxxxxxxxxxxx xxx xxxx xx xxxxx xx xxxxxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

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

### $XxxxxxxXxxx
Xxxxxxxxx xxx xxxx xxx XXX xxx XXXX xxx xxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_4
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XxxxxXxxx
Xxxxxxxxx x xxxx$ xx x XxxxXxxx xxxxxx$ xxx xxx xxx xx xxxxx.

```yaml
Type: DateTime
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### $XXX
Xxxxxxxxx x XXX xxx x xxx xxxxxx.

```yaml
Type: Uri
Parameter Sets: UNNAMED_PARAMETER_SET_1
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

[Xxx$XxxxxXxxxxxxxxXxxxXxx](5e65fa22-f969-413e-b4a6-62242d022380)


