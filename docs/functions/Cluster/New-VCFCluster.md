# New-VCFCluster

### Synopsis
Connects to the specified SDDC Manager & creates cluster.

### Syntax
```
New-VCFWorkloadDomain -json <path to json file>
```

### Description
The New-VCFCluster cmdlet connects to the specified SDDC Manager & creates a cluster in a specified workload domains.

### Examples
#### Example 1
```
New-VCFCluster -json .\WorkloadDomain\addClusterSpec.json
```
This example shows how to create a cluster in a Workload Domain from a json spec

### Parameters

#### -json
- Path to the JSON spec

```yaml
Type: JSON
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
```

### Sample JSON
```
{
  "nsxVClusterSpec": {
    "vdsNameForVxlanConfig": "w01-c02-vds02",
    "vlanId": 0
  },
  "hostSpec": {
    "hostSystemSpec": [
      {
        "license": "AAAAA-AAAAA-AAAAA-AAAAA-AAAAA",
        "id": "c2398611-23cd-4b94-b2e3-9d84848b73cb",
        "vmnicToVdsNameMap": {
             "vmnic0": "w01-c02-vds01",
             "vmnic1": "w01-c02-vds01",
             "vmnic2": "w01-c02-vds02",
             "vmnic3": "w01-c02-vds02"
            }
      },
      {
        "license": "AAAAA-AAAAA-AAAAA-AAAAA-AAAAA",
        "id": "8dbe7dcb-f409-4ccd-984b-711e70e9e767",
        "vmnicToVdsNameMap": {
             "vmnic0": "w01-c02-vds01",
             "vmnic1": "w01-c02-vds01",
             "vmnic2": "w01-c02-vds02",
             "vmnic3": "w01-c02-vds02"
            }
      },
      {
        "license": "AAAAA-AAAAA-AAAAA-AAAAA-AAAAA",
        "id": "e9ba66e0-4670-4973-bdb1-bc05702ca91a",
        "vmnicToVdsNameMap": {
             "vmnic0": "w01-c02-vds01",
             "vmnic1": "w01-c02-vds01",
             "vmnic2": "w01-c02-vds02",
             "vmnic3": "w01-c02-vds02"
            }
      }
    ]
  },
  "clusterName": "c02",
  "highAvailabilitySpec": {
    "enabled": true
  },
  "domainId": "983840c1-fa13-4edd-b3cb-907a95c29652",
  "datastoreSpec": {
    "vsanDatastoreSpec": {
      "license": "BBBBB-BBBBB-BBBBB-BBBBB-BBBBB",
      "ftt": 1,
      "name": "w01-c02-vsan01"
    }
  },
  "vdsSpec": [
    {
      "name": "w01-c02-vds01",
      "portGroupSpec": [
        {
          "name": "w01-c02-vds01-management",
          "transportType": "MANAGEMENT"
        },
        {
          "name": "w01-c02-vds01-vmotion",
          "transportType": "VMOTION"
        },
        {
          "name": "w01-c02-vds01-vsan",
          "transportType": "VSAN"
        }
      ]
    },
    {
       "name": "w01-c02-vds02",
       "portGroupSpec": [
        {
          "name": "w01-c02-vds02-ext",
          "transportType": "PUBLIC"
        }
        ]
    }
  ]
}

```

### Notes

### Related Links
