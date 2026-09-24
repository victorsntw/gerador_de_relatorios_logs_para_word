# Gerador de Relatórios de Logs (Word)

Script em Python que lê um arquivo de logs em texto, extrai informações usando expressões regulares e gera um relatório estruturado e formatado em Word (`.docx`).

## 🔍 Análise Técnica (O que foi utilizado)
- **`re`**: Para extração de padrões (data, hora, tipo e mensagem) via Regex.
- **`python-docx`**: Para criação e formatação do documento Word (tabelas, quebras de página, parágrafos).
- **Estruturas de Dados**: Uso de listas e dicionários para agrupamento e contagem de ocorrências.
- **I/O de Arquivos**: Leitura de arquivo `.txt` e salvamento de arquivo `.docx`.
- *Nota*: O módulo `datetime` está importado, mas não é utilizado na lógica atual (as datas são tratadas como strings).

## 🚀 Funcionalidades
- Extração automática de dados do log.
- Resumo com a contagem total de ocorrências por tipo.
- Listagem detalhada de todos os registros de `ERROR`.
- Geração de tabela resumo com a quantidade de logs por dia e tipo (INFO, ERRO, WARNING, DEBUG).

## ⚙️ Como Usar

### 1. Instalação
Instale a dependência necessária para manipulação de Word:
#
```bash
pip install python-docx
```
### 2. Preparação do Arquivo de Log
Crie um arquivo chamado `logs.txt` no mesmo diretório do script. O formato esperado para cada linha é:
``` bash
AAAA-MM-DD HH:MM:SS TIPO Mensagem do log
```
Exemplo:
```bash
2023-10-27 10:15:30 ERROR Falha na conexão com o banco
2023-10-27 10:16:00 INFO Tentativa de reconexão bem-sucedida
```

### 3. Execução
Rode o script:
```bash
python main.py
```
E o arquivo Relatório de logs com Python.docx será gerado automaticamente na mesma pasta.

``` bash 
Relatório de logs com Python.docx 
```
