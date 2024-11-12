---
description: Comprueba el código de autenticación TOTP proporcionado por el usuario.
---

# \[POST] /2fa/verify

El método \[POST]/2fa/verify comprueba la validez de un código de autenticación TOTP (Time-Based One-Time Password) proporcionado por el usuario como parte del proceso de autenticación de dos factores (2FA). Al recibir el código temporal generado por una aplicación autenticadora (por ejemplo, Google Authenticator o Authy), el método confirma que el código es correcto y está dentro del tiempo de validez. Esta verificación añade una capa adicional de seguridad al proceso de inicio de sesión, garantizando que sólo los usuarios con acceso al dispositivo autenticador puedan completar el inicio de sesión y acceder a la cuenta.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

ejemplo:

```
{
  "userId": "user123",
  "token": "123456"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
```
{% endtab %}
{% endtabs %}
