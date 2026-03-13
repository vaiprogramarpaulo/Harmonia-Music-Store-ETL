# Harmonia Music Store Project - ETL Pipeline

Este projeto demonstra a construção de um **pipeline ETL (Extract, Transform, Load)** aplicado aos dados da loja fictícia *Harmonia Music Store*.  
O objetivo é mostrar como organizar o fluxo de dados em etapas claras e reproduzíveis, desde a extração até a exportação para análise.

---

## 🎯 Objetivo
- Consolidar dados brutos em um formato limpo e estruturado.
- Criar colunas derivadas que auxiliem na análise (ex.: Ticket Médio, ordenação de meses).
- Exportar os dados tratados para arquivos CSV e Excel, prontos para uso em ferramentas como Power BI.
- Demonstrar boas práticas de organização de código em Python.

---

## ⚙️ Estrutura do Pipeline
O pipeline segue três etapas principais:

1. **Extract (Extração)**  
   - Leitura dos dados brutos a partir de um arquivo CSV.

2. **Transform (Transformação)**  
   - Limpeza de linhas nulas e duplicadas.  
   - Criação de colunas derivadas (`Mês_Num`, `Ticket Médio`).  
   - Ajuste estético do índice para começar em 1.

3. **Load (Carregamento)**  
   - Exportação dos dados tratados para novos arquivos CSV e Excel.

---

## 📂 Arquivos do Repositório
- `notebooks/harmonia_music_store.ipynb` → Notebook Jupyter com o código completo  
- `data/harmonia_music_store.csv` → Arquivo de dados brutos (entrada)  
- `output/harmonia_music_store_tratado.csv` → Dados tratados em CSV  
- `output/harmonia_music_store_tratado.xlsx` → Dados tratados em Excel  
- `README.md` → Documento explicativo do projeto  
- `pipeline_visual_hms.pdf` -> (opcional) Fluxograma visual do processo ETL

---

## 🚀 Como Executar
1. Clone este repositório:
   ```bash
   git clone https://github.com/vaiprogramarpaulo/harmonia-music-store-etl.git
   cd harmonia-music-store-etl

2. Abra o Jupyter Notebook:
	```bash
   jupyter notebook

3. Execute o arquivo:
	```bash
   notebooks/harmonia_music_store.ipynb

---

## 📊 Resultados
Após a execução do pipeline, os dados ficam prontos para análise em ferramentas de BI.
Exemplo de colunas criadas:
- Mês_Num → facilita ordenação cronológica.
- Ticket Médio → permite avaliar o valor médio por venda.

Prévia dos dados tratados: 
| Produto | Mês       | Quantidade | Receita Total | Ticket Médio |
|---------|-----------|------------|----------------|---------------|
| Violão  | Janeiro   | 10         | 5000           | 500.0         |
| Piano   | Fevereiro | 5          | 15000          | 3000.0        |

## ✨ Autor 
- Paulo V. R. Souza
- LinkedIn: paulovrsouza
- GitHub: vaiprogramarpaulo
