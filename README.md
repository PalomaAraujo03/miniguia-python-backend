# miniguia-python-backend

# 🐍 Miniguia de Estudos: Python para Back-end

> Projeto desenvolvido como parte do desafio da DIO — uso do NotebookLM como ferramenta de aprendizagem ativa, com curadoria de fontes, engenharia de prompts e construção de um miniguia temático.

---

## 📌 Contexto e Objetivos

### Assunto escolhido
**Python para Desenvolvimento Back-end** — com foco nos frameworks Flask e FastAPI para criação de APIs REST.

### Por que esse tema?
O desenvolvimento back-end com Python é uma das habilidades mais demandadas no mercado de tecnologia atualmente. Frameworks como FastAPI estão em franca ascensão, sendo adotados por grandes empresas como Microsoft, Uber e Netflix. Este estudo visa construir uma base sólida para aplicações práticas e estágios na área.

### Objetivos de estudo
- Compreender o papel do Python no desenvolvimento back-end
- Entender o que é uma API REST e como ela funciona
- Conhecer as diferenças entre Flask, FastAPI e Django
- Aprender os conceitos fundamentais do FastAPI (rotas, validação, documentação automática)
- Montar um glossário dos principais termos da área
- Construir prompts reutilizáveis para revisões futuras

---

## 📚 Curadoria de Fontes

As fontes abaixo foram selecionadas e carregadas no NotebookLM:

| # | Tipo | Fonte | Link |
|---|------|-------|------|
| 1 | 📄 Documentação | Documentação oficial do FastAPI | https://fastapi.tiangolo.com/tutorial/ |
| 2 | 📄 Documentação | Documentação oficial do Flask | https://flask.palletsprojects.com/en/stable/ |
| 3 | 📝 Artigo | Real Python — Get Started with FastAPI | https://realpython.com/get-started-with-fastapi/ |
| 4 | 📝 Artigo | DataCamp — Python Backend Development | https://www.datacamp.com/tutorial/python-backend-development |
| 5 | 🎬 Vídeo | YouTube — Curso FastAPI (Hashtag Treinamentos) | *(inserir link do YouTube aqui)* |

> **Critério de seleção:** fontes gratuitas, abertas, atualizadas e com abordagem técnica acessível para iniciantes. Priorizei fontes oficiais e canais reconhecidos pela comunidade Python.

---

## 🧪 Engenharia de Prompts e "Cicatrizes"

Esta seção documenta as perguntas estratégicas testadas no NotebookLM, as respostas obtidas, e os ajustes realizados.

---

### Bloco 1 — Compreensão do tema

**Prompt 1.1**
> *"O que é back-end e qual o papel do Python nesse contexto?"*

- ✅ Resultado: O back-end refere-se aos bastidores de uma aplicação, englobando tudo o que o usuário não consegue enxergar diretamente, mas que é processado e transformado no servidor
. Enquanto o front-end lida com a interface gráfica e o layout, o back-end é responsável pela lógica de negócio, cálculos e tarefas repetitivas, representando a maior parte do esforço de desenvolvimento de um sistema
. Sua função primordial, dentro da arquitetura cliente-servidor, é receber requisições do navegador, processar essas informações (como validar dados ou realizar consultas em bancos de dados) e retornar os resultados necessários para o cliente
.
O papel do Python nesse contexto é fundamental, sendo uma das linguagens mais populares e recomendadas para o desenvolvimento do lado do servidor
. A linguagem destaca-se por sua filosofia de design que prioriza a legibilidade do código e a produtividade do programador, oferecendo uma sintaxe clara e concisa
. Python permite o uso de diversos paradigmas de programação, como a orientação a objetos, facilitando a criação de sistemas complexos de forma organizada
.
Para atuar no back-end com Python, os desenvolvedores utilizam ferramentas e conceitos específicos destacados nas fontes:
Frameworks Web: São essenciais para não precisar escrever tudo do zero
. Os principais são o Django (robusto e completo para aplicações grandes), o Flask (um microframework leve e flexível para APIs e microsserviços) e o FastAPI (focado em alta performance e tipagem moderna)
.
Gestão de Dados: O back-end Python frequentemente interage com bancos de dados (relacionais como MySQL/PostgreSQL ou não-relacionais como MongoDB)
. Ferramentas de ORM (Object-Relational Mapping), como o SQLAlchemy, facilitam esse trabalho ao mapear tabelas de banco de dados para classes Python, permitindo manipular dados como se fossem objetos da linguagem
.
APIs e Protocolos: O Python é amplamente usado para construir APIs (Application Programming Interfaces), que são os protocolos que permitem a comunicação entre diferentes aplicações ou entre o front-end e o back-end através de requisições HTTP
.
Segurança e Autenticação: Tarefas críticas como autenticação de usuários, autorização de acesso e armazenamento seguro de senhas (usando hashes criptográficos) são funções centrais executadas pelo código back-end
.
Além dessas funções, o desenvolvedor back-end Python também lida com o deploy (implantação) da aplicação em servidores de produção, utilizando ferramentas auxiliares como Docker para contêineres e sistemas operacionais Linux
- 💡 Observações: O comando funcionou bem 

