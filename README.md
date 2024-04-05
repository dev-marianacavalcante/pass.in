# pass.in

O pass.in é uma aplicação de **gestão de participantes em eventos presenciais**.

A ferramenta permite que o organizador cadastre um evento e abra uma página pública de inscrição.

Os participantes inscritos podem emitir uma credencial para check-in no dia do evento.

O sistema fará um scan da credencial do participante para permitir a entrada no evento.

## Requisitos

### Requisitos funcionais

- [ ] O organizador deve poder cadastrar um novo evento;
- [ ] O organizador deve poder visualizar dados da lista de participantes;
- [ ] O organizador deve poder visualizar a lista de participantes;
- [ ] O organizador deve poder se inscrever em um evento;
- [ ] O organizador deve poder visualizar seu crachá de inscrição;
- [ ] O organizador deve poder realizar check-in no evento;

### Regras do negócio

- [ ] O participante só pode se increver em um evento uma única vez;
- [ ] O participante só pode se inscrever em eventos com vagas disponíveis;
- [ ] O participante só pode realizar check-in em um evento uma única vez;

### Requisitos não-funcionais

- [ ] O Check-in no evento será realizado através de um QRCode;

## Anotacoes

Metodos HTTP: GET, POST, PUT, PATCH, DELETE, OPTIONS, ...

Corpo da requisicao (Request Body);
Parametros de buscqa (Search Param / Query Params) `http://localhost:3333/users?name=Mariana`
Parametros de rota (Route Params) -> Identificacao de recursos `DELETE http://localhost:3333/users/5`
Cabecalhos (Headers) -> Contexto

Semantica = Significados

Driver nativo / Query Builders / ORMs

Object Relatorial Mapping (Hibernate / Doctrine / ActiveRecord)

JSON - JavaScript Object Notation

Status code:
20x => Sucesso
30x => Redirecionamento
40x => Erro do cliente (Erro em alguma informacao enviada por QUEM esta fazendo a chamada p/ API)
50x => Erro do servidor (Um erro que esta acontencendo INDEPENDENTE do que esta sendo enviado p/ o servidor)
