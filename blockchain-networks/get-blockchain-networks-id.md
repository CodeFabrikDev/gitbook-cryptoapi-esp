---
description: Obtener detalles de una red blockchain específica
---

# \[GET] /blockchain-networks/{id}

El método \[GET] /blockchain-networks/{id} de nuestra API le permite consultar información detallada sobre una red blockchain concreta, proporcionándole datos cruciales sobre su configuración, estado y características. Al introducir el ID de la red, recibirá un conjunto completo de información relativa a esa blockchain, incluidos parámetros técnicos, estado actual, tarifas de transacción, capacidad de procesamiento y mucho más.&#x20;

Este punto final es ideal para desarrolladores y plataformas que necesitan obtener detalles precisos sobre una red específica para llevar a cabo integraciones o supervisar el rendimiento de sus transacciones en tiempo real. También es útil para comprobar parámetros como el consenso, el tiempo medio de bloque, los métodos de validación y la compatibilidad con contratos inteligentes.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

Para ver los detalles de una de las redes disponibles, sólo tiene que introducir el ID de la red blockchain que desee y, a continuación, hacer clic en «Execute».

#### Parámetros

| Nombre | Descripción             |
| ------ | ----------------------- |
| id     | ID de la red Blockchain |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
```
{% endtab %}
{% endtabs %}
