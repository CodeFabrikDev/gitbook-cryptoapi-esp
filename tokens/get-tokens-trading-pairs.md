---
description: >-
  Obtendrá una lista de todos los pares de divisas que pueden negociarse, con un
  filtro opcional para las divisas base y cotizadas.
---

# \[GET] /tokens/trading-pairs

El método \[GET] /transaction-status/conversion devuelve la lista completa de todos los pares de divisas disponibles para operar, con la opción de aplicar filtros para divisas base y cotizadas. Al proporcionar parámetros como la divisa base (por ejemplo, BTC, USDT) o la divisa cotizada (como BRL o USD), los usuarios pueden refinar la consulta para obtener sólo los pares que satisfagan sus necesidades específicas. Esta función es esencial para las plataformas de intercambio y negociación de criptomonedas, ya que permite a los operadores y desarrolladores acceder a información actualizada sobre los pares de divisas disponibles y realizar transacciones de forma más eficiente y personalizada.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

Para filtrar la lista de todos los pares de divisas con los que se puede operar, basta con introducir la divisa base y la divisa de cotización y, a continuación, hacer clic en «Ejecutar»; si desea ver la lista completa, basta con dejarla en blanco.

#### Parámetros

| Nombre | Descripción                                             |
| ------ | ------------------------------------------------------- |
| base   | Divisa base para filtrar los pares de negociación       |
| quote  | Cotización de divisas para filtrar pares de negociación |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
[
  {
    "id": "BAT-ETH",
    "base_currency": "BAT",
    "quote_currency": "ETH",
    "display_name": "BAT-ETH",
    "status": "online",
    "trading_disabled": false
  },
  {
    "id": "SYLO-USD",
    "base_currency": "SYLO",
    "quote_currency": "USD",
    "display_name": "SYLO-USD",
    "status": "delisted",
    "trading_disabled": true
  },
  {
    "id": "COMP-USD",
    "base_currency": "COMP",
    "quote_currency": "USD",
    "display_name": "COMP-USD",
    "status": "online",
    "trading_disabled": false
  },
  {
    "id": "ARKM-USD",
    "base_currency": "ARKM",
    "quote_currency": "USD",
    "display_name": "ARKM/USD",
    "status": "online",
    "trading_disabled": false
  }
  ]
```
{% endtab %}
{% endtabs %}