---

**Prompt 1.2**
> *"Quais são as principais diferenças entre Flask, FastAPI e Django? Quando usar cada um?"*

- ✅ Resultado:As principais diferenças entre Django, Flask e FastAPI residem na sua arquitetura, no nível de recursos nativos oferecidos e no desempenho, sendo cada um voltado para necessidades específicas de desenvolvimento
.
1. Django: O Framework "Baterias Incluídas"
O Django é um framework de alto nível que segue o padrão MTV (Model-Template-View)
. Ele é conhecido por oferecer quase tudo o que um desenvolvedor precisa "pronto para uso"
.
Diferenciais: Possui um painel administrativo automático, sistema de autenticação robusto, ORM (Object-Relational Mapping) integrado e extensa documentação
.
Vantagens: Ideal para aplicações grandes e complexas, garantindo rapidez no desenvolvimento de funcionalidades comuns
.
Desvantagens: É menos flexível para arquiteturas personalizadas e pode ser considerado "pesado" ou excessivo para projetos pequenos ou APIs simples
.
2. Flask: Minimalismo e Flexibilidade
O Flask é classificado como um microframework, fornecendo apenas o núcleo essencial para fazer uma aplicação web funcionar
.
Diferenciais: É "não opinativo", o que significa que o desenvolvedor tem total liberdade para escolher quais bibliotecas e extensões deseja usar para banco de dados ou autenticação
.
Vantagens: É leve, fácil de entender e altamente personalizável
.
Desvantagens: Exige que o desenvolvedor tome mais decisões de arquitetura e requer a instalação manual de extensões para recursos que já vêm nativos no Django
.
3. FastAPI: Performance e Modernidade
O FastAPI é um framework moderno focado na construção de APIs com alta performance, utilizando recursos recentes do Python como type hints (dicas de tipagem)
.
Diferenciais: Baseado em Pydantic e Starlette, ele oferece validação automática de dados e gera documentação interativa (Swagger) de forma automática
.
Vantagens: Oferece um desempenho altíssimo (comparável a Node.js e Go) e suporte nativo para programação assíncrona (async/await)
.
Desvantagens: Possui menos recursos prontos para criar aplicações web completas (com interface do usuário) em comparação ao Django e tem uma comunidade ainda em crescimento
.
Resumo de "Quando usar":
Framework
Quando usar?
Django
Quando você precisa criar aplicações completas e robustas (como um e-commerce ou CMS) que necessitam de um painel administrativo e segurança pré-configurada
.
Flask
Quando você quer criar projetos leves, MVPs (Mínimo Produto Viável) ou microsserviços onde a simplicidade e a flexibilidade total de escolha são prioridades
.
FastAPI
Quando o foco é a criação de APIs modernas e performáticas, que exigem validação rigorosa de dados e alta capacidade de processamento assíncrono
.
- 
- ⚠️ Dificuldade encontrada: * Não encontrei dificuldades *

---

**Prompt 1.3**
> *"O que é uma API REST e como ela funciona?"*

