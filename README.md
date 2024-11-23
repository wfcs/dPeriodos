# Dimensão Períodos

Um script M para criar uma tabela dinâmica de períodos úteis para análises temporais em Power BI. Este script gera intervalos de datas pré-definidos, como "Hoje", "Ontem", "Esta Semana", "Mês Atual", entre outros, e pode ser adaptado conforme as necessidades.

## 📋 Funcionalidades

- Criação de períodos personalizados com intervalos definidos, incluindo:
  - Hoje e Ontem.
  - Semana Atual e Semana Passada.
  - Últimos 7 e 15 dias.
  - Mês Atual e Mês Passado.
  - Últimos 3 e 6 meses.
  - Ano Atual.
- Possibilidade de personalização para adicionar novos períodos ou ajustar os existentes.
- Organização por uma coluna de ordem para facilitar a classificação no Power BI.

## 🔧 Requisitos

- **Power BI Desktop** ou qualquer ferramenta compatível com **Power Query**.
- Versão mínima do Power BI para suporte a funções e scripts M avançados.

## 🚀 Como usar

1. **Copie o script**:
   Copie o código do arquivo `DimensaoPeriodos.m` (fornecido neste repositório).

2. **Cole no Editor de Consultas**:
   - Abra o Power BI.
   - No Editor de Consultas, clique em **Nova Fonte** > **Consulta em Branco**.
   - Acesse **Exibir Avançado** e cole o script.

3. **Carregue os dados**:
   Clique em **Fechar e Aplicar** para carregar a tabela no modelo de dados.

## 📜 Estrutura da Tabela

| Coluna      | Tipo    | Descrição                                              |
|-------------|---------|-------------------------------------------------------|
| `Data`      | Data    | Datas dentro do intervalo definido para cada período. |
| `Periodo`   | Texto   | Nome do período (ex.: "Hoje", "Semana Passada").       |
| `Ordem`     | Número  | Ordem para facilitar a classificação dos períodos.    |

## 🛠️ Personalização

- **Adicionar novos períodos**:
  Adicione entradas na lista `Intervalos`, seguindo a estrutura:
  ```m
  {"Nome do Período", DataInicial, DataFinal, Ordem}
  ```
### Próximos passos
- Confirme se há alguma informação adicional ou ajustes necessários.
