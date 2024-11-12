---
description: Criação de carteira Blockchain
---

# \[POST] /wallet/create

O método **\[POST] /wallet/create** permite a criação de uma nova carteira em blockchain, vinculada à conta do usuário. A carteira gerada inclui um endereço público único, usado para armazenar e transacionar criptomoedas com segurança. Este endpoint facilita a gestão de ativos digitais ao criar automaticamente uma carteira que pode receber depósitos, realizar saques e monitorar saldos em tempo real. Ideal para plataformas que desejam fornecer carteiras individuais aos seus usuários, este método oferece um ponto de entrada seguro para começar a transacionar no blockchain de forma descentralizada e rastreável.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

No hay ninguna, basta con hacer clic en «Execute» para utilizar el método.

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "publicKey": "0x0ED99A476FCCeD2f609C80A312FDAFdeDEE85AA1"
}
```
{% endtab %}
{% endtabs %}
