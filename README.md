# 📚 API de Atividades Docentes


**Descrição**
Esta API é responsável por gerenciar as atividades exercidas pelos professores dentro de um sistema escolar baseado em arquitetura de microsserviços. Ela opera de forma independente, mas pode se integrar com outras APIs do ecossistema, como a API Principal (alunos, professores e turmas) e a API de Reservas.

O serviço possibilita o cadastro e consulta de registros de atividades acadêmicas e administrativas realizadas por docentes.

# 🚀 Funcionalidades

✅ Cadastrar nova atividade docente

🔍 Consultar atividades por ID ou listar todas

📆 Registrar a data e descrição da atividade

🔗 Integração com os dados de professores da API principal (via ID)


# 🛠️ Tecnologias Utilizadas

-- Python 3.x
-- Flask
-- Flask-SQLAlchemy
-- SQLite (ou outro banco relacional configurado)
-- Docker (opcional)

# 📁 Estrutura de Pastas

Atividades/
├── controllers/atividade_controller.py        # Rotas e lógica de controle das atividades
├── instance/             # Configurações específicas da instância (ex: config local)
├── models/atividade_model.py               # Definição dos modelos do banco de dados (ORM)
├── app.py                # Ponto de entrada principal da aplicação Flask
├── config.py             # Arquivo de configuração geral da aplicação
├── database.py           # Conexão e inicialização do banco de dados
├── dockerfile            # Dockerfile para containerização da aplicação
├── errors.py             # Tratamento centralizado de erros e exceções
├── README.md             # Documentação principal do projeto
└── requirements.txt      # Lista de dependências do projeto

# ⚙️ Como Executar Localmente

git clone `https://github.com/FalgasDev/AtividadeMicrosservico.git`
cd AtividadeMicrosservico

# Criar e ativar o ambiente virtual (opcional)
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate

# Instalar dependências
pip install -r requirements.txt

# Rodar a aplicação
python app.py

# Build da imagem
docker build -t atividades-api .

# Executar o container
docker run -d -p 5002:5002 atividades-api

# 📬 Endpoints Disponíveis


`/atividades -->	Lista todas as atividades` (GET)
`/atividades/<id> -->  Consulta atividade específica `(GET)	
`/atividades -->	Cadastra nova atividade`(POST)


# Contatos
- caso tenha duvidas ou sugestões, entre em contato com:
**NOMES**
# Kaio Nogueira Mungo
# Diego da Silva Criscuolo
# Bruna Bispo Andreata
# Luiz Henrique Barros Calazans
# Fábio Luiz Garrote Ramaldes

**EMAIL**
# kaio.mungo@aluno.faculdadeimpacta.com.br
# diego.criscuolo@aluno.faculdadeimpacta.com.br
# bruna.andreata@aluno.faculdadeimpacta.com.br
# luiz.calazans@aluno.faculdadeimpacta.com.br
# fabio.ramaldes@aluno.faculdadeimpacta.com.br

**GITHUB**
# https://github.com/KaioMungo
# https://github.com/Diego09cr
# https://github.com/BrunaAndreata
# https://github.com/LuizCalazans
# https://github.com/FalgasDev

📜 Licença
**Este projeto está licenciado sob os contatos acima.**