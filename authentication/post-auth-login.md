---
description: Autenticarse y obtener un token JWT
---

# \[POST] /auth/login

El método \[POST] /auth/login autentica las credenciales del usuario y devuelve un token JWT (JSON Web Token) para el acceso seguro a otros puntos finales protegidos de la aplicación. Al enviar las credenciales de inicio de sesión, como el correo electrónico y la contraseña, el usuario recibe un token JWT válido, que puede utilizarse para la autenticación en llamadas posteriores, evitando la necesidad de volver a enviar las credenciales. El uso de JWT ofrece una forma segura y eficiente de gestionar las sesiones de usuario en aplicaciones distribuidas, garantizando que sólo los usuarios autenticados puedan acceder a los recursos sensibles durante el periodo de validez del token.

### Autorización

Bearer token permite autenticar las solicitudes mediante una clave de acceso, como un token web JSON (JWT). El token es una cadena de texto incluida en la cabecera de la solicitud.

```
Bearer <Your API token>
```

### Request Body

ejemplo:

```
{
  "username": "admin",
  "password": "password123"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6InNkdmFsZSIsInN1YiI6MSwiaWF0IjoxNzMxMzMwMTU1LCJleHAiOjE3MzEzNTg5NTV9.8SzGYaLV4rTzXA70Rx4AhKdSxku0STA06zUcRNvp9A2"
}
```
{% endtab %}
{% endtabs %}
