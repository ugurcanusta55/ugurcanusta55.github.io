`Servis URL:` https://api.wetrack.tech/<br>
`Methot URL:` "ats/ats/get_devices_last_signal" <br>
`Method Tip:` GET

???+ Açıklama

    Gönderilen filo id göre araç listesi ve anlık konumlarını dönen servis

## _Parametreler_

fleet_id

## _Response_

```
{
    "status_counts": {
        "total": 759,
        "move": 218,
        "park": 449,
        "idle": 42,
        "passive": 50
    },
    "data": {
        "type": "FeatureCollection",
        "crs": {
            "type": "name",
            "properties": {
                "name": "EPSG:4326"
            }
        },
        "features": [
            {
                "type": "Feature",
                "properties": {
                    "last_state": 1654094977,
                    "angle": 234,
                    "state": 0,
                    "speed": 93,
                    "mileage": 67296.112,
                    "first_ignition": 1654040177,
                    "last_ignition": 1654093029,
                    "ignition": true,
                    "sat": 15,
                    "extra_data": {
                        "speed_limit": {
                            "0": 120,
                            "1": 100,
                            "2": 90,
                            "4": 100
                        }
                    },
                    "max_speed": 133,
                    "daily_km": 809.56,
                    "address": "Ankara-Çankırı Otoyolu, Çubuk, Yozgat, Türkiye",
                    "info_data": {
                        "acc": true,
                        "gps": true,
                        "charge": true,
                        "defense": false,
                        "blockage": false,
                        "voltage_level": 6,
                        "gsm_signal_strength": 3
                    },
                    "id": 125,
                    "imei": "865784998844553",
                    "plate": "06TEST0606",
                    "driver_name": "",
                    "is_camera": null,
                    "vehicle_id": 123,
                    "engine_block": false,
                    "last_state_datetime": "01-06-2022 17:49:37",
                    "int_on": 5,
                    "int_off": 600,
                    "type": 2,
                    "blockage": null,
                    "icon_type": 0,
                    "vehicle_groups": "Adana TM Ara Hat 1",
                    "fullness": null,
                    "status": 0
                },
                "geometry": {
                    "type": "Point",
                    "coordinates": [
                        36.83821777777778,
                        37.197182222222224
                    ]
                }
            },
```