- ✅ Resultado: * Uma API REST (Representational State Transfer) é um estilo de arquitetura utilizado para construir serviços web que permitem a comunicação entre diferentes aplicações através do protocolo HTTP
. O termo API significa "Application Programming Interface" (Interface de Programação de Aplicativos) e refere-se ao conjunto de protocolos e padrões que possibilitam que sistemas distintos "conversem" entre si
.
Para entender como ela funciona, é necessário observar os seguintes pilares fundamentais descritos nas fontes:
1. Arquitetura Cliente-Servidor
O funcionamento de uma API REST baseia-se na interação entre um cliente (geralmente o navegador ou um aplicativo) e um servidor remoto (o back-end)
.
O cliente envia uma requisição HTTP para o servidor solicitando ou enviando dados
.
O servidor processa essa solicitação, realiza a lógica necessária (como consultar um banco de dados) e devolve uma resposta HTTP
.
2. Métodos ou Verbos HTTP
Uma API REST utiliza verbos específicos para definir qual ação deve ser executada sobre um recurso
. Essas ações geralmente estão ligadas ao conceito de CRUD (Create, Read, Update, Delete)
:
GET: Utilizado para ler ou recuperar informações de um servidor
.
POST: Usado para enviar novos dados e criar um recurso
.
PUT: Destinado à atualização de dados já existentes
.
DELETE: Serve para remover um recurso específico
.
3. Statelessness (Ausência de Estado)
Uma característica central do REST é ser stateless. Isso significa que cada requisição HTTP é independente e deve conter todas as informações necessárias para que o servidor a entenda e processe
. O servidor não armazena o contexto do cliente entre as chamadas
.
4. Recursos e Endpoints
A API organiza os dados em recursos, que são identificados por caminhos únicos chamados endpoints ou rotas (URLs)
. Por exemplo, uma rota /usuarios pode ser usada para acessar os dados de todas as pessoas cadastradas em um sistema
.
5. Formato de Dados (JSON)
Embora possa usar outros formatos, a grande maioria das APIs REST modernas utiliza o JSON (JavaScript Object Notation) para trocar informações
. O JSON é um formato leve e fácil de ser lido tanto por humanos quanto por máquinas, sendo o padrão de resposta padrão em frameworks como o FastAPI e o Flask
.
6. Códigos de Status
Toda resposta do servidor inclui um código de status HTTP, que informa ao cliente se a operação foi bem-sucedida ou se houve um erro
. Alguns exemplos comuns incluem:
200 OK: A solicitação foi bem-sucedida
.
400 Bad Request: Há um erro nos dados enviados pelo cliente
.
404 Not Found: O recurso solicitado (URL) não foi encontrado no servidor
.
500 Internal Server Error: Ocorreu uma falha inesperada no servidor
.
Ao seguir esses padrões, uma API REST torna-se legível, escalável e fácil de manter, permitindo que diferentes desenvolvedores integrem seus sistemas de forma eficiente*

- 💡 Observações: * Não tive que refazer o comando*

---

### Bloco 2 — Aprofundamento técnico

**Prompt 2.1**
> *"Como funciona o ciclo de uma requisição HTTP no FastAPI? Explique passo a passo."*

- ✅ Resultado: *Embora as fontes forneçam uma visão geral do ciclo de requisição em sites dinâmicos e as características específicas do FastAPI, o funcionamento passo a passo de uma requisição nesse framework pode ser compreendido através da síntese dos conceitos de arquitetura cliente-servidor e as funcionalidades nativas do FastAPI descritas nos documentos.
Aqui está o ciclo de uma requisição HTTP no FastAPI, passo a passo:
Envio da Solicitação pelo Cliente: O navegador ou cliente (como o Insomnia ou ferramentas de teste de API) envia uma solicitação HTTP para o servidor
. Esta solicitação inclui uma URL, um método (como GET, POST, PUT ou DELETE) e pode conter parâmetros de consulta, dados no corpo (JSON) ou cookies
.
Recepção pelo Servidor de Aplicação: A solicitação é recebida por um servidor remoto (geralmente um servidor ASGI para FastAPI, como o Uvicorn) que atua nos bastidores e encaminha a mensagem para a aplicação FastAPI
.
Roteamento e Validação Automática: O FastAPI identifica qual função de rota deve processar a requisição com base na URL e no método
. Diferente de outros frameworks, o FastAPI utiliza Type Hints do Python e a biblioteca Pydantic para realizar a validação automática de dados assim que a requisição chega
. Se os dados enviados pelo usuário não estiverem no formato correto (ex: um texto onde deveria ser um número), o framework retorna um erro automaticamente antes mesmo de executar a lógica de negócio
.
Processamento da Lógica de Negócio (Async/Await): Uma vez validados os dados, a função de rota é executada. O FastAPI destaca-se por permitir o uso de programação assíncrona (async e await), o que permite que o servidor processe outras tarefas enquanto aguarda respostas de bancos de dados ou APIs externas, garantindo um altíssimo desempenho
.
Interação com Banco de Dados (Opcional): Caso a requisição exija salvar ou recuperar informações, o back-end interage com uma base de dados
. Isso geralmente é feito através de um ORM como o SQLAlchemy, que mapeia as tabelas do banco para classes Python, facilitando a manipulação dos dados como objetos
.
Serialização da Resposta: Após o processamento, o FastAPI converte automaticamente os objetos Python ou resultados do banco de dados em um formato que o cliente entenda, geralmente JSON
. O framework também gera a documentação automática dessa resposta através do Swagger
.
Retorno da Resposta HTTP: O servidor envia de volta uma resposta HTTP ao navegador
. Esta resposta contém uma linha de status (como o código 200 OK para sucesso ou 404 Not Found para erros) e o corpo com os dados solicitados ou a confirmação da operação
.
*
- 💡 Observações: Compreendeu o comando

