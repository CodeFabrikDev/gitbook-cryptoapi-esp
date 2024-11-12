---
description: Lista todas las direcciones de depósito generadas para cada red blockchain
---

# \[GET] /deposit/list

El método \[GET] /deposit/list devuelve una lista de todas las direcciones de depósito generadas para cada red blockchain asociada a la cuenta del usuario. Proporciona una vista centralizada de las direcciones públicas, permitiendo a los usuarios ver fácilmente las direcciones específicas para cada red (como Bitcoin, Ethereum, entre otras) para las que pueden recibir depósitos. Esta funcionalidad es útil para las plataformas que gestionan múltiples criptodivisas y desean facilitar el seguimiento de las direcciones activas, garantizando que las transacciones se envíen a los lugares correctos de la red blockchain.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

Para listar todos los depósitos generados, basta con hacer clic en «Execute».

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
[
  {
    "networkId": 1,
    "networkName": "Ethereum",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "networkId": 2,
    "networkName": "Binance Smart Chain",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "networkId": 3,
    "networkName": "Polygon",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "networkId": 4,
    "networkName": "Avalanche",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  }
]
```
{% endtab %}
{% endtabs %}
