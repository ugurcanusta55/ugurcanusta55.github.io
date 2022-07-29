`Servis URL:` https://api.wetrack.tech/<br>
`Method URL:` "ats/report/get_report" <br>
`Method Tip:` POST

???+ Açıkalam

    Girilen tarih aralığında istenilen araçların mesai dışı km raporunu dönen servis.

## _Parametreler_

```
{
    "data": {
        "params": {
            "start_date": "1.06.2022",
            "end_date": "1.06.2022",
            "vehicles": [
                {
                    "value": 123
                }
            ],
            "report": 7
        },
        "page": 1,
        "limit": 10
    },
    "fleet_id": 1
}
```

## _Response_

```
{
    "data": [
        {
            "vehicle_id": 123,
            "plate": "06TEST0606",
            "driver_name": "",
            "_date": "01.06.2022",
            "out_shift_mileage": "270.39",
            "out_shift_time": 12659,
            "out_shift_idling_time": 0,
            "in_shift_mileage": "511.83",
            "in_shift_time": 28633,
            "in_shift_idling_time": 0,
            "_out_shift_first_ignition_on": "01.06.2022 02:36:17",
            "_out_shift_last_ignition_off": "01.06.2022 06:00:15",
            "_first_ignition_on": null,
            "_last_ignition_off": null
        }
    ],
    "count": 1,
    "data_count": 1,
    "status": true
}
```
