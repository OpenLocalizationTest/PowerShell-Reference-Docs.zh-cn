---
external help file: SMAzure_Compute.xml
online version: 
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Set-AzureWebsite
## XXXXXXXX
Xxxxxxxxxx x xxxxxxx xxxxxxx xx Xxxxx.

## XXXXXX

```
Set-AzureWebsite [[-Name] <String>] [[-SiteWithConfig] <SiteWithConfig>] [-AppSettings <Hashtable>]
 [-AutoSwapSlotName <String>] [-ConnectionStrings <ConnStringPropertyBag>] [-DefaultDocuments <String[]>]
 [-DetailedErrorLoggingEnabled <Boolean>] [-HandlerMappings <HandlerMapping[]>] [-HostNames <String[]>]
 [-HttpLoggingEnabled <Boolean>] [-ManagedPipelineMode] [-Metadata <List<NameValuePair>>]
 [-NetFrameworkVersion <String>] [-NumberOfWorkers <Int32>] [-PassThru] [-PhpVersion <String>]
 [-RequestTracingEnabled <Boolean>] [-RoutingRules <List<RoutingRule>>] [-Slot <String>]
 [-SlotStickyAppSettingNames <List<String>>] [-SlotStickyConnectionStringNames <List<String>>]
 [-Use32BitWorkerProcess <Boolean>] [-WebSocketsEnabled <Boolean>]
```

## XXXXXXXXXXX
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.00 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $Xxx$Xxxxxx $Xxxx Xxxxx$.Xxxxxxx.

Xxx Xxx$XxxxxXxxxxxx xxxxxx xxxxxxxxxx x xxxxxxx xxxxxxx xx Xxxxx.

## XXXXXXXX

### 0$ Xxxxxx XXXX xxxxxxx xxx x xxxxxxx
```
PS C:\>Set-AzureWebsite -HttpLoggingEnabled 1
```

Xxxx xxxxxxx xxxxxxx XXXX xxxxxxx.

### 0$ Xxx xxxxxxx xxxxxxxxxxx xxx x xxxxxxx
```
PS C:\>$settings = New-Object Hashtable$settings[â€œAZURE_STORAGE_ACCOUNTâ€= myaccountname$settings[â€œAZURE_STORAGE_ACCESS_KEYâ€] = myaccesskeySet-AzureWebsite -AppSettings $settings myWebsite
```

Xxxx xxxxxxx xxxx xxxxxxx xxxxxxxxxxx xx x xxxxxxx xxxxx xxXxxxxxx xxxx xxxxxxxxxxx xxxxxxxxx xxx XXXXX$XXXXXXX$XXXXXXX xxx XXXXX$XXXXXXX$XXXXXX$XXX.

## XXXXXXXXXX

### -AppSettings
Xxxxxxxxx xxx xxxxxxxxxxx xxxxxxxxx xxxx xxxx xx xxxx xx xxx xxxxxxx.

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

### -AutoSwapSlotName
$$Xxxx$$

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

### -ConnectionStrings
Xxxxxxxxx xxx xxxxxxxxxx xxxxxxx xxxx xx xxx xxxxxxx.

```yaml
Type: ConnStringPropertyBag
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DefaultDocuments
Xxxxxxxxx xxx xxxxxxxxx xxxx xxx xxxxxxxxxxxxx xxxxxxxxx xxxx xxxxxxxx xxx xxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DetailedErrorLoggingEnabled
Xxxxxxxxxx xxxxxxx xxxxxxxx XXX xxxxxx xxx xxxxxx xxx xxx xxxxxxx.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -HandlerMappings
Xxxxxxxxx xxx xxxxxxx xxxxxxxx xxxx xx xxx xxxxxxx.

```yaml
Type: HandlerMapping[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -HostNames
Xxxxxxxxx xxx xxxxx xxxxxxxxx xxxx xxxxx xxxx xxx xx xxxx xx xxxxxx xxx xxxxxxx.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -HttpLoggingEnabled
Xxxxxxxxxx xxxxxxx xxxx xxxxxxx xx xxxxxxx xxx xxx xxxxxxx.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ManagedPipelineMode
Xxxxxxxxx xxx xxxxxxx xxxxxxxx xxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Integrated, Classic

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Metadata
Xxxxxxxxx xxx xxxxxxxx xxx xxx xxxxxxx.

```yaml
Type: List<NameValuePair>
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx xxx xxxx xx xxx xxxxxxx.
\<Xxxx$$$x xxxx xx xxxx xxx$$$x xxxxxxxxx$\>

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

### -NetFrameworkVersion
Xxxxxxxxx xxx xxxxxxx xx xxx .Xxx Xxxxxxxxx xxxxxxxx xx xxx xxxxxxx.

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

### -NumberOfWorkers
Xxxxxxxxx xxx xxxxxx xx xxxxxx xxxxxxxxx xxxxxxx xxx xxxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
Xxxxxxxxx xxxx xxxx xxxxxx xxxxxxx x Xxxxxxx xxxxx.

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

### -PhpVersion
Xxxxxxxxx xxx XXX xxxxxxx xxxxxxxx xx xxx xxxxxxx.

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

### -RequestTracingEnabled
Xxxxxxxxxx xxxxxxx xxxxxxx xxxxxxx xx xxxxxxx xxx xxx xxxxxxx.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -RoutingRules
Xxxxxxxxx xxx xxxxxxx xxxxx xx xxx xxx xxxxxxx xx xxxxxxxxxx.

```yaml
Type: List<RoutingRule>
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SiteWithConfig
Xxxxxxxxx xxx xxxxxxxxxxxxx xxxx xx xxx xxxxxxx.

```yaml
Type: SiteWithConfig
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
Xxxxxxxxx xxx xxxx xxxx xx xxx xxxxxxx.

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

### -SlotStickyAppSettingNames
$$Xxxx$$

```yaml
Type: List<String>
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SlotStickyConnectionStringNames
$$Xxxx$$

```yaml
Type: List<String>
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Use32BitWorkerProcess
Xxxxxxxxx xxxxxxx xx xxxxxx 00$xxx xxxx.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -WebSocketsEnabled
Xxxxxxxxx xxxxxxx xx xxxxxx XxxXxxxxxx.

```yaml
Type: Boolean
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

[Get-AzureWebsite](0c2a5092-db45-4ce7-b39b-d1e499b4a867)


