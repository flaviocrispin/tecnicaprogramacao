[DS-PY-004] Técnicas de Programação I (Python)
Turma: Analista de Dados II — #1736 | Ada Tech
---
Visão Geral do Módulo
Bem-vindo(a) ao repositório do módulo Técnicas de Programação I (DS-PY-004) da formação em Análise de Dados da Ada Tech.
Este módulo tem como objetivo consolidar as bases práticas e conceituais de programação aplicadas à Análise Exploratória de Dados (EDA) e Ciência de Dados, cobrindo desde o versionamento e colaboração com Git e GitHub até o tratamento e transformação eficiente de dados com NumPy e Pandas.
---
Objetivos de Aprendizagem
Versionamento & Git: Compreender o papel do Git no fluxo de trabalho de dados, dominar comandos essenciais, estruturar repositórios locais e sincronizar com plataformas remotas (GitHub).
Computação Numérica com NumPy: Manipular arrays unidimensionais e matrizes n-dimensionais com eficiência vetorizada.
Análise & Manipulação de Dados com Pandas: Dominar estruturas `Series` e `DataFrame`, ingestão/exportação de múltiplos formatos (CSV, Excel, Parquet), tratamento de dados faltantes, agregações e transformações analíticas.
Boas Práticas: Construção de projetos versionados para portfólio profissional e código limpo/reprodutível.
---
Guia Prático: Git & GitHub Workflow
Abaixo está o passo a passo completo trabalhado em aula para criar, configurar e sincronizar seu repositório local com o GitHub.
1. Configuração Inicial do Git (Primeira vez no terminal)
```bash
# Define sua identidade nos commits
git config --global user.name "Seu Nome".
git config --global user.email "seu.email@exemplo.com"

# Define o editor padrão e o nome da branch inicial
git config --global core.editor "code -w"
git config --global init.defaultBranch main
```
---
2. Inicializando e Vinculando o Repositório
Opção A: Iniciar localmente e subir para o GitHub (Novo Projeto)
```bash
# 1. Navegue até a pasta do seu projeto e inicialize o repositório
git init

# 2. Crie o arquivo .gitignore para evitar subir arquivos pesados (>100MB) ou temporários
#echo "FactSales.csv
#*.csv
#__pycache__/
#.env
#venv/" > .gitignore

# 3. Adicione os arquivos para a área de preparação (staging)
git add .

# 4. Crie o primeiro commit
git commit -m "inicializa repositorio com scripts e documentacao"

# 5. Adicione o repositório remoto do GitHub
git remote add origin https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git

# 6. Envie o código para o GitHub vinculando a branch main
git push -u origin main
```
Opção B: Clonar um repositório já existente
```bash
git clone https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git
cd NOME_DO_REPOSITORIO
```
---
3. Ciclo de Trabalho Diário (Workflow Git)
Sempre que fizer alterações no seu código, utilize o fluxo padrão:
```bash
# 1. Verifique o status das alterações
git status

# 2. Adicione os arquivos modificados ao staging
git add .

# 3. Registre o commit com uma mensagem descritiva
git commit -m "adiciona funcoes de manipulacao e analise exploratoria"

# 4. Atualize seu repositório local antes do envio (boa prática colaborativa)
git pull origin main

# 5. Publique seus commits no GitHub
git push origin main
```
---
Boas Práticas e Atenção a Arquivos Grandes (Datasets)
Datasets Pesados (> 100 MB): O GitHub bloqueia o envio de arquivos individuais maiores que 100 MB. Sempre adicione arquivos CSV brutos ou bases volumosas ao seu `.gitignore` antes de fazer o commit.
Commits Atômicos: Faça commits frequentes e objetivos, organizando cada mudança lógica de forma clara.
---
🗓️ Cronograma do Módulo
Aula	Tema Principal	Conteúdos e Atividades

Aula 1	Git & Versionamento	Instalação, conceitos, workflow, comandos fundamentais e sincronização com GitHub.

Aula 2	NumPy: Arrays 1D	Vetorização, fatiamento, indexação, operações matemáticas e comparativo com listas.

Aula 3	NumPy: Matrizes 2D+	Operações com matrizes n-dimensionais e lançamento do mini-projeto de NumPy.

Aula 4	Pandas: Fundamentos	Estruturas `Series` e `DataFrame`; Leitura e gravação (CSV, Excel, Parquet).

Aula 5	Pandas: Transformações	Manipulação tabular avançada: `concat`, `merge`, `pivot`, `melt` e `groupby`.

Aula 6	Pandas: Limpeza de Dados	Identificação de valores atípicos e faltantes (`isna`, `describe`, `drop`, `dropna`). Definição do Projeto Final.

Aula 7	Pandas: Tratamento Avançado	Substituições com regras, `loc`/`iloc`, `apply`, `map`, `np.where` e `get_dummies`.

Aula 8	Revisão & Mentoria	Revisão geral integrada e plantão de dúvidas do projeto final em grupo.

Aula 9	Apresentação & Rubricas	Apresentação dos projetos finais e devolutiva da avaliação por rubricas.

---
📚 Bibliografia e Links Úteis
Documentação Oficial:
Git Book (Oficial)
NumPy Documentation
Pandas Documentation
Livro de Referência:
Python for Data Analysis: Data Wrangling with Pandas, NumPy, and IPython — Wes McKinney.
Cursos Digitais Ada:
Git e Versionamento
Introdução a Python
