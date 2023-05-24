# oauth2-studies
Estudos sobre o framework OAuth 2.0

Para todos os fluxos abaixo, caso a applicação cliente necessite de um ID Token, basta incluir o escopo **`openid`** na lista de escopos na chamada do `/authorize`. Nesse caso estamos falando do Framework OpenID Connect

### Authorization Code Flow for Native Apps

![](nativeFlow.svg)


### Authorization Code Flow for Single-Page Apps

![](singlePageFlow.svg)

### Referências
* OAuth 2.0 Authorization Framework: https://datatracker.ietf.org/doc/html/rfc6749;
* PKCE Extension: https://datatracker.ietf.org/doc/html/rfc7636;
* OpenID Connect: https://openid.net/connect/.
