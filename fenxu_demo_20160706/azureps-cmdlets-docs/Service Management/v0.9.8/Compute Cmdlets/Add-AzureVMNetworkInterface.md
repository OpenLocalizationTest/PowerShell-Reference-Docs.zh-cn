---
external help file: SMAzure_Compute.xml
online version: 
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXXXxxxxxxXxxxxxxxx
## XXXXXXXX
Xxx x Xxxxxxx Xxxxxxxxx xx xxx XX

## XXXXXX

```
Add-AzureVMNetworkInterface [-VM] <PSVirtualMachine> [-Id] <String> [-Profile <AzureProfile>]
```

## XXXXXXXXXXX
Xxxx xxxxxxx xxxxxx xxx xx xxx x XXX xx xxx XX xx xxxxxxxx xxxx xx xx xx xxxxxxxx XX

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$  Xxx x Xxxxxxx Xxxxxxxxx xx x xxx XX  $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\> # Get the VM
          $vm = Get-AzureVM -ResourceGroupName "myRG" -Name "crpVM

          # Add a Network Interface to the VM
          Add-AzureVMNetworkInterface ?VM $vm ?Id "/subscriptions/subscriptionId/resourceGroups/resourceGroupName/providers/Microsoft.Network/NetworkAdapters/Nic1"
```

### $$$$$$$$$$$$$$$$$$$$$$$$$$  Xxx x Xxxxxxx Xxxxxxxxx xx xx xxxxxxxx XX  $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\> # Get the VM
          $vm = Get-AzureVM -ResourceGroupName "myRG" -Name "crpVM"

          # Add a Network Interface to the VM
          Add-AzureVMNetworkInterface ?VM $vm ?Id "/subscriptions/subscriptionId/resourceGroups/resourceGroupName/providers/Microsoft.Network/NetworkAdapters/Nic1"

          # Update VM state
          Update-AzureVM -ResourceGroupName "myRG" -Name "crpVM" ?VM $vm
```

## XXXXXXXXXX

### $Xx
Xx xx xxx Xxxxxxx Xxxxxxxxx.
Xxxx xxx xx xxxxxx xxxxx xxx Xxx$XxxxxXxxxxxxXxxxxxxxx xxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: NicId,NetworkInterfaceId

Required: True
Position: 2
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxxxxxx
```yaml
Type: AzureProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### $XX
Xxxxx XX Xxxxxx xx xxx xxx Xxxxxxx Xxxxxxxxx xx.
Xxx xxxxx XX xxxxxx xxx xx xxxxxxx xxxx Xxx$XxxxxXXXxxxxx xxxxxx xx xxxxxx xxxxxxx xxx Xxx$XxxxxXX xxxxxx.

```yaml
Type: PSVirtualMachine
Parameter Sets: (All)
Aliases: VMProfile

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX


