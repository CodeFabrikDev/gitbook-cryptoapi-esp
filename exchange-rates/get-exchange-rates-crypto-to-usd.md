---
description: Obtener la tasa de una criptomoneda a USD(Dólar)
---

# \[GET] /exchange-rates/crypto-to-usd

El método \[GET] /exchange-rates/crypto-to-usd permite obtener el precio actual de una criptomoneda específica, como Bitcoin (BTC), en relación con el dólar estadounidense (USD). Consulta datos en tiempo real de los mercados financieros y devuelve el valor de conversión más reciente entre la criptomoneda y el USD, lo que permite a las aplicaciones y a los usuarios seguir las variaciones de precios y tomar decisiones informadas en sus transacciones.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

No hay ninguna, para obtener la cotización de una criptodivisa en USD, simplemente introduzca el ID de la criptodivisa que desee (por ejemplo, BTC, ETH, etc.) y, a continuación, haga clic en «Execute».

#### Parámetros

| Nombre       | Descripción                |
| ------------ | -------------------------- |
| cryptoSymbol | Símbolo de la criptomoneda |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "cryptoId": "bitcoin",
  "vsCurrency": "usd",
  "price": 82194
}
```
{% endtab %}
{% endtabs %}
