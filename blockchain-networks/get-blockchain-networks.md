---
description: Lista de todas las redes blockchain disponibles
---

# \[GET] /blockchain-networks

El método **\[GET] /blockchain-networks** de nuestra API le permite acceder y consultar las redes blockchain compatibles para la integración en su aplicación. Con este endpoint, puede obtener una lista completa de las principales redes blockchain disponibles para transacciones.

Este recurso es ideal para desarrolladores que buscan identificar las redes compatibles con su plataforma o aplicación, facilitando la elección de la blockchain más adecuada para el tipo de transacción o servicio que desean implementar. La API proporciona información detallada sobre cada red, como nombre, el ChainID (código de la red) y la dirección de depósito.&#x20;

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
    "name": "Ethereum",
    "chainId": "1",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "id": 2,
    "name": "Binance Smart Chain",
    "chainId": "56",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "id": 3,
    "name": "Polygon",
    "chainId": "137",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "id": 4,
    "name": "Avalanche",
    "chainId": "43114",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  }
]
```
{% endtab %}
{% endtabs %}
