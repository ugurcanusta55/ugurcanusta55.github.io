`Servis URL:` https://api.wetrack.tech/<br>
`Method URL:`"ats/ats/alarm_report_table"<br>
`Method Tip: ` POST

???+ Açıklama

    Girilen tariharalığında istenilen araçların park alarmlarını dönen servis

## _Parametreler_

```
{
    "fleet_id": 1,
    "data": {
        "limit": 10,
        "page": 1,
        "s_ts": 1654030800,
        "e_ts": 1654117140,
        "alarm_type": 4
    }
}
```

## _Response_

```
{
    "count": 3,
    "data": [
        {
            "plate": "06TEST0606",
            "alarm_type": 4,
            "created_date": "28/05/2022 22:33:47",
            "lat": "32",
            "lng": "23",
            "address": "Libya}",
            "id": 111111,
            "ignition": "",
            "content": "",
            "vehicle_id": 1
        }...
```