---

**Prompt 2.2**
> *"O que são rotas, endpoints e métodos HTTP (GET, POST, PUT, DELETE)? Dê exemplos práticos."*

- ✅ Resultado: *No desenvolvimento back-end, a comunicação entre o navegador (cliente) e o servidor ocorre através do protocolo HTTP, utilizando rotas, endpoints e métodos para organizar como os dados são solicitados e processados
.
Rotas e Endpoints
Rotas: São os caminhos (URLs) que os usuários utilizam para acessar recursos específicos de uma aplicação
. Elas funcionam como "endereços" que dizem ao framework (como Flask ou FastAPI) qual função do código deve ser executada para processar aquela solicitação
.
Endpoints: Embora frequentemente usados como sinônimos de rotas, o termo refere-se especificamente ao ponto final de comunicação de uma API onde os recursos podem ser acessados
. Em frameworks modulares como o Flask, o nome do endpoint costuma ser o nome da função associada à rota, podendo ser prefixado pelo nome de um "Blueprint"
.
Métodos HTTP
Os métodos definem a ação que deve ser realizada sobre o recurso identificado pela rota
. Os principais são associados às operações de CRUD (Create, Read, Update, Delete)
:
GET (Leitura): Utilizado para obter ou recuperar informações do servidor (como uma página HTML, uma imagem ou uma lista de usuários)
. É o método padrão para a maioria das rotas
.
POST (Criação): Usado para enviar novos dados ao servidor, como informações de um formulário de cadastro ou um novo arquivo
. No ciclo de login, por exemplo, o POST envia as credenciais para autenticação
.
PUT (Atualização): Destinado a atualizar ou substituir dados existentes
. É comum usá-lo para editar informações de um perfil de usuário ou o conteúdo de uma postagem de blog
.
DELETE (Exclusão): Serve para remover um recurso específico do servidor
.
Exemplos Práticos
Imagine um sistema de gerenciamento de usuários
. As rotas e métodos seriam organizados da seguinte forma:
Listar todos os usuários:
Rota: /usuarios
Método: GET
Ação: O servidor consulta o banco de dados e retorna a lista de todos os cadastrados
.
Cadastrar um novo usuário:
Rota: /usuarios
Método: POST
Ação: O servidor recebe o nome e o tipo do usuário e os insere em uma nova linha da tabela do banco de dados
.
Atualizar o nome de um usuário específico:
Rota: /usuarios/<id> (ex: /usuarios/1)
Método: PUT
Ação: O servidor localiza o usuário pelo ID "1" e altera seu nome para o novo valor enviado
.
Remover um usuário do sistema:
Rota: /usuarios/<id> (ex: /usuarios/1)
Método: DELETE
Ação: O servidor identifica o registro pelo ID "1" e o deleta permanentemente da base de dados
.
Essa estrutura garante que a aplicação seja legível, mantível e escalável, permitindo que diferentes desenvolvedores entendam facilmente como interagir com a API
*
- ⚠️ Dificuldade encontrada: Não tive dificuldade
- 🔁 Prompt ajustado: Não precisou ajustar 
  

