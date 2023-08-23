![Washing Machine](pictures/iot-machine.png)

## Get hardware level operations e.g. wash_count

```
Topic: v1cdti/hw/get/6310301004/model-01/SN-001
Payload: {
   "action"    : "get",
    "project"   : "6310301004",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "wash_count",
    "value"     : "10"
}
```

## Get firmware version

```
Topic: v1cdti/hw/get/6310301004/model-01/SN-001
Payload: {
   "action"    : "get",
    "project"   : "6310301004",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "firmware",
    "value"     : "1.0"
}
```

## Get manufacture id and geo-location or location placement

```
Topic: v1cdti/hw/get/6310301004/model-01/SN-001
Payload: {
   "action"    : "get",
    "project"   : "6310301004",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "manufacture",
    "value"     : "10",
    "geo_lat" : "22.1234",
    "geo_lng": "-112.221"
}
```

## Set geo-location or location placement

```
Topic: v1cdti/hw/set/6310301004/model-01/SN-001
Payload: {
   "action"    : "set",
    "project"   : "6310301004",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "geo_lat" : "22.1234",
    "geo_lng": "-112.221"
}
```

## Monitor machine sensor

```
Topic: v1cdti/app/monitor/6310301004/model-01/SN-001
Payload: {
   "action"    : "monitor",
    "project"   : "6310301004",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "temperature",
    "value"     : "30",
}
```

## Set machie status to "maint" to indicate this machine need to be maintenance.

```
Topic: v1cdti/hw/set/6310301004/model-01/SN-001
Payload: {
   "action"    : "monitor",
    "project"   : "6310301004",
    "model"     : "model-01",
    "serial"    : "SN-001",
    "name"      : "status",
    "value"     : "maint",
}
