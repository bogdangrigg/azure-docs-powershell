---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: CE6E1BD4-E1CE-4AFC-8AE6-EECCEAE116B3
---

# Get-AzureApplicationGatewaySslCertificate

## SYNOPSIS
Gets application gateway certificates.

## SYNTAX

```
Get-AzureApplicationGatewaySslCertificate [-Name] <String> [[-CertificateName] <String>]
 [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureApplicationGatewaySslCertificate** cmdlet gets Secure Sockets Layer (SSL) certificates for an application gateway.

## EXAMPLES

### Example 1: Get an SSL certificate
```
PS C:\>Get-AzureApplicationGatewaySslCertificate -Name "ApplicationGateway08" -CertificateName "SslCertificate13"
```

This command gets an SSL certificate named SslCertificate13 on the application gateway named ApplicationGateway08.

### Example 2: Get all SSL certificates
```
PS C:\>Get-AzureApplicationGatewaySslCertificate -Name "ApplicationGateway08"
```

This command gets all the SSL certificates on the application gateway named ApplicationGateway08.

## PARAMETERS

### -Name
Specifies the name of the application gateway from which this cmdlet gets an SSL certificate.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -CertificateName
Specifies the name of an SSL certificate.
This cmdlet gets the certificate that this parameter specifies.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### Microsoft.Azure.Networking.ApplicationGatewayObjectModel.ApplicationGatewayCertificate, List<Microsoft.Azure.Networking.ApplicationGatewayObjectModel.ApplicationGatewayCertificate>

## NOTES

## RELATED LINKS

[Add-AzureApplicationGatewaySslCertificate](./Add-AzureApplicationGatewaySslCertificate.md)

[Remove-AzureApplicationGatewaySslCertificate](./Remove-AzureApplicationGatewaySslCertificate.md)