---

**Prompt 2.3**
> *"O que é Pydantic e por que o FastAPI usa para validação de dados?"*

- ✅ Resultado: *O Pydantic é uma biblioteca de validação de dados e gerenciamento de configurações para Python, baseada em type hints (dicas de tipagem)
. No contexto do FastAPI, ele funciona como o "motor" que interpreta e valida os dados que entram e saem da aplicação
.
O FastAPI utiliza o Pydantic para validação de dados pelos seguintes motivos principais:
Validação Automática de Dados: Assim como mencionado em nossa conversa anterior, o FastAPI utiliza os modelos Pydantic para verificar se os dados enviados pelo cliente (em uma requisição POST, por exemplo) estão no formato correto assim que chegam ao servidor
. Se um campo que deveria ser um número for enviado como texto, o Pydantic detecta o erro e o FastAPI retorna uma resposta de erro ao usuário automaticamente, antes mesmo de a lógica de negócio ser executada.
Tipagem Estática Moderna: O Pydantic permite que o desenvolvedor defina a estrutura dos dados usando a sintaxe padrão de tipos do Python 3.6+
. Isso torna o código mais legível, fácil de manter e permite que editores de código (como o VS Code) ofereçam melhor preenchimento automático e detecção de erros durante o desenvolvimento
.
Documentação Interativa (OpenAPI/Swagger): Um dos grandes diferenciais do FastAPI é a geração automática de documentação
. O framework lê os modelos Pydantic e os utiliza para gerar os esquemas JSON que alimentam ferramentas como o Swagger UI, detalhando exatamente quais campos a API espera receber e quais tipos de dados ela retorna
.
Alta Performance: O FastAPI é construído sobre o Pydantic (e o Starlette), o que contribui para o seu desempenho altíssimo, sendo comparável a linguagens como Node.js e Go
.
Serialização de Dados: Além de validar o que entra, o Pydantic facilita a conversão de objetos Python complexos em formatos que podem ser enviados pela rede, como JSON, garantindo que a resposta da API também siga um contrato estrito
.
Em resumo, enquanto o FastAPI gerencia as rotas e a comunicação web, o Pydantic garante a integridade dos dados, assegurando que a aplicação só processe informações que estejam estritamente de acordo com o que foi definido pelo desenvolvedor
.*
- 💡 Observações: Não precisei refazer o comando 

---

### Bloco 3 — Aplicação prática

**Prompt 3.1**
> *"Como eu criaria uma API simples de gerenciamento de tarefas (to-do list) com FastAPI?"*

- ✅ Resultado: * Para criar uma API simples de gerenciamento de tarefas (to-do list) com o FastAPI, você deve seguir um fluxo que envolve a preparação do ambiente, a definição dos modelos de dados e a implementação das rotas para as operações básicas de CRUD (Criar, Ler, Atualizar e Deletar).
Aqui está o passo a passo baseado nas fontes:
1. Preparação do Ambiente
Antes de começar, é altamente recomendado criar e ativar um ambiente virtual para isolar as dependências do projeto
. Em seguida, instale o FastAPI:
Instalação: Use o comando pip install "fastapi[standard]"
. A versão "standard" já inclui as dependências necessárias para rodar o servidor e as ferramentas de desenvolvimento
.
Editor: O VS Code é recomendado, e existe uma extensão oficial do FastAPI que ajuda na busca e navegação de rotas
.
2. Estrutura Básica e Modelo de Dados
O FastAPI utiliza o Pydantic para a validação automática de dados
. Você deve definir como uma "tarefa" se parece usando uma classe que herda de BaseModel.
from fastapi import FastAPI
from pydantic import BaseModel
from typing import Optional

app = FastAPI() # Inicializa a aplicação [5]

# Modelo Pydantic para validar a entrada de dados [4]
class Task(BaseModel):
    id: int
    titulo: str
    descricao: Optional[str] = None
    concluida: bool = False
