## Alan Giriş Çıkış

# Araç Grupları Listesi

`Servis URL:` https://api.wetrack.tech/<br>
`Method URL:` "ats/ats/vehicle_group_list" <br>
`Method Tip:` GET

- Parametreler <br>
  \*Fleet_id

???+ Açıklama

    Araç ve poi gruplarını dönen servis.

- <strong>_Response_

```
[
    {
        "value": 11,
        "label": "Ankara TM Ara Hat 1",
        "vehicles": [
            {
                "label": "06TEST0606",
                "value": 123
            }
        ]
    }...
```

# Grup Noktaları Listesi

`Servis URL:` https://api.wetrack.tech/<br>
`Method URL:` "ats/ats/get_group_all_points" <br>
`Method Tip:` POST

???+ Açıklama

      Gönderilen poi grubunun  noktalarını dönen servis.

Parametreler

```
{
    "fleet_id": 1,
    "group_id": "11"
}
```

- _Response_

```
{
    "points": [
        {
            "id": 1234,
            "index": 1,
            "name": "ACIGOL",
            "radius": 500.0,
            "deflection": null,
            "location": [
                34.4949846105891,
                38.54689113077168
            ]
        }...
```

# Alan Giriş-Çıkış Raporu

`Servis URL:` https://api.wetrack.tech/<br>
`Method URL`: "ats/ats/detailed_area_entrance_exitance_report" <br>
`Method Tip`: POST

???+ Açıklama

      Girilen tarih aralığında istenilen noktalar ve araçların girdiği alanları dönen  servis

- Parametreler

```
  "sort": [
    {
      "field": "vehicle_plate",
      "type": "asc"
    },
    {
      "field": "enter_date",
      "type": "asc"
    }
  ],
  "page": 1,
  "limit": 100,
  "start_date": 1654030800,
  "end_date": 1654117140,
  "vehicles": "211,499,510,572,578",
  "points": "1072,850,1065,1016,1048,1009,1042,1034,1026,1055,1040,1051,1054,1023,1062,1053,1007,1024,1047,1039,1064,1056,1030,1031,1059,1058,1077,1081,1083,1019,1015,1028,1002,1012,1084,1022,1032,1086,1017,1038,1043,1085,1074,1049,1050,1018,1046,1075,1035,1052",
  "fleet_id": 1
}
```

- <strong>_Response_

```
{
    "status": true,
    "activity_count": 24,
    "activities": [
        {
            "index": 1,
            "vehicle_id": 123,
            "vehicle_plate": "01TEST0101",
            "point_id": 999,
            "point_name": "Adana TM",
            "enter_date": "01-06-2022 02:49:34",
            "exit_date": "01-06-2022 03:17:12",
            "voyage_id": null,
            "area_log_ids": [
                25444,
                25448
            ]
        }...
```

```
{
  "sort": [
    {
      "field": "vehicle_plate",
      "type": "asc"
    },
    {
      "field": "enter_date",
      "type": "asc"
    }
  ],
  "page": 1,
  "limit": 100,
  "start_date": 1654030800,
  "end_date": 1654117140,
  "vehicles": "211,499,510,572,578",
  "points": "1072,850,1065,1016,1048,1009,1042,1034,1026,1055,1040,1051,1054,1023,1062,1053,1007,1024,1047,1039,1064,1056,1030,1031,1059,1058,1077,1081,1083,1019,1015,1028,1002,1012,1084,1022,1032,1086,1017,1038,1043,1085,1074,1049,1050,1018,1046,1075,1035,1052",
  "fleet_id": 1
}
```
