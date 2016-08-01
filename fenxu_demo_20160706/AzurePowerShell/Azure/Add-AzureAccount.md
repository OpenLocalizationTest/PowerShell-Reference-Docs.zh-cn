---
external help file: Microsoft.WindowsAzure.Commands.Profile.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=397618
schema: 2.0.0
---

# Add-AzureAccount
## SYNOPSIS
Adds the Azure account to Windows PowerShell

## SYNTAX

### User (Default)
```
Add-AzureAccount [-Environment <String>] [-Credential <PSCredential>] [-Tenant <String>]
 [-Profile <AzureSMProfile>]
```

### ServicePrincipal
```
Add-AzureAccount [-Environment <String>] -Credential <PSCredential> [-ServicePrincipal] -Tenant <String>
 [-Profile <AzureSMProfile>]
```

## DESCRIPTION
The Add-AzureAccount cmdlet makes your Azure account and its subscriptions available in Windows PowerShell.
It's like logging into your Azure account in Windows PowerShell.
To log out of the account, use the Remove-AzureAccount cmdlet.

Add-AzureAccount downloads information about your Azure account and saves it in a subscription data file in your roaming user profile.
It also gets an access token that allows Windows PowerShell to access your Azure account on your behalf.
When the command completes, you can manage your Azure account in Windows PowerShell.

There are two different ways to make your Azure account available to Windows PowerShell.
You can use the Add-AzureAccount cmdlet, which uses Azure Active Directory (Azure AD) authentication access tokens, or Import-AzurePublishSettingsFile, which uses a management certificate.
For guidance on which method to use, see "How to: Connect to your subscription" (http://azure.microsoft.com/en-us/documentation/articles/install-configure-powershell/#Connect).

When you run Add-AzureAccount, it displays an interactive window that prompts you to sign into your Azure account.
This sign-in is valid until the access token expires.
When it expires, cmdlets that require access to your account prompt you to run Add-AzureAccount again.

If you have a Microsoft Organizational account, you can use the -Credential parameter to add the subscriptions associated with your account to Windows PowerShell without an interactive dialog.

When specifying -ServicePrincipal switch a -Credential parameter is used to authenticate a Service Principal.

## EXAMPLES

### --------------------------  Example 1: Add an account  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>Add-AzureAccount
```

This command adds an Azure account to Windows PowerShell.
When you run the command, a windows pops up to request the user name and password of the account.

### --------------------------  Example 2: Use an alternate subscription data file  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>Add-AzureAccount -SubscriptionDataFile C:\Testing\SDF.xml
```

This command uses the SubscriptionDataFile parameter to direct Add-AzureAccount to store the account data in the C:\Testing\SDF.xml file, instead of the default file.

### --------------------------  Example 3: Add a Microsoft Organizational account using Credential  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>$credential = Get-Credential
          PS C:\>Add-AzureAccount -Credential $credential
```

This command uses the Credential parameter to provide AAD authentication information on the command line, rather than using the pop-up dialog for AAD authentication.

### --------------------------  Example 4: Add a Service Principal account using Credential and ServicePrincipal  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>$credential = Get-Credential
          PS C:\>Add-AzureAccount -Credential $credential -ServicePrincipal -Tenant "3EB32C56-E1E5-46A6-9410-F4A0572B3998"
```

This command uses the Credential parameter to provide AAD authentication information of the Service Principal in the tenant 3EB32C56-E1E5-46A6-9410-F4A0572B3998.

### --------------------------  Example 5: Add an account in Azure China  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>Add-AzureAccount -Environment AzureChinaCloud
```

This command uses the Environment parameter to add an Azure China account to Windows PowerShell.
When you run the command, a windows pops up to request the user name and password of the account.

## PARAMETERS

### -Environment
Specifies the Azure environment.
Valid values are: AzureCloud, AzureChinaCloud, AzureUSGovernment.
The default is AzureCloud.
This parameter is optional.

An Azure environment an independent deployment of Microsoft Azure, such as AzureCloud for global Azure, AzureChinaCloud for Azure operated by 21Vianet in China, and AzureUSGoverment for the Azure US Government Cloud.
You can also create on-premises Azure environments by using Azure Pack and the WAPack cmdlets.
For more information, see Azure Pack.
To get the available Azure environments, use the Get-AzureEnvironment cmdlet.
To add an environment, use the Add-AzureEnvironment cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential
The username and password account credentials used to authenticate with Azure Active Directory. 
The credentials must be for a Microsoft Organizational account or Service Principal, not a Microsoft account.

```yaml
Type: PSCredential
Parameter Sets: User
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: PSCredential
Parameter Sets: ServicePrincipal
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
The Profile to add accounts and subscriptions to. 
If not specified, adds accounts and subscriptions to the default (on disk) profile.

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: Default on-disk Profile
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServicePrincipal
Specifies that your are logging in as a service principal.
You must give a Credentials parameter for this case, with the service principal ID as the user name and the service principal key as the password.

```yaml
Type: SwitchParameter
Parameter Sets: ServicePrincipal
Aliases: 

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tenant
Used when logging in as a service principal.
Specifies the AAD tenant the service principal is defined in.
This can be either the tenant's domain name or id.

```yaml
Type: String
Parameter Sets: User
Aliases: TenantId

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: ServicePrincipal
Aliases: TenantId

Required: True
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### None

## OUTPUTS

### None

## NOTES
Add-AzureAccount (and the Azure AD authentication method) takes precedence over Import-AzurePublishSettings (and the management certificate method).
If you use Add-AzureAccount even once on your account, the Azure AD authentication method is used and the management certificate is ignored.
To remove the Azure AD token and restore the management certificate method, use the Remove-AzureAccount cmdlet.
For more information, type: Get-Help Remove-AzureAccount.

Keywords: azure, azuresm, servicemanagement, management, service, profile, common, login, account

## RELATED LINKS

[Add-AzureEnvironment]()

[Get-AzureEnvironment]()

[Import-AzurePublishSettingsFile]()

[Get-AzureAccount]()

[Remove-AzureAccount]()

