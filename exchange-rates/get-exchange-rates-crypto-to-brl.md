---
description: Obtener el tipo de cambio de una criptomoneda a BRL(Real)
---

# \[GET] /exchange-rates/crypto-to-brl

El método \[GET] /exchange-rates/crypto-to-brl permite obtener la cotización actual de una criptomoneda específica, como Bitcoin (BTC), en relación con el real brasileño (BRL). Consulta datos en tiempo real de los mercados financieros y devuelve el valor de conversión más reciente entre la criptomoneda y el BRL, lo que permite a las aplicaciones y a los usuarios seguir los cambios de precios y tomar decisiones informadas en sus transacciones.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

No hay, para obtener la tasa de una criptodivisa para BRL, basta con introducir el ID de la criptodivisa que desea (por ejemplo, BTC, ETH, etc.) y, a continuación, haga clic en «Execute».

#### Parámetros

| Nombre       | Descripción                |
| ------------ | -------------------------- |
| cryptoSymbol | Símbolo de la criptomoneda |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "symbol": "BTCBRL",
  "price": 475081.32000000007
}
```
{% endtab %}
{% endtabs %}
