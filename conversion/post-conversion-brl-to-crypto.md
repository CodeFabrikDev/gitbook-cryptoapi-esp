---
description: >-
  Convierte una cantidad en BRL(Real) a una cantidad equivalente en una
  criptomoneda específica.
---

# \[POST] /conversion/brl-to-crypto

El método \[POST] /conversion/brl-to-crypto convierte una cantidad en Real Brasileño (BRL) a la cantidad equivalente en una criptomoneda específica, como USDT (Tether). Esta funcionalidad es útil para usuarios y aplicaciones que desean conocer el precio aproximado de compra de criptodivisas en moneda local, facilitando las transacciones y la toma de decisiones en tiempo real basadas en cotizaciones de mercado.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

ejemplo:

```
{
  "amount": 100,
  "cryptoSymbol": "USDT",
  "networkId": 1,
  "networkName": "Ethereum"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "originalAmountInBrl": 100,
  "cryptoAmount": 17.2608,
  "cryptoSymbol": "USDT",
  "networkId": 1,
  "networkName": "Ethereum",
  "rateInfo": {
    "brlToUsdRate": 0.174,
    "cryptoToUsdRate": 1
  },
  "fee": "0.14",
  "finalAmountInUsd": "17.26"
}
```
{% endtab %}
{% endtabs %}
