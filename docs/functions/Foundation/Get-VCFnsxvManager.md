# Get-VCFnsxvManager

### Synopsis
Gets a list of NSX-v Managers

### Syntax
```
Get-VCFnsxvManager -id <string>
```

### Description
Retrieves a list of NSX-v Managers managed by the connected SDDC Manager

### Examples
#### Example 1
```
Get-VCFnsxvManager
```
This example shows how to get the list of NSX-v Managers managed by the connected SDDC Manager

#### Example 2
```
Get-VCFnsxvManager -id d189a789-dbf2-46c0-a2de-107cde9f7d24
```
This example shows how to return the details for a specic NSX-v Manager managed by the connected SDDC Manager

#### Example 3
```
Get-VCFnsxvManager | select fqdn
```
This example shows how to get the list of NSX-v Managers managed by the connected SDDC Manager but only return the fqdn

### Parameters

#### -id
- ID of a specific VCF NSX-V Manager

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
```

### Notes

### Related Links
