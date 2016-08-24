---
external help file: SMAzure_Compute.xml
online version: 
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Xxx$XxxxxXXXxxxXxxx
## XXXXXXXX
Xxx Xxxx Xxxx xx XX

## XXXXXX

```
Add-AzureVMDataDisk [-VM] <PSVirtualMachine> [-Name] <String> [[-VhdUri] <String>] [-Caching]
 [-DiskSizeInGB] <Int32> [[-Lun] <Int32>] [-Profile <AzureProfile>]
```

## XXXXXXXXXXX
Xxxx xxxxxxx xxxxxx xxx xx xxx x Xxxx Xxxx xx xxx XX xx xxxxxxxx xxxx xx xx xx xxxxxxxx XX

## XXXXXXXX

### $$$$$$$$$$$$$$$$$$$$$$$$$$  Xxx Xxxx Xxxx xx x xxx XX  $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\> # Create the local VM Object
          $vm =  New-AzureVMConfig ?VMName ?myVM? ?VMSize ?Standard_A1" -AvailabilitySetID $as1.Id

          # Add Data Disk disk1 to this VM
          Add-AzureVMDataDisk ?VM $vm ?Name "disk1" ?VhdUri "http://storageaccountname.blob.core.windows.net/vhds/test2.vhd" ?LUN 0 ?Caching ReadOnly ?DiskSizeinGB 1
```

### $$$$$$$$$$$$$$$$$$$$$$$$$$  Xxx x Xxxx Xxxx xx xx xxxxxxxx XX  $$$$$$$$$$$$$$$$$$$$$$$$$$
```
PS C:\> # Get the VM
          $vm = Get-AzureVM -ResourceGroupName "myRG" -Name "crpVM"

          # Add Data Disk disk1 to VM
          Add-AzureVMDataDisk ?VM $vm ?Name "disk1" ?VhdUri "http://storageaccountname.blob.core.windows.net/vhds/test2.vhd" ?LUN 0 ?Caching ReadOnly ?DiskSizeinGB 1

          # Update VM state
          Update-AzureVM -ResourceGroupName "myRG" -Name "crpVM" ?VM $vm
```

## XXXXXXXXXX

### $Xxxxxxx
Xxxxxxxxx xxx xxxxxxx xxxx xx xxx xxxx.
Xxxx xxxxxxx xxxxxxx xxx xxxxxxxxxxx xxx xxxxxxxxxxx xx xxx xxxx.
Xxxx$ Xxxxxxxx xxxx xxxxx xxxxxx xxx Xxxxxxx Xxxxxxx xx xxxxxx.
Xxxxxxxx xxxxxx xxx$ $
XxxxXxxx $
XxxxXxxxx Xxx xxxxxxx xxxxx xx XxxxXxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: ReadOnly, ReadWrite

Required: False
Position: 4
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XxxxXxxxXxXX
Xxxxxxxxx xxx xxxx$ xx XX$ xx xx xxxxx xxxx xx xx xxxxxxxx xx xxx Xxxxxxx Xxxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
Position: 5
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxx
Xxxxxxxxx xxx Xxxxxxx Xxxx Xxxxxx $XXX$ xxx xxx xxxx xxxx.
Xx xxx xxxx xx xxx xxxxx xxxx xxxx xx xxxxx$ xxxx xxxxxxx xx xxxxxxxx xxx xxx xxxxxxx xxxxx xx 0 xx xxxx.
Xx xxxx xxxx xxx xxxx xx xxxxx xxxxx$ xxxx xxxxxxx xx xxxxxxxx.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 6
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $Xxxx
Xxxx xx xxx Xxxx Xxxx

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

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

### $XxxXxx
Xxxxxxxxx xxx XXX xxxx xxxx xxxxx xx xx xxxxxxx xxxx x xxxxxxxx xxxxx xx xxxx xxxxx xx xxxx.
Xxxx xx xxxxx xxx xxxxx xxxx xxxx xx xxxxxx xx xxxxx xxx XX xxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### $XX
Xxxxx XX Xxxxxx xx xxx xxx Xxxx Xxxx xx.
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


