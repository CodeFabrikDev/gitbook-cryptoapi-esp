---
description: Obtener la cotización de un par de divisas específico
---

# \[GET] /exchange-rates/pair

El método \[GET] /exchange-rates/pair de nuestra API le permite comprobar el valor actual de un par de criptodivisas específico, como BTCUSD, ETHUSD, entre otros. Este endpoint proporciona información en tiempo real sobre el precio de varios pares de divisas, lo que le permite integrar datos de mercado directamente en su aplicación, plataforma de comercio electrónico o servicio financiero.&#x20;

Con esta función, es posible obtener el precio de un par de divisas específico en diferentes unidades de medida, como el valor en dólares estadounidenses (USD), euros (EUR) u otras monedas fiduciarias y digitales. El método devuelve información precisa sobre el precio de compra y venta, así como la variación del precio en un periodo determinado, lo que ayuda a tomar decisiones informadas sobre transacciones e inversiones.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

Para obtener una cotización para un par de divisas específico, simplemente introduzca el ID de la criptomoneda que desee (por ejemplo, bitcoin, ethereum, etc.) y la divisa contra la que se cotizará (por ejemplo, usd, brl) y, a continuación, haga clic en «Execute».

#### Parámetros

| Nombre     | Descripción                                   |
| ---------- | --------------------------------------------- |
| cryptold   | Cryptocurrency ID según CoinGecko             |
| vcCurrency | Moneda contra la que cotizará la criptomoneda |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "cryptoId": "bitcoin",
  "vsCurrency": "usd",
  "price": 82274
}
```
{% endtab %}
{% endtabs %}
