# API de Gerenciamento de Solução IoT

Este é um projeto desenvolvido como parte da disciplina de Tópicos Avançados de Computação. A API é projetada para ser uma ferramenta complementar para o gerenciamento de eventos de uma solução IoT, permitindo o armazenamento, recuperação, atualização e exclusão de eventos.

## Funcionalidades

- Armazenamento de eventos da solução IoT.
- Recuperação de eventos.
- Atualização de eventos existentes.
- Exclusão de eventos.
- Autenticação JWT para acesso restrito aos recursos da API.

## Tecnologias Utilizadas

- Node.js
- Express.js
- MongoDB
- Mongoose


## Uso

1. Acesse a API através do endpoint `http://localhost:3000`.
2. Utilize um cliente HTTP (como o Insomnia ou Postman) para interagir com os endpoints disponíveis.
3. Antes de fazer qualquer requisição, certifique-se de incluir um token JWT válido no cabeçalho `Authorization` para acessar os recursos protegidos.

## Exemplo de Requisição POST para Criar um Evento

```json
POST /events

{
"type": "Falha de comunicação",
"deviceId": 123,
"timestamp": "2024-05-20T12:00:00Z",
"details": "Erro de conexão com o servidor"
}