3. Implementação das Rotas (Endpoints)
Você usará os métodos HTTP para definir as ações da sua API
:
Criar (POST): Para adicionar uma nova tarefa à lista.
Listar (GET): Para recuperar a lista de tarefas
.
Atualizar (PUT): Para modificar uma tarefa existente (como marcar como concluída)
.
Deletar (DELETE): Para remover uma tarefa através do seu ID
.
Exemplo de uma rota para listar tarefas:
tasks_db = [] # Banco de dados simples na memória para testes [8]

@app.get("/tasks")
def get_tasks():
    return tasks_db
4. Execução e Testes
Para rodar sua API localmente, salve o código em um arquivo (ex: main.py) e use o comando:
fastapi dev main.py
.
Diferenciais do FastAPI para seu projeto:
Documentação Automática: Assim que o servidor subir, você pode acessar /docs no seu navegador para visualizar a documentação interativa gerada pelo Swagger UI, onde pode testar cada endpoint diretamente
.
Performance: O framework oferece altíssimo desempenho, ideal para aplicações modernas e assíncronas
.
Thunder Client: Dentro do VS Code, você pode usar a extensão Thunder Client para realizar requisições de teste (GET, POST, etc.) sem precisar sair do editor
.
Se desejar que as tarefas sejam salvas permanentemente, você precisará integrar um banco de dados (como o SQLite) utilizando um ORM como o SQLAlchemy, que mapeia suas classes Python para tabelas de banco de dados
*
- 💡 Observações: 

---

**Prompt 3.2**
> *"Quais boas práticas devo seguir ao organizar um projeto back-end em Python?"*

- ✅ Resultado: * Organizar um projeto back-end em Python exige a adoção de padrões que garantam a manutenibilidade, escalabilidade e segurança do sistema. De acordo com as fontes, as principais boas práticas podem ser divididas em estrutura de código, ambiente de desenvolvimento, segurança e gestão de dados.
1. Estrutura de Projeto e Modularidade
Uma das práticas mais importantes é evitar o "código espaguete", onde lógica de negócio, rotas e banco de dados se misturam
.
Separação de Responsabilidades: Recomenda-se organizar o projeto em diretórios distintos, como models/ (banco de dados), routes/ (endpoints), schemas/ (validação/serialização), services/ (lógica de negócio) e tests/
.
Uso de Blueprints (Flask): Para aplicações grandes, é essencial utilizar Blueprints, que permitem fatorar o código em componentes distintos, facilitando o gerenciamento de rotas e recursos de forma modular
.
Padrão MTV (Django): Seguir rigorosamente a arquitetura Model-Template-View do Django ajuda a manter o mapeamento do banco de dados e a lógica de negócio organizados e interligados de forma lógica
.
2. Ambiente de Desenvolvimento e Ferramentas Auxiliares
Um ambiente bem configurado evita conflitos e melhora a produtividade.
Ambientes Virtuais: É altamente recomendado o uso de ambientes virtuais (como venv ou Poetry) para isolar as dependências de cada projeto
. O uso do Poetry é destacado para um controle de dependências mais robusto
.
Formatação de Código: Utilizar ferramentas como o Black garante que o código esteja sempre devidamente formatado e bonitão, seguindo padrões de legibilidade
.
Versionamento: O uso do Git é essencial para o trabalho em equipe e controle de histórico
.
Testes Automatizados: Implementar testes unitários (usando pytest, por exemplo) é integral para assegurar que a API se comporte corretamente
.
3. Segurança e Gestão de Dados
O back-end é responsável por tarefas críticas que exigem atenção redobrada à segurança.
Proteção de Senhas: Nunca armazene senhas em texto puro
. Utilize bibliotecas como a werkzeug.security para gerar e verificar hashes criptográficos
.
Validação de Dados: Use bibliotecas de validação automática, como Pydantic (nativa no FastAPI) ou Marshmallow (comum no Flask), para garantir que os dados recebidos estejam no formato correto antes do processamento
.
Uso de ORM: Prefira utilizar um ORM (como SQLAlchemy ou o ORM do Django) em vez de SQL nativo. Isso oferece abstração, portabilidade entre bancos de dados e facilita a manipulação de dados através de objetos Python
.
Migrações: Para alterações no esquema do banco de dados, utilize ferramentas de migração como Alembic ou Flask-Migrate para manter a integridade da base de dados entre diferentes ambientes
.
4. Boas Práticas em APIs e Produção
Verbos e Métodos HTTP: Utilize os métodos corretos para cada ação (GET para leitura, POST para criação, PUT para atualização e DELETE para exclusão) e siga padrões de arquitetura REST para ordenação, filtragem e paginação
.
Tratamento de Erros e Logs: Registre handlers de erro para fornecer respostas claras ao cliente (como páginas 404 customizadas) e utilize ferramentas como o Sentry para monitorar exceções em tempo real
.
Deploy Seguro: Nunca utilize o servidor de desenvolvimento em produção, pois ele não é seguro nem eficiente
. Utilize servidores dedicados como Gunicorn, Uvicorn ou WSGI/ASGI e configure o sistema atrás de um proxy reverso como Nginx
.
Segurança de Cookies: Em produção, utilize sempre HTTPS e configure cookies como secure e httpOnly para protegê-los de acessos maliciosos via JavaScript *
- 💡 Observações: Não precisei refazer o comando

