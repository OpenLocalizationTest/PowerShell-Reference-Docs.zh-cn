---
external help file: SMAzure_Compute.xml
online version: 4b060a7d-da50-45ff-adb6-bcba63faa90b
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# New-WAPackVM
## XXXXXXXX
Xxxxxxx x xxxxxxx xxxxxxx.

## XXXXXX

### UNNAMED_PARAMETER_SET_1
```
New-WAPackVM [-ProductKey <String>] [-VNet <VMNetwork>] -Name <String> -Template <VMTemplate>
 -VMCredential <PSCredential> [-Windows]
```

### UNNAMED_PARAMETER_SET_2
```
New-WAPackVM [-AdministratorSSHKey <String>] [-VNet <VMNetwork>] [-Linux] -Name <String> -Template <VMTemplate>
 -VMCredential <PSCredential>
```

### UNNAMED_PARAMETER_SET_3
```
New-WAPackVM [-VNet <VMNetwork>] -Name <String> -OSDisk <VirtualHardDisk> -VMSizeProfile <HardwareProfile>
```

## XXXXXXXXXXX
Xxxxx xxxxxx xxx xxxxxxxxxx xxx xxxx xx xxxxxxx xx xxx xxxxxx.
Xxx xxx xxxxxxx xxxxxx$ xxx  Xxxxx XXXxxx Xxxxxxxxxxx$$$xxxx.xxxxxxxxx.xxx$xxxxxxx$xx000000.xxxx.
Xxxx xxxxx xxxxxxxxx xxx xxxxxx xx xxx 0.0.0 xxxxxxx xx xxx Xxxxxxxxx Xxxxx XxxxxXxxxx xxxxxx.
Xx xxxx xxx xxx xxxxxxx xx xxx xxxxxx xxx$xx xxxxx$ xxxx xxx Xxxxx XxxxxXxxxx xxxxxxx$ xxxx $xxx$xxxxxx xxxxx$.xxxxxxx.

Xxx Xxx$XXXxxxXX xxxxxx xxxxxxx x xxxxxxx xxxxxxx.

## XXXXXXXX

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxxxxxx xxx xxx Xxxxxxx xxxxxxxxx xxxxxx xx xxxxx x xxxxxxxx
```
PS C:\>$Credentials = Get-Credential PS C:\> $Template = Get-WAPackVMTemplate -Name "ContosoTemplate04"PS C:\> New-WAPackVM -Name "ContosoV023" -Template $Template -VMCredential $Credentials -Windows
```

Xxx xxxxx xxxxxxx xxxxxxx x XXXxxxxxxxxx xxxxxx$ xxx xxxx xxxxxx xx xx xxx $Xxxxxxxxxxx xxxxxxxx.
Xxx xxxxxx xxxxxxx xxx xxx xx xxxxxxx xxx xxxxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxxx Xxx$Xxxx Xxx$Xxxxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxx xxxxxxxx xxxxx XxxxxxxXxxxxxxx00 xx xxxxx xxx Xxx$XXXxxxXXXxxxxxxx xxxxxx$ xxx xxxx xxxxxx xx xx xxx $Xxxxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxxxxx xxxxxxx xxxxx XxxxxxxX000$ xxxxx xx xxx xxxxxxxx xxxxxx xx xxx $Xxxxxxxx xxxxxxxx.
Xxx xxxxxxx xxxxxxxxx xxx Xxxxxxx xxxxxxxxx$ xxx$ xxxxxxxxx$ xxx xxxxxxx xxxxxxx xxxx xxx x xxxxxxx xx xxx Xxxxxxx xxxxxxxxx xxxxxx.

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxxxxxx xxx xxx Xxxxx xxxxxxxxx xxxxxx xx xxxxx x xxxxxxxx
```
PS C:\>$Credentials = Get-Credential PS C:\> $Template = Get-WAPackVMTemplate -Name "ContosoTemplate19"PS C:\> New-WAPackVM -Linux -Name "ContosoV028" -Template $Template -VMCredential $Credentials
```

Xxx xxxxx xxxxxxx xxxxxxx x XXXxxxxxxxxx xxxxxx$ xxx xxxx xxxxxx xx xx xxx $Xxxxxxxxxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxxxxx xxxxxxx xxxxxxxx xxxxx XxxxxxxXxxxxxxx00 xx xxxxx xxx Xxx$XXXxxxXXXxxxxxxx xxxxxx$ xxx xxxx xxxxxx xx xx xxx $Xxxxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxxxxx xxxxxxx xxxxx XxxxxxxX000$ xxxxx xx xxx xxxxxxxx xxxxxx xx xxx $Xxxxxxxx xxxxxxxx.
Xxx xxxxxxx xxxxxxxxx xxx Xxxxx xxxxxxxxx$ xxx$ xxxxxxxxx$ xxx xxxxxxx xxxxxxx xxxx xxx x xxxxxxx xx xxx Xxxxx xxxxxxxxx xxxxxx.

### Xxxxxxx 0$ Xxxxxx x xxxxxxx xxxxxxx xxxx xx xxxxxxxxx xxxxxx xxxx xxx xxxx xxxxxxx
```
PS C:\>$OSDisk = Get-WAPackVMOSDisk -Name "ContosoDiskOS"PS C:\> $SizeProfile = Get-WAPackVMSizeProfile -Name "MediumSizeVM"PS C:\> New-WAPackVM -Name "ContosoV073" -OSDisk $OSDisk -VMSizeProfile $SizeProfile
```

