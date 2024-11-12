---
description: >-
  Solicita una retirada de criptomoneda, que requiere un código de aprobación de
  dos factores.
---

# \[POST] /withdrawl/request

El método \[POST] /withdrawl/request permite solicitar una retirada de criptomoneda, requiriendo una confirmación adicional mediante un código de autenticación de dos factores (2FA) para garantizar la seguridad de la transacción. Al realizar la solicitud de retirada, el usuario debe proporcionar el código temporal generado por una aplicación autenticadora, como Google Authenticator o Authy, para validar la operación. Este proceso añade una capa adicional de protección, evitando retiradas no autorizadas y garantizando que sólo los usuarios autenticados puedan completar las transacciones de retirada.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

ejemplo:

```
{
  "address": "0xRecipientAddress123",
  "amount": 1.5,
  "networkId": 1,
  "coin": "USDT",
  "userId": "user123",
  "approvalCode": "b3b7c9b2-48d6-4f0b-8881-3f2cdb15a5e9"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
```
{% endtab %}
{% endtabs %}
