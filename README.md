# Projeto de Dashboard: Análise de Consumo e Informações dos Usuários

Este repositório contém um projeto desenvolvido no Power BI, com um dashboard que analisa dados de consumo de conteúdos e perfis de usuários. O objetivo é fornecer insights para melhorar o engajamento na plataforma e compreender padrões de uso. A proposta do projeto é simular uma empresa fictícia que vende cursos para estudantes de medicina.

## 📂 Arquivos no Repositório

- **Base_P_Projeto.xlsx**: Planilha contendo os dados brutos sobre consumo de conteúdos e informações dos usuários.
- **projeto_dados.pbix**: Arquivo do Power BI com o dashboard interativo, incluindo transformações e visualizações.

## 🪯 Limpezas e Transformações dos Dados

As seguintes ações foram realizadas para preparar os dados para análise:

### Renomeação das Colunas

- Todas as colunas foram renomeadas seguindo a convenção `snake_case` para padronização.

### Formatação de CPFs

- Padronizados para conter 11 dígitos, adicionando zeros à esquerda, quando necessário.
- Formatação no padrão `XXX.XXX.XXX-XX` usando manipulações de texto.

### Ajustes de Datas

- Colunas contendo informações de datas foram convertidas para o formato correto.

### Tradução de Dados

- Todas as informações em inglês foram traduzidas para português.

### Limpeza de Dados Indevidos

- Dados inconsistentes ou incorretos foram corrigidos ou removidos.

### Formatação de Cursos

- Nomes de cursos foram padronizados.

### Criação de Colunas Calculadas

- **Dia da Semana**: Criada a partir da coluna `created_at`, usando funções DAX.
- **Semestre Atual**: Concatenado com o símbolo º (exemplo: 5º).
- Outras colunas calculadas foram criadas com base nos dados disponíveis para enriquecer as análises.

## 🔁 Gráficos e Visualizações

O dashboard foi dividido em duas páginas com as seguintes visualizações:

### Página 1: Consumo de Conteúdo

- **Cursos com Mais Tempo de Consumo em Vídeo (Treemap)**:
  - Mostra os cursos com maior consumo em vídeos, agrupados visualmente.

- **Total de Segundos Assistidos (Cartão)**:
  - Exibe o valor total de segundos consumidos em todos os conteúdos.

- **Total de Acessos (Cartão)**:
  - Número total de acessos registrados na plataforma.

- **Consumo de Cada Tipo de Conteúdo (Gráfico de Pizza)**:
  - Mostra a distribuição de consumo por tipo de conteúdo (vídeo, resumo, etc.).

- **Consumo por Universidade (Gráfico de Barras)**:
  - Quantidade de acessos segmentados por universidade.

- **Conteúdo Consumido por Período (Arvore Hierárquica)**:
  - Relaciona conteúdos consumidos a períodos específicos.

- **Acessos por Dia da Semana (Gráfico de Barras)**:
  - Exibe a frequência de acessos durante os dias da semana.

- **Consumo por Usuário (Gráfico de Barras Horizontais com Rolagem)**:
  - Mostra o consumo individual de cada usuário, baseado na contagem de linhas associadas ao identificador do usuário.

### Página 2: Informações dos Usuários

- **Cadastros por Período (Arvore Hierárquica)**:
  - Analisa o volume de cadastros segmentados por períodos.

- **Usuários em Cada Semestre (Gráfico de Pizza)**:
  - Exibe a distribuição de usuários por semestre atual.

- **Perfil dos Assinantes (Gráfico de Barras)**:
  - Mostra o perfil dos usuários (aluno ou professor).

- **Usuários por Universidade (Gráfico de Pizza)**:
  - Quantidade de usuários assinantes de cada universidade.

- **Usuários por Curso Assinado (Gráfico de Barras)**:
  - Mostra a quantidade de usuários matriculados em cada curso.

- **Quantidade Total de Usuários Assinantes (Cartão)**:
  - Exibe o número total de usuários assinantes na plataforma.

- **Quantidade de Universidades (Cartão)**:
  - Total de universidades presentes na plataforma.

## 📌 Insights Obtidos

Com base nos dados analisados, foram identificados os seguintes insights estratégicos:

- **Gamificação para Usuários Engajados**:
  - Premiar usuários com maior engajamento pode estimular o consumo.

- **Lançamento de Conteúdos em Dias com Menor Engajamento**:
  - Publicar conteúdos em dias menos movimentados para equilibrar o consumo.

- **Eventos nos Dias de Menor Acessos**:
  - Promover eventos para aumentar o engajamento nos dias com menos atividade.

- **Motivação para Consumo de Quizzes**:
  - Estimular o consumo de conteúdos do tipo "quiz", que pode aumentar o aprendizado ativo.

## 🚀 Como Executar

1. Certifique-se de ter o Microsoft Power BI instalado.
2. Faça o download dos arquivos deste repositório.
3. Abra o arquivo `projeto_dados.pbix` no Power BI para explorar o dashboard interativo.

## 🛠️ Ferramentas Utilizadas

- **Microsoft Power BI**: Para desenvolvimento do dashboard e modelagem de dados.
- **Excel**: Para visualização e manipulação inicial dos dados.
