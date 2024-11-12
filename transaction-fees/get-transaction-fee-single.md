---
description: >-
  Obtenga las tarifas de transacción actuales para una divisa específica en
  mempool.
---

# \[GET] /transaction-fee/single

El método \[GET] /transaction-fee/single muestra las tarifas de transacción actuales para una moneda específica en el mempool, que es el conjunto de transacciones pendientes a la espera de confirmación en la red blockchain. Al consultar las tarifas de una moneda específica, como BTC o ETH, el método devuelve información en tiempo real sobre las tarifas medias, mínimas y máximas, lo que ayuda a los usuarios a ajustar sus transacciones para una confirmación más rápida o tarifas más baratas. Esta funcionalidad es esencial para los usuarios y las plataformas que desean optimizar el coste y la velocidad de sus transacciones proporcionando datos precisos y actualizados sobre la congestión y el coste de las transacciones en la red blockchain elegida.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

Para comprobar el tipo de cambio de una divisa, basta con introducir la divisa y hacer clic en «Execute».

#### Parámetros

| Nombre   | Descripción                 |
| -------- | --------------------------- |
| currency | Código de la red Blockchain |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "currency": "BTC",
  "fastest_fee_usd": 9.71,
  "normal_fee_usd": 2.52,
  "slow_fee_usd": 4.49
}
```
{% endtab %}
{% endtabs %}
