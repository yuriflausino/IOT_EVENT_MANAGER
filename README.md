API de Gerenciamento de Solução IoT
Este é um projeto desenvolvido como parte da disciplina de Tópicos Avançados de Computação. A API é projetada para ser uma ferramenta complementar para o gerenciamento de eventos de uma solução IoT, permitindo o armazenamento, recuperação, atualização e exclusão de eventos.

Funcionalidades
Armazenamento de eventos da solução IoT.
Recuperação de eventos.
Atualização de eventos existentes.
Exclusão de eventos.
Autenticação JWT para acesso restrito aos recursos da API.
Tecnologias Utilizadas
Node.js
Express.js
MongoDB
Mongoose
Instalação
Certifique-se de ter o Node.js e o MongoDB instalados em sua máquina.

Clone este repositório usando o comando:

bash
Copiar código
git clone https://github.com/seu_usuario/api-gerenciamento-solucao-iot.git
Navegue até o diretório do projeto:

bash
Copiar código
cd api-gerenciamento-solucao-iot
Instale as dependências do projeto:

Copiar código
npm install
Inicie o servidor:

sql
Copiar código
npm start
Uso
Acesse a API através do endpoint http://localhost:3000.
Utilize um cliente HTTP (como o Insomnia ou Postman) para interagir com os endpoints disponíveis.
Antes de fazer qualquer requisição, certifique-se de incluir um token JWT válido no cabeçalho Authorization para acessar os recursos protegidos.
Exemplo de Requisição POST para Criar um Evento
json
Copiar código
POST /events

{
  "type": "Falha de comunicação",
  "deviceId": 123,
  "timestamp": "2024-05-20T12:00:00Z",
  "details": "Erro de conexão com o servidor"
}
