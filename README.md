# V2Ray VLESS Heroku

## Visão geral

Este projeto é usado para instalar o <b>V2Ray WebSocket VLESS</b> no <b>Heroku</b>. Na medida do uso razoável, esta imagem não será banida devido a uma grande quantidade de recursos.

Uma vez instalado, o <b>V2Ray</b> sempre será executado com a versão mais recente sempre que o aplicativo for iniciado

## Instalação

### Passos

 1. Fork este projeto para sua própria conta do GitHub (nome de usuário é um `exemplo`)
 2. Modifique o nome do projeto, tome cuidado para não incluir as palavras-chave `v2ray` e `heroku` (o nome do projeto modificado usa demo como exemplo)
 3. Modifique o `README.md` e substitua `peterquill-starlord/V2Ray-VLESS-Heroku` pelo seu próprio conteúdo (como `exemplo/demonstração`)

> [![Implantar](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/peterquill-starlord/V2Ray-VLESS-Heroku)

 4. Volte para a página inicial do projeto e clique no link acima para instalar o `V2Ray`

### variáveis

Os nomes de variáveis ​​que precisam ser definidos durante a instalação são explicados a seguir.

| variável | valor padrão | descrição |
| :--- | :--- | :--- |
| ID | ad806487-2d26-4636-98b6-ab85cc8521f7 | ID mestre do usuário VLESS, usado para autenticação, no formato UUID |
| WSPATH | / | Caminho do protocolo HTTP usado pelo WebSocket |

## Acesso ao CloudFlare

Os dois métodos a seguir podem conectar o aplicativo ao <b>CloudFlare</b>, o que pode melhorar a velocidade até certo ponto.

 1. Vincule um nome de domínio ao aplicativo e conecte o nome de domínio ao [CloudFlare](https://dash.cloudflare.com/login)
 2. Proxy reverso por meio de <b>CloudFlare Workers</b>

## Atenção

 1. Por favor, não abuse deste projeto, existem muito poucos serviços gratuitos como <b>Heroku</b>, use e valorize
 2. Se estiver usando um nome de domínio para acessar o CloudFlare, considere ativar o TLS 1.3
 3. A maioria dos endereços IPv4 da AWS são bloqueados pelo Twitter
