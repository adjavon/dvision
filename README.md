# dvision
Python client for the DVID database

## Usage:

```
>>> dvid_hostname = "..."
>>> dvid_port = int
>>> data_instance = dvision.DVIDDataInstance("slowpoke3", 32788, "341", "groundtruth_pruned")
>>> data_instance[5022:5026, 3000:3002, 3200:3202]
array([[[586315, 586315],
        [586315, 586315]],

       [[586315, 586315],
        [586315, 586315]],

       [[372796, 586315],
        [372796, 586315]],

       [[372796, 372796],
        [372796, 372796]]], dtype=uint64)
>>> roi = dvision.DVIDRegionOfInterest("slowpoke3", 32788, "341", "seven_column_z_gte_5024")
>>> roi[5022:5026, 3000:3002, 3200:3202]
array([[[0, 0],
        [0, 0]],

       [[0, 0],
        [0, 0]],

       [[1, 1],
        [1, 1]],

       [[1, 1],
        [1, 1]]], dtype=uint8)
```
