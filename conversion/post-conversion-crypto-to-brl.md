---
description: Convierte una cantidad específica de criptomoneda a BRL
---

# \[POST] /conversion/crypto-to-brl

El método \[POST] /conversion/crypto-to-brl convierte una cantidad específica de una criptomoneda, como BTC (Bitcoin) o USDT (Tether), al valor equivalente en BRL (real brasileño). Cuando usted proporciona la cantidad deseada de criptomoneda, el método devuelve el valor correspondiente en BRL, basado en la tasa de mercado actual. Esta función es útil para las aplicaciones que necesitan mostrar el valor de las criptomonedas en moneda local, ayudando a los usuarios a visualizar el valor de sus activos digitales en BRL, lo que facilita las transacciones, los cálculos y la toma de decisiones financieras.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

ejemplo:

```
{
  "cryptoAmount": 0.5,
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
  "cryptoAmount": 0.5,
  "equivalentBrl": "2.85",
  "fee": "0.00",
  "finalAmountInUsd": "0.50",
  "cryptoSymbol": "USDT",
  "networkId": 1,
  "networkName": "Ethereum",
  "rateInfo": {
    "brlToUsdRate": 0.174,
    "cryptoToUsdRate": 1
  }
}
```
{% endtab %}
{% endtabs %}
