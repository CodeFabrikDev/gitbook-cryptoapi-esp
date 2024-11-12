---
description: >-
  Genera un secreto TOTP para que el usuario configure la autenticación de dos
  factores.
---

# \[POST] /2fa/generate

El método \[POST]/2fa/generate genera un secreto TOTP (Time-Based One-Time Password) para el usuario, permitiéndole configurar la autenticación de dos factores (2FA) en su cuenta. El secreto TOTP es un código único que se puede escanear en aplicaciones de autenticación, como Google Authenticator o Authy, para generar códigos de autenticación temporales. Este proceso añade una capa adicional de seguridad, ya que requiere que el usuario introduzca un código de autenticación adicional al iniciar sesión, además de la contraseña, protegiendo la cuenta de accesos no autorizados.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

ejemplo:

```
{
  "userId": "user123"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
```
{% endtab %}
{% endtabs %}
