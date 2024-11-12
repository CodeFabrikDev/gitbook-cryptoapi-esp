---
description: Genera una dirección de depósito específica para una red blockchain
---

# \[POST] /deposit/create

El método \[POST] /deposit/create genera una dirección de depósito única y específica para una red blockchain, lo que permite al usuario recibir criptomonedas de forma segura. Al solicitar la generación de una dirección, el sistema crea automáticamente una dirección pública válida para la red blockchain elegida (como Bitcoin, Ethereum u otras), que puede utilizarse para futuros depósitos. Esta función facilita la recepción de fondos al proporcionar una forma práctica y segura de gestionar las transacciones entrantes, garantizando que los depósitos se envían a la dirección correcta de la red blockchain.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

Para generar una dirección de depósito, basta con introducir el ID de red y pulsar «Execute».

#### Parámetros

<table><thead><tr><th width="364">Nombre</th><th>Descripción</th></tr></thead><tbody><tr><td>networkId</td><td>ID de la red blockchain para la que se generará la dirección de depósito</td></tr></tbody></table>

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
```
{% endtab %}
{% endtabs %}
