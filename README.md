# Projeto SQL 2 - Dashboard de Perfil dos Clientes

## Sobre o projeto

Esse foi o segundo projeto guiado que desenvolvi durante o curso **SQL para Análise de Dados: Do básico ao avançado**, ministrado pela Midori Toyota na Udemy.

No projeto, analisei o perfil dos clientes que visitaram um e-commerce de veículos e os principais tipos de veículos procurados por eles.

Realizei as consultas no PostgreSQL por meio do pgAdmin. Depois, organizei os resultados no Excel e usei esses dados para montar um dashboard com as principais análises.

## Objetivo

O objetivo foi criar um dashboard para entender melhor o perfil dos clientes e os interesses demonstrados nas visitas ao e-commerce. Para isso, analisei gênero, status profissional, faixa etária e faixa salarial.

Também observei a distribuição das visitas por classificação dos veículos, faixa de idade e modelo.

## Perguntas de negócio

Para orientar as análises, trabalhei com sete perguntas:

1. Qual é a distribuição dos clientes por gênero?
2. Quais são os status profissionais mais frequentes entre os clientes?
3. Qual é a faixa etária predominante entre os clientes?
4. Qual é a faixa salarial predominante entre os clientes?
5. Os visitantes demonstram maior interesse por veículos novos ou seminovos?
6. Quais faixas de idade dos veículos recebem mais visitas?
7. Quais modelos de veículos registraram o maior número de visitas?

## Indicadores e análises apresentados

O dashboard reúne sete análises:

- Distribuição dos clientes por gênero;
- Distribuição por status profissional;
- Distribuição por faixa etária;
- Distribuição por faixa salarial;
- Visitas a veículos novos e seminovos;
- Visitas por faixa de idade dos veículos;
- Modelos de veículos com maior número de visitas.

## Principais resultados

A análise dos resultados permitiu identificar alguns padrões no perfil dos clientes e nos veículos visitados:

- **Gênero:** entre os 25.109 clientes analisados, 15.106 foram classificados como femininos (60,16%) e 10.003 como masculinos (39,84%). Essa classificação foi estimada a partir dos primeiros nomes, conforme a referência utilizada na consulta.
- **Status profissional:** clientes com vínculo CLT representam aproximadamente 64,94% dos registros.
- **Faixa etária:** a faixa de 20 a 40 anos concentra a maior parcela dos clientes, com 41,27%.
- **Faixa salarial:** a faixa de R$ 5 mil a R$ 10 mil reúne 71,03% dos clientes.
- **Veículos novos e seminovos:** foram registradas 29.418 visitas a seminovos (96,2%) e 1.162 a veículos classificados como novos (3,8%).
- **Idade dos veículos:** a faixa de 8 a 10 anos concentrou a maior parcela das visitas, com 24,77%, seguida pelos veículos com mais de 10 anos, com 22,92%.
- **Modelos mais visitados:** FIAT PALIO liderou com 1.699 visitas, seguido por VW GOL (1.547) e FIAT UNO (1.385). O top 10 também inclui FORD FIESTA (1.221), RENAULT SANDERO (1.039), CHEVROLET CELTA (1.028), CHEVROLET ONIX (1.012), VW FOX (983), FORD KA (968) e HYUNDAI HB20 (768).

As análises completas, com gráficos, interpretações e observações sobre os resultados, estão disponíveis no documento complementar:

[**Consultar a análise completa dos resultados (PDF)**](An%C3%A1lise%20dos%20resultados/Projeto2-An%C3%A1lise-dos-Resultados.pdf)

## Banco de dados

A base fictícia utilizada no projeto representa as operações de um marketplace de veículos.

Principais tabelas consultadas:

- `sales.funnel`: registros das visitas realizadas no e-commerce;
- `sales.customers`: informações dos clientes;
- `sales.products`: informações dos veículos;
- `temp_tables.ibge_genders`: tabela de referência utilizada para estimar o gênero a partir dos primeiros nomes.

## Recursos SQL aplicados

Durante o desenvolvimento, utilizei recursos do SQL para consultar, relacionar, agrupar e analisar os dados, incluindo:

- Consultas com `SELECT`;
- Filtros com `WHERE`;
- Relacionamentos entre tabelas com `JOIN`;
- Agrupamentos com `GROUP BY`;
- Ordenação com `ORDER BY`;
- Funções de contagem;
- Expressões de tabela comuns com `WITH` (CTEs);
- Subqueries;
- Classificações com `CASE`;
- Tratamento e extração de informações de datas;
- Conversão de tipos;
- Cálculos de porcentagem;
- Criação de faixas etárias, salariais e de idade dos veículos.

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
- [Consultar a análise completa dos resultados (PDF)](An%C3%A1lise%20dos%20resultados/Projeto2-An%C3%A1lise-dos-Resultados.pdf)

## Verificações adicionais

Além de desenvolver as consultas para responder às perguntas de negócio, também conferi os resultados apresentados nas planilhas para verificar os totais, os percentuais e a ordenação das principais categorias.

As verificações incluíram:

- Conferência dos totais e percentuais das distribuições de gênero, status profissional, faixa etária e faixa salarial;
- Conferência do total de visitas a veículos novos e seminovos;
- Conferência dos percentuais por faixa de idade dos veículos;
- Conferência da ordenação dos dez modelos com maior número de visitas.

Essas conferências foram realizadas sobre os resultados disponíveis no Excel. Elas não representam uma auditoria completa da base original nem a reexecução integral de todas as consultas.

Alguns pontos também precisam ser considerados na interpretação:

- O gênero foi estimado a partir do primeiro nome, com uso de uma tabela de referência; portanto, não corresponde a uma informação autodeclarada pelos clientes.
- A faixa etária é calculada com base em `CURRENT_DATE`, então os resultados podem mudar quando as consultas forem executadas novamente.
- A idade dos veículos considera a diferença entre o ano da visita e o ano do modelo, e não uma diferença exata entre datas.
- A classificação entre novo e seminovo segue a regra aplicada na consulta: veículos com diferença de até dois anos entre o ano da visita e o ano do modelo são classificados como novos; acima disso, como seminovos.
- A quantidade de visitas representa registros de acesso aos veículos. Um mesmo cliente pode aparecer mais de uma vez, portanto os resultados não representam necessariamente pessoas únicas.

## Estrutura do repositório

```text
sql-analise-perfil-clientes/
├── README.md
├── Dashboard/
│   └── Projeto 2 - Dashboard de Perfil dos Clientes.xlsx
├── Imagens/
│   └── Print Dashboard Projeto 2.jpg
├── SQL/
│   └── Querys Projeto 2 - Dashboard de Perfil dos Clientes.sql
└── Análise dos resultados/
    └── Projeto2-Análise-dos-Resultados.pdf
```

## Aprendizados

Com esse projeto, consegui aplicar SQL para analisar o perfil dos clientes e identificar os principais interesses relacionados aos veículos disponíveis no e-commerce.

Também pratiquei o relacionamento entre tabelas, a criação de categorias e faixas com `CASE`, o cálculo de porcentagens e o tratamento de informações de datas.

Além disso, organizei os resultados das consultas e apresentei as análises em um dashboard feito no Excel, complementando a apresentação com um relatório de interpretação dos resultados.

## Observação

Este é um projeto guiado, desenvolvido para fins de estudo e portfólio durante o curso **SQL para Análise de Dados: Do básico ao avançado**, da Udemy.
