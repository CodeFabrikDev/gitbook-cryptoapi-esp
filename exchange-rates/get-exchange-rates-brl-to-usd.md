---
description: >-
  Obtener el tipo de cambio del real brasileño (BRL) frente al dólar
  estadounidense (USD)
---

# \[GET] /exchange-rates/brl-to-usd

El método \[GET] /exchange-rates/brl-to-usd de nuestra API le permite comprobar el valor actual del real brasileño (BRL) frente al dólar estadounidense (USD). Este endpoint proporciona el tipo de cambio en tiempo real entre las dos monedas.

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
0.17271157167530224
```
{% endtab %}
{% endtabs %}
