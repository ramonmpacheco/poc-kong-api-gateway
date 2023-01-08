# POC-KONG-API-GATEWAY
## Kong API Gateway + docker-compose

<br>

> PARA SUBIR O AMBIENTE DOCKER
> 
> Rodar o kong_compose:
```docker-compose -f kong_compose.yml up```

> URL DO KONGA
>
> http://localhost:1337 (é preciso criar um usuário admin)
>
> * É possível usar o nome do container como hostname quando for especificar uma url em um novo serviço do konga

> EXEMPLO DE POST
> ROTA: ```localhost:80/api/bets```

> HEADERS:
>~~~
> Content-Type | application/json
> Host         | bets-app.com.br
> ~~~

> BODY:
>~~~json
>{
>    "match": "1X-DC",
>    "email": "john@doe.com",
>    "championship": "Uefa Champions League",
>    "awayTeamScore": "2",
>    "homeTeamScore": "3"
>}
>~~~