---

### Bloco 4 — Glossário e revisão

**Prompt 4.1**
> *"Liste os 15 termos mais importantes do desenvolvimento back-end com Python e explique cada um em até 2 linhas."*

- ✅ Resultado: *Com base nos documentos e no nosso histórico, aqui estão os 15 termos fundamentais do desenvolvimento back-end com Python:
Back-end: Refere-se aos "bastidores" de uma aplicação, onde ocorre o processamento de dados, lógica de negócio e cálculos no servidor
. É a parte que o usuário não enxerga, mas que sustenta o funcionamento do sistema
.
Framework: Coleção de ferramentas e regras (como Django, Flask ou FastAPI) que aceleram o desenvolvimento e resolvem problemas comuns
. Eles organizam a estrutura do código e fornecem funcionalidades prontas como autenticação e acesso a dados
.
API (Application Programming Interface): Conjunto de protocolos que permite que diferentes aplicações se comuniquem entre si
. Funciona como uma interface padrão para que o front-end solicite recursos ao servidor
.
Métodos HTTP: Verbos que definem a ação de uma requisição, sendo os principais: GET (leitura), POST (criação), PUT (atualização) e DELETE (exclusão)
. Eles orientam como o servidor deve manipular um recurso específico
.
Rotas/Endpoints: URLs específicas que identificam o ponto de acesso a um recurso no servidor
. Cada rota é mapeada para uma função de código que processa a solicitação do cliente
.
Banco de Dados: Sistema responsável por armazenar, recuperar e organizar as informações de forma persistente
. Podem ser relacionais (como PostgreSQL), que usam tabelas, ou não-relacionais (como MongoDB)
.
ORM (Object-Relational Mapping): Tecnologia que mapeia tabelas de banco de dados para classes e objetos na programação
. Permite manipular dados usando código Python puro, abstraindo a necessidade de escrever SQL nativo
.
Autenticação: Processo de verificação da identidade de um usuário, geralmente através de credenciais como login e senha
. Garante que a pessoa acessando o sistema é realmente quem ela diz ser
.
Autorização: Mecanismo que determina se um usuário já autenticado possui permissão para acessar áreas ou recursos específicos
. Depende da identidade do usuário para conceder ou negar direitos de acesso
.
Hashing: Técnica de transformar senhas em códigos criptográficos irreversíveis para armazenamento seguro no banco de dados
. Protege as senhas originais mesmo em caso de vazamento de dados
.
Sessão (Session): Recurso que permite ao servidor manter o estado e memorizar informações do usuário entre diferentes interações
. É o que mantém você "logado" enquanto navega por várias páginas de um site
.
Deploy: Ato de implantar a aplicação em um servidor de produção para torná-la disponível aos usuários na internet
. Envolve o uso de servidores robustos e seguros como Gunicorn ou Nginx
.
Docker: Ferramenta de criação de contêineres que isolam a aplicação e suas dependências
. Garante que o sistema funcione da mesma forma em qualquer computador ou servidor
.
Async/Await: Comandos de programação assíncrona que permitem que o servidor realize múltiplas tarefas simultaneamente sem travar
. É essencial para garantir alta performance em frameworks como o FastAPI
.
Pydantic: Biblioteca de validação de dados baseada em tipos, usada para garantir que as informações enviadas para a API estejam no formato correto
. Ela automatiza a verificação de erros e a geração de documentação
.*
- 💡 Observações: Não precisei refazer o comando

