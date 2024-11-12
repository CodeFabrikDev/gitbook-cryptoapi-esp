---
description: >-
  Obtener los tipos de transacción actuales para un par de divisas (base y
  cotización) de mempool.
---

# \[GET] /transaction-fee/pair

El método \[GET] /transaction-fee/pair obtiene las tarifas de transacción actuales para un par de divisas específico (divisa base y divisa cotizada) de mempool, donde las transacciones esperan ser procesadas en la red blockchain. Al especificar el par de divisas, como BTC/USDT o ETH/BRL, el método devuelve datos en tiempo real sobre las tarifas de transacción para las conversiones entre estas divisas, incluidas las tarifas medias, mínimas y máximas. Esta función es útil para usuarios y plataformas que quieran hacer un seguimiento de los costes de las transacciones entre pares específicos, lo que les permitirá ajustar sus operaciones en función de las condiciones de congestión y los costes actuales en la blockchain.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

Para comprobar el estado de una operación de conversión, basta con introducir el ID de la operación y hacer clic en «Execute».

#### Parámetros

<table><thead><tr><th width="364">Nombre</th><th>Descripción</th></tr></thead><tbody><tr><td>base</td><td>Código de la divisa base</td></tr><tr><td>quote</td><td>Código de moneda de cotización</td></tr></tbody></table>

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "base": {
    "currency": "BTC",
    "fastest_fee_usd": 8.49,
    "normal_fee_usd": 2.52,
    "slow_fee_usd": 7.77
  },
  "quote": {
    "currency": "ETH",
    "fastest_fee_usd": 4.28,
    "normal_fee_usd": 3.78,
    "slow_fee_usd": 3.04
  }
}
```
{% endtab %}
{% endtabs %}
