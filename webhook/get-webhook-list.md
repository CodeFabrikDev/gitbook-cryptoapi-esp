---
description: Devuelve una lista de todos los webhooks registrados
---

# \[GET] /webhook/list

El método \[GET] /webhook/list devuelve una lista completa de todos los webhooks registrados por el usuario.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

No hay ninguna, basta con hacer clic en «Execute» para utilizar el método.

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
[
  {
    "id": 1,
    "url": "https://meusite.com/webhook",
    "transactionId": "TX123456"
  }
]
```
{% endtab %}
{% endtabs %}
