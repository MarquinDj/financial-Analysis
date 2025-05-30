# Análise de Dados de Compras da London Fire Brigade

## Resumo
Este workflow utiliza a plataforma KNIME para processar e analisar dados de compras da London Fire Brigade. Ele gera insights como totais gerais, tendências de gastos, análise de VAT e relatórios por fornecedor, departamento e categoria.

## Dados e Caso de Uso
- **Fonte dos Dados**: [London Data Store](https://data.london.gov.uk/dataset/lfb-payments-over-f250---2022-23)
- **Descrição**: Dados reais de compras com 10 colunas e cerca de 6000 linhas por mês.
- **Objetivo**: Processar 3 meses de dados para:
  - Calcular totais gerais e tendências.
  - Analisar VAT.
  - Gerar relatórios por fornecedor, departamento e categoria.

## Estrutura do Workflow
1. **Acesso aos Dados**:
   - Leitura de arquivos em formatos XLSX e CSV.
   - Conexão com banco de dados para leitura de tabelas.

2. **Limpeza dos Dados**:
   - Remoção de valores ausentes e duplicados.
   - Renomeação e transformação de colunas.
   - Criação de metanodos para organização.

3. **Transformação e União dos Dados**:
   - Manipulação e concatenação de tabelas.
   - Remoção de duplicatas e renomeação de colunas.

4. **Agregação dos Dados**:
   - Cálculo de totais por fornecedor, departamento e categoria.
   - Pivotagem e agrupamento por mês.

5. **Visualização e Exportação**:
   - Geração de gráficos (e.g., Bar Chart).
   - Exportação para CSV e Excel.

## Requisitos
- **Plataforma**: KNIME Analytics Platform
- **Extensões Necessárias**:
  - Database Connector
  - Excel Reader/Writer
  - Data Manipulation
  - Visualization

## Como Executar
1. Abra o KNIME Analytics Platform.
2. Importe o workflow.
3. Configure os caminhos para os arquivos de entrada.
4. Execute o workflow completo ou por seções.

## Resultados
- **Visualizações**:
  - TOP 20 fornecedores por valor gasto.
  - Totais por departamento e categoria.
  - Análise de VAT por fornecedor.
  - Tendências de gastos ao longo dos três meses.
- **Arquivos de Saída**:
  - Relatórios em CSV e Excel.