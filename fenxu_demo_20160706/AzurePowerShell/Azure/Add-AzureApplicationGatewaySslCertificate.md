---
External help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=397618
schema: 2.0.0
---

# Add-AzureApplicationGatewaySslCertificate
## SYNOPSIS
Adds ssl certificate to application gateway

## SYNTAX

```
Add-AzureApplicationGatewaySslCertificate [-Name] <String> [-CertificateName] <String> [-Password] <String>
 [-CertificateFile] <String> [-Profile <AzureSMProfile>]
```

## DESCRIPTION
The Add-AzureApplicationGatewaySslCertificate cmdlet adds the ssl certificate to an application gateway

## EXAMPLES

### --------------------------  Example 1  --------------------------
```
PS C:\> Add-AzureApplicationGatewaySslCertificate -Name "gatewayName" -CertificateName "sslCertificateName" -Password "xxxx" -CertificateFile "c:\Certs\sslCertificate.pfx"
```

Adding certificate using named parameters

### --------------------------  Example 2  --------------------------
```
PS C:\> Add-AzureApplicationGatewaySslCertificate "gatewayName" "sslCertificateName" "xxxx" "c:\Certs\sslCertificate.pfx"
```

Adding certificate using positional parameters

## PARAMETERS

### -Name
Name of application gateway

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -CertificateName
Name of ssl certificate that is being added

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Password
Password of ssl certificate

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -CertificateFile
Path of ssl certificate file

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
In-memory profile.

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### System.String

## OUTPUTS

### Microsoft.WindowsAzure.Management.ApplicationGateway.Models.ApplicationGatewayOperationResponse

## NOTES
Keywords: azure, azuresm, servicemanagement, management, service, network, networking

## RELATED LINKS