---


## 📖 Miniguia de Estudo (Entrega Final)

### Resumos Estruturados

#### O que é Back-end?
> * O back-end refere-se a tudo aquilo que acontece nos bastidores de uma aplicação, sendo processado e transformado no servidor, longe da visão direta do usuário *

#### Python no Back-end
> * A utilização da linguagem Python no back-end é caracterizada por sua filosofia de priorizar a legibilidade do código e o esforço do programador sobre a velocidade de execução computacional
. No contexto do desenvolvimento do lado do servidor, o Python é responsável pelo "trabalho duro": processamento de dados, lógica de negócio, interações com bancos de dados e a sustentação da arquitetura cliente-servidor *

#### O que é uma API REST?
> * Uma API REST (Representational State Transfer) é um estilo de arquitetura utilizado para resolver serviços web, permitindo que diferentes aplicações se comuniquem entre si de forma padronizada
. O termo API refere-se a uma "Interface de Programação de Aplicativos", que funciona como um conjunto de protocolos e ferramentas que permitem a interação entre sistemas distintos *

#### Flask vs FastAPI vs Django
> * A escolha entre os principais frameworks Python — Django, Flask e FastAPI — depende do equilíbrio entre a necessidade de recursos prontos, flexibilidade e exigências de desempenho

> O Django é um framework de alto nível que utiliza o padrão MTV (Model-Template-View)

> Flask: Minimalismo e Flexibilidade
O Flask é um microframework que fornece apenas o núcleo essencial, permitindo total liberdade de escolha de bibliotecas externas


>FastAPI: Performance e Modernidade
O FastAPI é voltado para a construção de APIs de altíssimo desempenho, com performance comparável a Go e Node.js


*

#### Fundamentos do FastAPI
> * O FastAPI é um framework moderno e de alto desempenho para a construção de APIs com Python 3.6+, fundamentado em padrões abertos como OpenAPI e JSON Schema
. Seus fundamentos combinam a agilidade do Flask com a robustez do Django, sendo especialmente otimizado para o processamento rápido de requisições *

---

### 📘 Glossário

| Termo | Definição |
|-------|-----------|
. É a parte que o usuário não enxerga, mas que sustenta o funcionamento do sistema* |
| BACKEND | *  * |
| REST | *()* |
| Endpoint | *(preencha)* |
| Rota | *(preencha)* |
| HTTP | *(preencha)* |
| GET / POST / PUT / DELETE | *(preencha)* |
| Request / Response | *(preencha)* |
| JSON | *(preencha)* |
| Framework | *(preencha)* |
| Pydantic | *(preencha)* |
| Uvicorn | *(preencha)* |
| ASGI / WSGI | *(preencha)* |
| Virtual Environment (venv) | *(preencha)* |
| Swagger UI | *(preencha)* |
| CRUD | *(preencha)* |

---

### 🔁 Prompts Reutilizáveis para Revisão Futura

Use estes prompts sempre que quiser revisar o tema em sessões futuras no NotebookLM ou em qualquer IA:

```
1. "Explique o que é uma API REST e quais são os métodos HTTP mais usados."

2. "Quais são as vantagens do FastAPI em relação ao Flask para projetos modernos?"

3. "Como o Pydantic ajuda na validação de dados em aplicações FastAPI?"

4. "Me dê um exemplo de código comentado de uma rota GET simples em FastAPI."

5. "Quais boas práticas devo seguir ao estruturar um projeto back-end em Python?"

6. "Crie 5 perguntas de revisão sobre os fundamentos de back-end com Python."

7. "Explique o ciclo completo de uma requisição HTTP em uma API FastAPI."
```

---

## 🛠️ Tecnologias e Ferramentas

- **Python 3.x**
- **FastAPI**
- **Flask**
- **NotebookLM** (Google) — ferramenta de estudo com IA
- **GitHub** — versionamento e portfólio

---

## 👩‍💻 Autora

**Paloma Araujo** — Estudante de Engenharia de Software  
🔗 [GitHub](https://github.com/PalomaAraujo03) | [LinkedIn](*(inserir link)*)

---

*Projeto desenvolvido como entrega do desafio de projeto da [DIO](https://www.dio.me/).*
