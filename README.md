📱 Sistema de Gerenciamento de Assistência Técnica de Celulares

Este é um sistema web desenvolvido em Python com Flask para o gerenciamento de serviços em uma assistência técnica de celulares. O projeto contempla cadastro de clientes, dispositivos, agendamentos de serviços, autenticação de usuários e persistência de dados via banco de dados SQL.

🚀 Funcionalidades

🔐 Autenticação e Segurança: Login e controle de acesso a páginas restritas.

👤 Gestão de Clientes: Cadastro e gerenciamento dos dados dos clientes.

📱 Gestão de Aparelhos: Registro dos dispositivos associados aos clientes para manutenção.

📅 Agendamentos de Serviços: Organização dos horários, serviços solicitados e acompanhamento.

🎨 Interface Amigável: Interface simples desenvolvida com HTML, CSS e JavaScript integrados aos templates Jinja do Flask.

📁 Estrutura do Projeto

sistema_celulares/
└── sistema_celulares_flask_desafio/
    ├── __pycache__/             # Arquivos bytecode compilados do Python
    ├── static/                  # Arquivos estáticos (CSS, JS)
    │   ├── app.js               # Scripts e interatividades do frontend
    │   └── style.css            # Estilização visual do sistema
    ├── templates/               # Páginas HTML renderizadas pelo Flask (Jinja2)
    │   ├── agendamentos.html    # Tela de agendamento de serviços
    │   ├── aparelhos.html       # Tela de gerenciamento de aparelhos
    │   ├── clientes.html        # Tela de cadastro e listagem de clientes
    │   ├── login.html           # Tela de autenticação
    │   └── principal.html       # Painel principal (Dashboard)
    ├── agendamento.py           # Lógica de negócios de agendamentos
    ├── aparelhos.py             # Lógica de negócios de aparelhos
    ├── app.py                   # Ponto de entrada (Entrypoint) da aplicação Flask
    ├── assistencia_db.sql       # Script de criação/povoamento do banco de dados
    ├── autenticacao.py          # Lógica de login/logout e permissões
    ├── clientes.py              # Lógica de negócios de clientes
    ├── db.py                    # Configuração e conexão com o banco de dados
    ├── requirements.txt         # Dependências do projeto Python
    ├── rotas.py                 # Definição das rotas e endpoints
    ├── ROTEIRO.md               # Documentação complementar / Guia do desafio
    └── testar_conexao.py        # Script utilitário para testar a conexão com o banco


🛠️ Tecnologias Utilizadas

Linguagem: Python 3.13

Framework Web: Flask

Banco de Dados: SQL (script assistencia_db.sql)

Frontend: HTML5, CSS3, JavaScript

Gerenciador de Pacotes: pip

⚙️ Como Executar o Projeto

Próximos Passos & Pré-requisitos

Ter o Python 3.x instalado.

Ter um servidor de Banco de Dados (como MySQL/PostgreSQL) configurado.

1. Clonar o Repositório

git clone <URL_DO_SEU_REPOSITORIO>
cd sistema_celulares/sistema_celulares_flask_desafio


2. Criar e Ativar um Ambiente Virtual (Opcional, mas recomendado)

# Windows
python -m venv venv
.\venv\Scripts\activate

# Linux / MacOS
python3 -m venv venv
source venv/bin/activate


3. Instalar as Dependências

pip install -r requirements.txt


4. Configurar o Banco de Dados

Execute o script assistencia_db.sql no seu SGBD de preferência para criar a estrutura das tabelas.

Verifique e adicione suas credenciais de banco de dados no arquivo db.py.

(Opcional) Teste se a conexão está funcionando corretamente:

python testar_conexao.py


5. Iniciar a Aplicação

python app.py


Acesse no seu navegador a URL indicada no terminal (geralmente http://127.0.0.1:5000/).

📄 Licença

Este projeto foi desenvolvido como parte de um desafio de aprendizado e desenvolvimento com Flask.
