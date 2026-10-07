# Análise de cancelamento de clientes

Análise exploratória em Python para investigar padrões associados ao cancelamento de clientes. 
Projeto desenvolvido com organização e apresentação adaptadas para este repositório.

## O que o projeto faz

- Valida as colunas necessárias e apresenta os valores ausentes.
- Calcula quantidades e percentuais de cancelamento.
- Gera histogramas interativos com Plotly.
- Compara taxas de cancelamento por contrato, ligações e atraso.
- Explora um recorte da base sem alterar os dados originais.

## Executar localmente

Recomendado: Python 3.13, versão utilizada na validação. No terminal, dentro da pasta do projeto:

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
.\.venv\Scripts\python.exe -m jupyterlab
```

Abra `gabarito.ipynb`, selecione o kernel do ambiente criado e execute as células em ordem. No VS Code, também é possível abrir o notebook com as extensões Python e Jupyter, selecionando `.venv` como kernel.

O arquivo `cancelamentos.csv` deve estar na pasta do projeto. A leitura usa um caminho relativo; execute o notebook a partir dessa pasta.

## Arquivos

| Arquivo | Descrição |
| --- | --- |
| `gabarito.ipynb` | Análise completa, com explicações e gráficos |
| `cancelamentos.csv` | Base utilizada na aula |
| `requirements.txt` | Dependências para executar o projeto |

## Resultados da base local

Após remover quatro registros incompletos, a análise utiliza **49.996 clientes**. A taxa de cancelamento é **56,79%**. No recorte de contratos não mensais, até quatro ligações e até 20 dias de atraso, a taxa é **18,35%**.

Essa diferença descreve grupos distintos de clientes. Ela não demonstra que uma intervenção reduziria o cancelamento para esse percentual. Os resultados são exploratórios e não estabelecem causalidade.

## Dados e créditos

O notebook é salvo sem saídas para manter o arquivo leve e os diffs legíveis. Execute-o localmente para visualizar os gráficos interativos. Os materiais de vídeo, PDF e arquivos compactados da aula são ignorados pelo Git.
