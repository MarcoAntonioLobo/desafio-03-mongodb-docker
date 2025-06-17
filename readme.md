🐳 Ambiente de Desenvolvimento com MongoDB + Docker
Este projeto configura rapidamente um ambiente com MongoDB usando Docker e Docker Compose.

Ideal para desenvolvimento local, sem necessidade de instalar MongoDB diretamente na máquina.

🚀 Objetivo
Criar um banco de dados MongoDB com as seguintes credenciais:
```
👤 Usuário root: mongo_usr

🔐 Senha: mongo_pwd
```
🧪 Ambiente: Apenas para desenvolvimento (sem persistência obrigatória dos dados)

🗂 Estrutura do Projeto
```bash

.
├── Dockerfile              # Imagem personalizada do MongoDB
├── docker-compose.yml      # Orquestração do container
├── .env                    # Variáveis de ambiente do MongoDB
├── .gitignore              # Ignora arquivos sensíveis e desnecessários
└── README.md               # Documentação do projeto
```
🛠 Pré-requisitos
Docker

Docker Compose

Verifique se estão instalados:

```bash

docker -v
docker-compose -v
```
⚙️ Como usar
Clone o repositório ou copie os arquivos:

```bash

git clone <url-do-seu-repo>
cd nome-do-projeto
```
Edite o arquivo .env se quiser alterar usuário/senha.

Suba o container:

```bash

docker-compose up -d
```
Esse comando irá:
```
✅ Criar um container chamado mongo_dev
✅ Rodar o MongoDB na porta padrão 27017
✅ Usar as variáveis definidas no .env
```
🧪 Como testar a conexão
Use qualquer cliente MongoDB (como MongoDB Compass, mongosh, DBeaver, etc) com os seguintes dados:
```
Campo	Valor
Host	localhost
Porta	27017
Usuário	mongo_usr
Senha	mongo_pwd
Auth DB	admin
```
📦 Parar ou remover o container
Parar o container:

```bash

docker-compose down
```
Parar e apagar volumes (se estiver usando):

```bash

docker-compose down -v
```
🧾 .gitignore
Ignora arquivos sensíveis como .env, dados locais e configurações de IDEs.

📬 Contato
```
Marco Lobo
📧 marcoantoniolobo82@gmail.com
```
