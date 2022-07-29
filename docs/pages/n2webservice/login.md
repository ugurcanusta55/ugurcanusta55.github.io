# <strong>_Login_</strong>

Araç Takip Sistemi ;

[Postman Collection için](../../postman/n2mobil.postman_collection.json){ .md-button download="" }

Sisteme giriş için verilen kullanıcı adı ve şifre bilgisi ile giriş yapabilirsiniz.
Session bilgisi sisteme kayıt edilir ve bundan sonraki methodlarda bu session bilgisini kullanarak methodları kullanabilirsiniz.

!!! Hatırlatma

     Login zorunluluğu gerektiren metodlar için;

    Headers’a
    Authorization: JWT {{AUTH_TOKEN}}

    Şeklinde eklenmelidir.

## _Login Request_

`Servis URL:` https://api.wetrack.tech/<br>
`Method Url:` <bold>auth</bold> <br>
`Method Tipi:` <bold>POST</bold>

Servis metotlarına erişim için gerekli izinlerin alınmasını sağlar.

<strong>Parametreler</strong><br>
<strong>Request</strong>

```
{
    "username": "Username",
    "password": "Password"
}
```

## _Login Response_

```
{
"refresh": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9..... ",
    "access": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9...... ",
    "username": "Username",
    "profile_update": false,
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9..... ",
    "status": true,
    "profile": {
        "username": "Username”
        "email": "test@n2mobil.com.tr",
        "first_name": "",
        "last_name": "Test",
        "phone": "(500) 500-1508",
        "admin": false
    },
    "domain": "https://web.wetrack.tech/",
    "app_url": "https://web.wetrack.tech/api"
}
```
