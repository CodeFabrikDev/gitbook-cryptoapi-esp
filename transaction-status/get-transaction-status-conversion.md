---
description: >-
  Comprueba el estado de una transacción de conversión de divisas por ID de
  transacción
---

# \[GET] /transaction-status/conversion

El método \[GET] /transaction-status/conversion permite comprobar el estado de una transacción de conversión de criptomoneda utilizando el ID de transacción. Al proporcionar el ID de transacción único, el método devuelve información detallada sobre el progreso de la conversión, como si la transacción se ha completado, está pendiente o ha fallado. Esta función es útil para las plataformas que desean supervisar y proporcionar actualizaciones en tiempo real a los usuarios sobre el estado de sus conversiones de criptomoneda, ofreciendo transparencia y facilitando el seguimiento de los procesos financieros en curso.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

Para comprobar el estado de una operación de conversión, basta con introducir el ID de la operación y hacer clic en «Execute».

#### Parámetros

| Nombre        | Descripción                                              |
| ------------- | -------------------------------------------------------- |
| transactionId | ID de transacción de conversión para comprobar el estado |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "transactionId": "TX123456",
  "status": "Completed"
}
```
{% endtab %}
{% endtabs %}
