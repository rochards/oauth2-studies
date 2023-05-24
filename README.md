# oauth2-studies
Estudos sobre o framework OAuth 2.0

### Authorization Code Flow for Native Apps

![](nativeFlow.svg)


### Authorization Code Flow for Single-Page Apps

![](singlePageFlow.svg)

### OpenID Connect

Para todos os fluxos acima, caso a applicação cliente necessite de um ID Token, basta incluir o escopo **`openid`** na lista de escopos na chamada do `/authorize`. Nesse caso estaríamos falando do Framework OpenID Connect. Ao realizar a chamada de troca do `code` pelo `access_token`, também virá um `id_token`. Ex.:
```JSON
{
    "token_type": "Bearer",
    "access_token": "Rs75hayasyasdfa...",
    "expires_in": 3600,
    "id_token": "eyJraWQioiJiRmxzzL2..."
}
```

### Referências
* OAuth 2.0 Authorization Framework: https://datatracker.ietf.org/doc/html/rfc6749;
* PKCE Extension: https://datatracker.ietf.org/doc/html/rfc7636;
* OpenID Connect: https://openid.net/connect/.
