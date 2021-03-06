# Connect-VCFManager

### Synopsis
Connect to a VCF SDDC Manager

### Syntax
```
Connect-VCFManager -fqdn <String> -Username <String> -Password <String>
```

### Description
Connect to the SDDC Manager and stores the credentials in a base64 string.
It is required once per session before running all other cmdlets.

### Examples
#### Example 1
```
Connect-VCFManager -fqdn sfo01vcf01.sfo.rainpole.local -username admin -password VMware1!
```
This example shows how to connect to SDDC Manager

### Parameters

#### -fqdn
VCF SDDC Manager to connect to

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

#### -Username
Username to connect with
Currently supported with VCF admin account only

```yaml
Type: String
Parameter Sets: Username
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

#### -Password
Password to connect with

```yaml
Type: SecureString
Parameter Sets: Password
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### Notes

### Related Links
