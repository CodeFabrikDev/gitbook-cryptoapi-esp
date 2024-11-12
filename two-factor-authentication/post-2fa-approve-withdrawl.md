---
description: >-
  Aprueba una solicitud de retirada comprobando el código de autenticación de
  dos factores.
---

# \[POST] /2fa/approve-withdrawl

El método \[POST]/2fa/approve-withdrawl permite aprobar una solicitud de retirada de fondos tras verificar el código de autenticación de dos factores (2FA) proporcionado por el usuario. Garantiza que el usuario no sólo ha iniciado la transacción, sino que también tiene acceso al dispositivo de autenticación, lo que añade una capa crítica de seguridad al proceso de retirada de fondos. Al validar el código temporal TOTP (Time-Based One-Time Password) u otro método 2FA, este método ayuda a proteger la cuenta contra retiradas no autorizadas, garantizando que sólo los usuarios autenticados puedan completar las transacciones financieras.

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
