# Projeto SQL 2 - Análise de Perfil dos Clientes

## Sobre o projeto

Esse foi o segundo projeto guiado que desenvolvi durante o curso **SQL para Análise de Dados: Do básico ao avançado**, ministrado pela Midori Toyota na Udemy.

No projeto, analisei o perfil dos clientes que visitaram um e-commerce de veículos e os principais tipos de veículos procurados por eles.

Fiz as consultas no PostgreSQL por meio do pgAdmin. Depois, levei os resultados para o Excel e usei os dados para montar o dashboard.

## Objetivo

O objetivo foi criar um dashboard para entender melhor o perfil dos clientes e seus interesses, analisando gênero, status profissional, faixa etária e faixa salarial.

Também analisei a classificação, a idade e os modelos dos veículos mais visitados no e-commerce.

## Perguntas respondidas

- Qual é a distribuição dos clientes por gênero?
- Quais são os status profissionais mais frequentes?
- Qual é a faixa etária predominante?
- Qual é a faixa salarial predominante?
- Os clientes visitam mais veículos novos ou seminovos?
- Qual é a faixa de idade dos veículos mais visitados?
- Quais são os modelos mais visitados de cada marca?

## Indicadores e análises apresentados

- Distribuição dos clientes por gênero
- Distribuição por status profissional
- Distribuição por faixa etária
- Distribuição por faixa salarial
- Classificação dos veículos entre novos e seminovos
- Distribuição dos veículos por faixa de idade
- Modelos mais visitados por marca

## Banco de dados

A base fictícia usada no projeto representa as operações de um marketplace de veículos.

Principais tabelas consultadas:

- `sales.funnel`: registros das visitas realizadas no e-commerce
- `sales.customers`: informações dos clientes
- `sales.products`: informações dos veículos visitados

## Recursos SQL aplicados

- Consultas com `SELECT`
- Filtros com `WHERE`
- Relacionamentos entre tabelas com `JOIN`
- Agrupamentos com `GROUP BY`
- Ordenação com `ORDER BY`
- Contagens com `COUNT`
- Subqueries
- Expressões de tabela comuns com `WITH`
- Classificações com `CASE`
- Tratamento de datas
- Conversão de tipos
- Cálculos de porcentagem
- Criação de faixas etárias, salariais e de idade dos veículos

## Ferramentas utilizadas

- SQL
- PostgreSQL
- pgAdmin
- Microsoft Excel

## Organização do arquivo Excel

O arquivo possui três abas:

| Aba | Conteúdo |
|---|---|
| Dashboard | Apresentação visual dos indicadores e gráficos |
| Resultados das Consultas | Resultados extraídos das consultas executadas no PostgreSQL |
| Consultas SQL | Consultas utilizadas para produzir cada análise |

## Dashboard

![Dashboard de Perfil dos Clientes](Imagens/Print%20Dashboard%20Projeto%202.jpg)

## Arquivos do projeto

- [Abrir o dashboard em Excel](Dashboard/Projeto%202%20-%20Dashboard%20de%20Perfil%20dos%20Clientes.xlsx)
- [Visualizar as consultas SQL](SQL/Querys%20Projeto%202%20-%20Dashboard%20de%20Perfil%20dos%20Clientes.sql)

## Estrutura do repositório

```text
sql-analise-perfil-clientes/
├── README.md
├── Dashboard/
│   └── Projeto 2 - Dashboard de Perfil dos Clientes.xlsx
├── Imagens/
│   └── Print Dashboard Projeto 2.jpg
└── SQL/
    └── Querys Projeto 2 - Dashboard de Perfil dos Clientes.sql
```

## Aprendizados

Com esse projeto, consegui aplicar SQL para analisar o perfil dos clientes e identificar os principais interesses relacionados aos veículos disponíveis no e-commerce.

Também pratiquei a criação de categorias e faixas com `CASE`, o cálculo de porcentagens e o relacionamento entre as informações dos clientes, das visitas e dos veículos.

Além disso, organizei os resultados das consultas e apresentei as análises em um dashboard feito no Excel.

## Observação

Este é um projeto guiado, desenvolvido para fins de estudo e portfólio durante o curso **SQL para Análise de Dados: Do básico ao avançado**, da Udemy.
