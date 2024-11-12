---
description: Registrar un nuevo webhook asociado a una transacción de retirada específica
---

# \[POST] /webhook/register

El método \[POST] /webhook/register permite registrar un nuevo webhook asociado a una transacción de retirada específica. Al configurar el webhook, el usuario puede recibir notificaciones en tiempo real sobre el estado de una transacción de retirada, como confirmaciones, procesamiento o finalización. Esta funcionalidad es ideal para desarrolladores y plataformas que quieran monitorizar automáticamente el progreso de las transacciones e integrar notificaciones instantáneas en sus sistemas, facilitando el seguimiento y la automatización de acciones relacionadas con las retiradas de criptodivisas.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

ejemplo:

```
{
  "url": "https://meusite.com/webhook",
  "transactionId": "TX123456"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "id": 1,
  "url": "https://meusite.com/webhook",
  "transactionId": "TX123456"
}
```
{% endtab %}
{% endtabs %}
