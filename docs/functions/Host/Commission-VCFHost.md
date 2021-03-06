# Commission-VCFHost

### Synopsis
Connects to the specified SDDC Manager and commissions a list of hosts.

### Syntax
```
Commission-VCFHost -json <json file>
```

### Description
The Commission-VCFHost cmdlet connects to the specified SDDC Manager and commissions a list of hosts. Host list spec is provided in a JSON file.

### Examples
#### Example 1
```
Commission-VCFHost -json .\Host\commissionHosts\commissionHostSpec.json
```
This example shows how to commission a list of hosts based on the details provided in the JSON file.

### Parameters

#### -json
Path to the json spec

```yaml
Type: JSON
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
```

### Sample JSON
```json
[
        {
            "fqdn": "sfo01w01esx01.sfo.rainpole.local",
            "username": "root",
            "storageType": "VSAN",
            "password": "VMw@re1!",
            "networkPoolName": "sfo01w01-cl01",
			"networkPoolId": "1cb5a82e-b1b0-4d98-9d99-544a22875584"
        },
        {
            "fqdn": "sfo01w01esx02.sfo.rainpole.local",
            "username": "root",
            "storageType": "VSAN",
            "password": "VMw@re1!",
            "networkPoolName": "sfo01w01-cl01",
			"networkPoolId": "1cb5a82e-b1b0-4d98-9d99-544a22875584"

        },
		{
            "fqdn": "sfo01w01esx03.sfo.rainpole.local",
            "username": "root",
            "storageType": "VSAN",
            "password": "VMw@re1!",
            "networkPoolName": "sfo01w01-cl01",
			"networkPoolId": "1cb5a82e-b1b0-4d98-9d99-544a22875584"
        },
		{
            "fqdn": "sfo01w01esx04.sfo.rainpole.local",
            "username": "root",
            "storageType": "VSAN",
            "password": "VMw@re1!",
            "networkPoolName": "sfo01w01-cl01",
			"networkPoolId": "1cb5a82e-b1b0-4d98-9d99-544a22875584"
        }
    ]

```

### Notes

### Related Links
