---
external help file: SMAzure_Compute.xml
online version: 
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Publish-AzureServiceProject
## XXXXXXXX
Xxxxxxx xxx xxxxxxx xxxxxxx xx Xxxxxxx Xxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
Publish-AzureServiceProject [[-ServiceName] <String>] [-AffinityGroup <String>] [-DeploymentName <String>]
 [-ForceUpgrade] [-Launch] [-Location <String>] [-Slot <String>] [-StorageAccountName <String>]
```

### UNNAMED_PARAMETER_SET_2
```
Publish-AzureServiceProject [[-Package] <String>] [-Configuration] <String> [-AffinityGroup <String>]
 [-DeploymentName <String>] [-ForceUpgrade] [-Launch] [-Location <String>] [-Slot <String>]
 [-StorageAccountName <String>]
```

## XXXXXXXXXXX
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.00 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $Xxx$Xxxxxx $Xxxx Xxxxx$.Xxxxxxx.

Xxx Xxxxxxx$XxxxxXxxxxxxXxxxxxx xxxxxx xxxxxxxxx xxx xxxxxxx xxxxxxx xx xxx xxxxx.
Xxx xxx xxxxxxx xxxxxxxxxx xxxxxxxxxxxxx $xxxx xx Xxxxxxxxxxxx$ XxxxxxxXxxxxxxXxxx$ Xxxxxxxx$ Xxxx$ xx xxx xxxxxxx xxxx$ xx xx xxxxx xxxxxxxx xxxxxxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx.

## XXXXXXXX

### 0$ Xxxxxxx x xxxxxxx xxxxxxx xxxx xxxxxxx xxxxxx
```
PS C:\>Publish-AzureServiceProject
```

Xxxx xxxxxxx xxxxxxxxx xxx xxxxxxx xxxxxxx$ xxxxx xxx xxxxxxx xxxxxxx xxxxxxxx xxx xxx xxxxxxx Xxxxx xxxxxxx xxxxxxx.

### 0$ Xxxxxx x xxxxxxxxxx xxxxxxx
```
PS C:\>Publish-AzureServiceProject -PackageOnly
```

Xxxxxxx x xxxxxxxxxx xxxxxxx $.xxxxx$ xxxx xx xxx xxxxxxx xxxxxxxxx xxx xxxx xxx xxxxxxx xx Xxxxxxx Xxxxx.

## XXXXXXXXXX

### -AffinityGroup
Xxxxxxxxx xxx xxxxxxxx xxxxx xxxx xxx xxxx xxx xxxxxxx xx xxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: ag

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Configuration
Xxxxxxxxx xxx xxxxxxx xxxxxxxxxxxxx xxxx.
Xx xxx xxxxxxx xxxx xxxxxxxxx$ xxxxxxx xxx Xxxxxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: cc

Required: True
Position: 2
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DeploymentName
Xxxxxxxxx xxx xxxxxxxxxx xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: dn

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ForceUpgrade
$$Xxxx$$

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: f

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Launch
Xxxxx x xxxxxxx xxxxxx xx xxx xxx xxxx xxx xxxxxxxxxxx xxxxx xx xx xxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: ln

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Location
Xxx xxxxxx xx xxxxx xxx xxxxxxxxxxx xxxx xx xxxxxx.
Xxxxxxxx xxxxxx xxx$ Xxxxxxxx Xxxx$ Xxxxxxxx Xxxxxx$ Xxxxxxxx XX$ Xxxx Xxxx$ Xxxx XX$ Xxxxx Xxxxxxx XX$ Xxxxx Xxxxxx$ Xxxxx Xxxxxxx XX$ Xxxxxxxxx Xxxx$ Xxxx Xxxxxx$ Xxxx XX. Xx xx Xxxxxxxx xx xxxxxxxxx$ xxx xxxxxxxx xxxxxxxxx xx xxx xxxx xxxx xx Xxx$XxxxxXxxxxxxXxxxxxx xxxx xx xxxx. Xx xx Xxxxxxxx xxx xxxx xxxxxxxxx$ xxx Xxxxxxxx xxxx xx xxxxxxxx xxxxxx xxxx $Xxxxx Xxxxxxx XX$ xxx $Xxxxx Xxxxxxx XX$ xxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: l

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Package
Xxxxxxxxx xxx xxxxxxx xxxx xx xxxxxx.
Xxxxxxx xxxxxx x xxxxx xxxx xxxx xxx xxx .xxxxx xxxx xxxx xxxxxxxxx xx x XXX xx x xxxx xxxx xxxxxxxx xxx xxxxxxx.
Xx xxx xxxxxxx xxxx xxxxxxxxx$ xx xxx xxxxxxx xxx XxxxxxxXxxx xxxxxxxxx.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: sp

Required: False
Position: 1
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServiceName
Xxxxxxxxx xxx xxxx xx xx xxxx xxx xxx xxxxxxx xxxx xxxxxxxxxx xx Xxxxxxx Xxxxx.
Xxx xxxx xxxxxxxxxx xxxx xx xxx xxxxx xx xxx xxxxxxxx.xxx xxxxxxxxx xxxx xx xxxx xx xxxxxxx xxx xxxxxxx xxxx xxxxxx xx Xxxxxxx Xxxxx $xxxx xx$ xxxx.xxxxxxxx.xxx$.
Xxx xxxx xxxxxxxxx xxxxx xxxxxxxxxx xxx xxxxxxx xxxxxxxxx xxx xxxx xxxxx xxxx xxx xxxxxxx xxx xxxxxxx.
$Xxx xxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxx$.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: sv

Required: False
Position: 1
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
Xxx xxxxxxxxxx xxxx xx xx xxxx xxx xxxx xxxxxxx.
Xxxxxxxx xxxxxx xxx $Xxxxxxx$ xxx $Xxxxxxxxxx$.
Xx xx xxxx xx xxxxxxxxx$ xxx xxxx xxxxxxxx xx xxx xxxx xxxx xx Xxx$XxxxxXxxxxxxxxxXxxx xx xxxx.
Xx xx xxxx xxx xxxx xxxx xxxxxxxxx$ xxx $Xxxxxxxxxx$ xxxx xx xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: sl

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StorageAccountName
Xxxxxxxxx xxx Xxxxxxx Xxxxx xxxxxxx xxxxxxx xxxx xx xx xxxx xxxxx xxxxxxxxxx xxx xxxxxxx.
Xxxx xxxxx xx xxx xxxx xxxxx xxx xxxxxxx xx xxxxxxxxx.
Xxxx xxxx xxxxxxxxx xx xxx xxxxxxxxx$ xxx xxxxx xx xxxxxxxx xxxx xxx xxxx Xxx$XxxxxXxxxxxxXxxxxxx xxxxxxx.
Xx xx xxxxxxx xxxxxxx xxx xxxx xxxxxxxxx$ x xxxxxxx xxxxxxx xxxxxxxx xxx xxxx xx xxx xxxxxxx xxxx xx xxxx.
Xx xx xxxx xxxxxxx xxxxxxx xxxxxx$ xxx xxxxxx xxxxxxxx xx xxxxxx x xxx xxx.
Xxxxxxx$ xxx xxxxxxx xxx xxxx xx x xxxxxxx xxxxxxx xxxxxxxx xxx xxxxxxx xxxx xxxxxx xx xxxxxxx xxxxxxxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: st

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

[Enable-AzureServiceProjectRemoteDesktop](8d3f7f43-f8f6-4ecf-b8be-7c69cd10cde7)

[Set-AzureServiceProject](c3baa783-e57a-46bd-abe4-6d06130eaaf0)


