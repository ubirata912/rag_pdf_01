# RAG com PDF

Notebook da aula para consultar um PDF com LangChain, Chroma e OpenAI.

## Preparar no Windows

Ambiente usado na aula: Python 3.14 e VS Code com as extensoes Python e Jupyter da Microsoft.

No terminal, dentro da pasta do projeto:

```powershell
py -3.14 -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
```

Abra `index.ipynb` e escolha **Select Kernel > Python Environments > .venv**. Execute as celulas na ordem. A ativacao do terminal nao seleciona o kernel do notebook.

O notebook pede a chave da API OpenAI localmente se `OPENAI_API_KEY` nao estiver definida no ambiente. Nao escreva a chave no codigo nem a publique. O uso da API exige uma conta e acesso ao modelo indicado no notebook.

O PDF `etica-a-nicomaco.pdf` acompanha o projeto. Confira o caminho usado na celula de carregamento antes de executar. O banco vetorial em `db/` e gerado localmente e nao e versionado.

Para conferir as dependencias:

```powershell
.\.venv\Scripts\python.exe -m pip check
```
