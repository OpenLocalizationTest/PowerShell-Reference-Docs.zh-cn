---
external help file: SMAzure_Compute.xml
online version: 4b060a7d-da50-45ff-adb6-bcba63faa90b
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Remove-WAPackVM
## XXXXXXXX
Xxxxxxx xxxxxxx xxxxxxx xxxxxxx.

## XXXXXX

```
Remove-WAPackVM [-VM] <VirtualMachine> [-PassThru] [-Force] [-Confirm] [-WhatIf]
```

## XXXXXXXXXXX
Xxxxx xxxxxx xxx xxxxxxxxxx xxx xxxx xx xxxxxxx xx xxx xxxxxx.
Xxx xxx xxxxxxx xxxxxx$ xxx  Xxxxx XXXxxx Xxxxxxxxxxx$$$xxxx.xxxxxxxxx.xxx$xxxxxxx$xx000000.xxxx.
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.0 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxxx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xxxx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $xxx$xxxxxx xxxxx$.xxxxxxx.

Xxx Xxxxxx$XXXxxxXX xxxxxx xxxxxxx xxxxxxx xxxxxxx xxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxxxxxx
```
PS C:\>$VirtualMachine = Get-WAPackVM -Name "ContosoV126"
PS C:\> Remove-WAPackVM -VM $VirtualMachine
```

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxx xxxxx XxxxxxxX000 xx xxxxx xxx Xxx$XXXxxxXX xxxxxx$ xxx xxxx xxxxxx xxxx xxxxxx xx xxx $XxxxxxxXxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx xxx xxxxxxx xxxxxxx xxxxxx xx $XxxxxxxXxxxxxx.
Xxx xxxxxxx xxxxxxx xxx xxx xxxxxxxxxxxx.

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxxxxxx xxxxxxx xxxxxxxxxxxx
```
PS C:\>$VirtualMachine = Get-WAPackVM -Name "ContosoV126"
PS C:\> Remove-WAPackVM -VM $VirtualMachine -Force
```

Xxx xxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxx xxxxx XxxxxxxX000 xx xxxxx xxx Xxx$XXXxxxXX xxxxxx$ xxx xxxx xxxxxx xxxx xxxxxx xx xxx $XxxxxxxXxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxxxxx xxx xxxxxxx xxxxxxx xxxxxx xx $XxxxxxxXxxxxxx.
Xxxx xxxxxxx xxxxxxxx xxx Xxxxx xxxxxxxxx.
Xxx xxxxxxx xxxx xxx xxxxxx xxx xxx xxxxxxxxxxxx.

## XXXXXXXXXX

### -Force
Xxxxxxxxx xxxx xxx xxxxxx xxxxxxx x xxxxxxx xxxxxxx xxxxxxx xxxxxxxxx xxx xxx xxxxxxxxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Xxxxxxxxx xxxx xxx xxxxxx xxxxxxx x Xxxxxxx xxxxx.
Xx xxx xxxxxxxxx xxxxxxxx$ xxx xxxxxx xxxxxxx x xxxxx xx $Xxxx.
Xxxxxxxxx$ xx xxxxxxx x xxxxx xx $Xxxxx.
Xx xxxxxxx$ xxxx xxxxxx xxxx xxx xxxxxxxx xxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -VM
Xxxxxxxxx x xxxxxxx xxxxxxx.
Xx xxxxxx x xxxxxxx xxxxxxx$ xxx xxx Xxx$XXXxxxXX xxxxxx.

```yaml
Type: VirtualMachine
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: 
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Confirm
Xxxxxxx xxx xxx xxxxxxxxxxxx xxxxxx xxxxxxx xxx xxxxxx.Xxxxxxx xxx xxx xxxxxxxxxxxx xxxxxx xxxxxxx xxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Xxxxx xxxx xxxxx xxxxxx xx xxx xxxxxx xxxx.
Xxx xxxxxx xx xxx xxx.Xxxxx xxxx xxxxx xxxxxx xx xxx xxxxxx xxxx.
Xxx xxxxxx xx xxx xxx.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-WAPackVM](4b060a7d-da50-45ff-adb6-bcba63faa90b)

[New-WAPackVM](1f74deb4-e9b0-4aeb-8e13-b1554a4ebbec)

[Restart-WAPackVM](fd89742d-0d21-41e9-b3b1-5d8c638f8c6d)

[Resume-WAPackVM](d2594d2a-c0c6-4bca-8c81-9ed03b24d100)

[Set-WAPackVM](8b07e4cb-c677-4e6b-b034-25847da03dbf)

[Start-WAPackVM](8cc5bf6b-bf5b-427f-922d-57e4a99b2d55)

[Stop-WAPackVM](7f3e6c33-2196-4e24-95fd-e5763c6f7402)

[Suspend-WAPackVM](d8041113-5a71-447d-9bbe-dc6405aa6029)


