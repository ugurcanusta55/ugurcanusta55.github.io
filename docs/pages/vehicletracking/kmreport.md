`Servis URL:` https://api.wetrack.tech/<br>
`Method Url:` <bold>"ats/ats/get_report_data"</bold> <br>
`Method Tipi:` <bold>POST</bold>

???+ Açıklama

    Girilen tarih aralığındaki istenilen araçların km bilgilerini dönen servis

## _Request_

<strong>Parametreler</strong>

```
{
    "data": {
    "params": {
        "start_date": "1.06.2022 00:00",
        "end_date": "1.06.2022 23:59",
        "vehicles": [
            {
                "label": "06TEST0606",
                "value": 123
            },
            {
                "label": "34TEST3434",
                "value": 124
            }
        ],
        "report": 3,
        "server_side": true
    },
    "page": 1,
    "limit": 10
}
}
```

## _Response_

```
{
    "total_mileage_sum": 1135.0,
    "data_count": 1,
    "count": 1,
    "vehicles_not_found": [],
    "data": [
        {
            "vehicle__plate": "06TEST0606",
            "driver": "",
            "last_ignition": "01-06-2022 17:17:09",
            "started_date": "01.06.2022 02:37:24",
            "start_address": "Çankırı",
            "finished_date": "01.06.2022 17:16:57",
            "end_address": "Kahramanmaraş - Gaziantep yolu, Pazarcık, Kahramanmaraş, Türkiye",
            "start_km": 66487.0,
            "end_km": 67255.0,
            "total_distance": 769.0,
            "total_mileage_sum": 769.0,
            "vehicle_id": 123
        }
    ]
}
```