Xxx xxxxx xxxxxxx xxxx xx xxxxxxxxx xxxxxx xxxx xxxxx XxxxxxxXxxxXX xx xxxxx xxx Xxx$XXXxxxXXXXXxxx xxxxxx$ xxx xxxx xxxxxx xx xx xxx $XXXxxx xxxxxxxx.

Xxx xxxxxx xxxxxxx xxxx xxx xxxx xxxxxxx xxxxx XxxxxxXxxxXX xx xxxxx xxx Xxx$XXXxxxXXXxxxXxxxxxx xxxxxx$ xxx xxxx xxxxxx xx xx xxx $XxxxXxxxxxx xxxxxxxx.

Xxx xxxxx xxxxxxx xxxxxxx x xxxxxxx xxxxxxx xxxxx XxxxxxxX000 xxxx xxx xxxxxxxxx xxxxxx xxxx xxxxxx xx $XXXxxx xxx xxx xxxx xxxxxxx xxxxxx xx $XxxxXxxxxxx.

## XXXXXXXXXX

### -AdministratorSSHKey
Xxxxxxxxx xxx Xxxxxx Xxxxx $XXX$ xxx xxx xxx Xxxxxxxxxxxxx xxxxxxx.

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

### -Linux
Xxxxxxxxx xxxx xxx xxxxxx xxxxxxx x xxxxxxx xxxxxxx xx xxx xxx Xxxxx xxxxxxxxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Xxxxxxxxx x xxxx xxx xxx xxxxxxx xxxxxxx.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -OSDisk
Xxxxxxxxx xx xxxxxxxxx xxxxxx xxxx xx x XxxxxxxXxxxXxxx xxxxxx.
Xx xxxxxx xx xxxxxxxxx xxxxxx xxxx$ xxx xxx Xxx$XXXxxxXXXXXxxx xxxxxx.

```yaml
Type: VirtualHardDisk
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ProductKey
Xxxxxxxxx x xxxxxxx xxx.
Xxx xxxxxxx xxx xx x 00 xxxxx xxxxxx xxxx xxxxxxxxxx xxx xxxxxxx xxxxxxx.
Xxx x xxxxxxx xxx xxx xx xxxxxxxxx xxxxxx xxxx xxx xxxx xx xxxxxxx xx x xxxxxxx xxxxxxx xx xxxx.

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

### -Template
Xxxxxxxxx x xxxxxxxx.
Xxx xxxxxx xxxxxxx x xxxxxxx xxxxxxx xxxxx xx xxx xxxxxxxx xxxx xxx xxxxxxx.
Xx xxxxxx x xxxxxxxx xxxxxx$ xxx xxx Xxx$XXXxxxXXXxxxxxxx xxxxxx.

```yaml
Type: VMTemplate
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VMCredential
Xxxxxxxxx xxx xxxxxxxxxx xxx xxx xxxxx Xxxxxxxxxxxxx xxxxxxx.
Xx xxxxxx x XXXxxxxxxxxx xxxxxx$ xxx xxx Xxx$Xxxxxxxxxx xxxxxx.
Xxx xxxx xxxxxxxxxxx$ xxxx Xxx$Xxxx Xxx$Xxxxxxxxxx.

```yaml
Type: PSCredential
Parameter Sets: UNNAMED_PARAMETER_SET_1, UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VMSizeProfile
Xxxxxxxxx x xxxx xxxxxxx xxx x xxxxxxx xxxxxxx xx x XxxxxxxxXxxxxxx xxxxxx.
Xx xxxxxx x xxxx xxxxxxx$ xxx xxx Xxx$XXXxxxXXXxxxXxxxxxx xxxxxx.

```yaml
Type: HardwareProfile
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VNet
Xxxxxxxxx x xxxxxxx xxxxxxx.
Xxx xxxxxx xxxxxxxx xxx xxxxxxx xxxxxxx xx xxx xxxxxxx xxxxxxx xxxx xxx xxxxxxx.
Xx xxxxxx x xxxxxxx xxxxxxx$ xxx xxx Xxx$XXXxxxXXxx xxxxxx.

```yaml
Type: VMNetwork
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Windows
Xxxxxxxxx xxxx xxx xxxxxx xxxxxxx x xxxxxxx xxxxxxx xx xxx xxx Xxxxxxx xxxxxxxxx xxxxxx.

```yaml
Type: SwitchParameter
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## XXXXXX

## XXXXXXX

## XXXXX

## XXXXXXX XXXXX

[Get-WAPackVM](4b060a7d-da50-45ff-adb6-bcba63faa90b)

[Remove-WAPackVM](76b51795-43e6-45c3-ade1-aa8ea61efc23)

[Restart-WAPackVM](fd89742d-0d21-41e9-b3b1-5d8c638f8c6d)

[Resume-WAPackVM](d2594d2a-c0c6-4bca-8c81-9ed03b24d100)

[Set-WAPackVM](8b07e4cb-c677-4e6b-b034-25847da03dbf)

[Start-WAPackVM](8cc5bf6b-bf5b-427f-922d-57e4a99b2d55)

[Stop-WAPackVM](7f3e6c33-2196-4e24-95fd-e5763c6f7402)

[Suspend-WAPackVM](d8041113-5a71-447d-9bbe-dc6405aa6029)

[Get-WAPackVMSizeProfile](6dd436e0-b366-4a6b-adde-0aa6cdbfc3c6)

[Get-WAPackVMTemplate](1b16012f-1da0-42f0-8407-1601cf4168e8)

[Get-WAPackVMOSDisk](31ae72c2-c1d7-4c8d-b8be-61a46bfd6289)

[Get-WAPackVNe](3a6cfd0e-530b-42fb-a105-179559e91f3d)


