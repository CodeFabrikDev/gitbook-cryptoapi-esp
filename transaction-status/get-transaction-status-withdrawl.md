---
description: >-
  Comprueba el estado de una transacción de retirada de criptomoneda por ID de
  transacción
---

# \[GET] /transaction-status/withdrawl

El método \[GET] /transaction-status/withdrawl permite comprobar el estado de una transacción de retirada de criptomoneda utilizando el ID único de la transacción. Al proporcionar el ID, el método devuelve el estado actual de la retirada, indicando si la transacción se ha procesado, está en curso o si se ha producido algún error. Esta función es esencial para los usuarios que desean seguir el progreso de sus retiradas, ya que ofrece una visión clara y en tiempo real del estado de la transacción y garantiza una mayor transparencia y confianza en las operaciones financieras.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

Para comprobar el estado de una operación de conversión, basta con introducir el ID de la operación y hacer clic en «Execute».

#### Parámetros

<table><thead><tr><th width="364">Nombre</th><th>Descripción</th></tr></thead><tbody><tr><td>transactionId</td><td>ID de transacción de conversión para comprobar el estado</td></tr></tbody></table>

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "transactionId": "TX987654",
  "status": "Pending"
}
```
{% endtab %}
{% endtabs %}
