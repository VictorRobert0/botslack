# Slack Bot

Este projeto é um bot para o Slack que usa Flask para gerenciar eventos e interagir com a API do Slack. Ele envia mensagens de boas-vindas, agenda mensagens e detecta palavras ruins em mensagens.

---

## Requisitos

Antes de começar, certifique-se de ter o Python 3.x instalado no seu sistema.

---

## Instalação

### 1. Clone o Repositório

Clone este repositório para sua máquina local usando o comando:

git clone <URL_DO_REPOSITORIO>
cd <NOME_DO_REPOSITORIO>


### 2. Criar um Ambiente Virtual (Opcional)

Embora não seja estritamente necessário, é recomendado usar um ambiente virtual para isolar as dependências do projeto. Você pode criar um ambiente virtual com:

python -m venv venv

Ative o ambiente virtual:

- **Windows:**

venv\Scripts\activate


- **macOS/Linux:**

source venv/bin/activate
### 3. Instalar Dependências

Instale as dependências necessárias usando `pip`. Crie um arquivo `requirements.txt` com o seguinte conteúdo:

slack-sdk
python-dotenv
flask
slackeventsapi


Então, instale todas as dependências com:

pip install -r requirements.txt


### 4. Configuração

Crie um arquivo `.env` na raiz do projeto com as seguintes variáveis:

SIGNING_SECRET_=sua_signing_secret
SLACK_TOKEN_=seu_slack_token


- `SIGNING_SECRET_` deve ser o segredo de assinatura do seu aplicativo Slack.
- `SLACK_TOKEN_` deve ser o token do bot do seu aplicativo Slack.

### 5. Executar o Aplicativo

Com o ambiente virtual ativado e as dependências instaladas, execute o aplicativo com:

python app.py


Substitua `app.py` pelo nome do seu arquivo Python, se for diferente.

### 6. Testar o Bot

- **Mensagens:** Envie uma mensagem no Slack para o bot e verifique se ele responde de acordo.
- **Reações:** Adicione uma reação a uma mensagem e veja se o bot atualiza a mensagem de boas-vindas.

---

## Funcionalidades

- **Envio de Mensagens de Boas-Vindas:** O bot envia uma mensagem de boas-vindas quando um usuário envia a palavra "start".
- **Detecção de Palavras Ruins:** O bot detecta palavras ruins em mensagens e pode responder com uma mensagem específica.
- **Mensagens Agendadas:** O bot agenda mensagens para serem enviadas em horários futuros.

---

## Criado por Victor Roberto

Sinta-se à vontade para contribuir com o projeto. Se encontrar problemas ou tiver sugestões de melhorias.
