## **Erişim**

Servis metotlarını kullanmak için, N2Mobil tarafından verilen kullanıcı adı ve şifre ile authentication yapılması gerekmektedir.

## **Güvenlik**

- Servis güvenliğini sağlamak için JSON Web Token (JWT) kullanılmaktadır. Authentication yapıldıktan sonra elde edilen “accessToken" servis metotları kullanılırken header bölümünde “Authorization” parametresinde gönderilmesi gerekmektedir.

  - Servise gelen istekler için Content-Type parametresi “application/json” olmalıdır.
  - İstekler JWT token kullanılarak gönderilmelidir.

## **API**

API, REST etrafında düzenlenmiştir. API'miz tahmin edilebilir kaynak odaklı URL'lere sahiptir, formla kodlanmış istek gövdelerini kabul eder, JSON kodlu yanıtları döndürür ve standart HTTP yanıt kodlarını, kimlik doğrulamasını ve fiilleri kullanır.
