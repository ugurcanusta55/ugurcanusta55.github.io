## Güvenli Sürüş

`Servis URL:` https://api.wetrack.tech/<br>
`Method URL:` "ats/ats/get_report_data" <br>
`Method Tip:` POST

???+ Açıklama

    Girilen tarih aralığındaki istenilen araçların Güvenli sürüş ihlallerini dönen servis

## _Parametreler_

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
        "report": 14,
        "server_side": true
    },
    "page": 1,
    "limit": 10
}
}
```

## _Response_

```
    "count": 95,
    "data_count": 95,
    "data": [
        {
            "vehicle__plate": "06TEST0606",
            "driver": "",
            "vehicle_id": 999,
            "movement": "Keskin_Donus",
            "created_date": "2022-06-01 14:16:23",
            "address": "Ankara Çevre Yolu, Kazan, Çankırı, Türkiye",
            "lat": "38.37743111",
            "lng": "38.25875111",
            "speed": 21
        },

```
