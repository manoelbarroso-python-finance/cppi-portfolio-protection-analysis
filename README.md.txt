# Backtest de Estratégia de Proteção de Capital (CPPI) vs. Buy & Hold

Um estudo de caso quantitativo sobre a eficácia da estratégia *Constant Proportion Portfolio Insurance* (CPPI) para a Petrobras (PETR4) durante a Crise Financeira de 2008.

---

## Objetivo do Projeto

Este projeto investiga se uma estratégia de alocação dinâmica como o CPPI teria sido eficaz em mitigar as perdas severas de um ativo de alta volatilidade (PETR4) durante o conturbado período de 2007 a 2010, em comparação com uma abordagem passiva "Buy & Hold".

## Estrutura da Análise

O notebook segue uma narrativa analítica rigorosa:

1.  **Diagnóstico da Estratégia Passiva:** Análise completa da estratégia "Buy & Hold", validando suas premissas e quantificando seu perfil de risco-retorno.
2.  **Validação Visual (Scatter Plot):** Verificação da premissa de linearidade antes da aplicação de modelos como o CAPM.
3.  **Análise de Risco Quantitativa:** Cálculo de um conjunto abrangente de métricas para avaliar a performance ajustada ao risco e o risco de cauda.
4.  **Backtest da Estratégia CPPI:** Implementação e simulação da estratégia de proteção de capital.
5.  **Análise Comparativa Final:** Avaliação dos resultados visuais (curvas de patrimônio) e numéricos (tabela de métricas) para chegar a uma conclusão balanceada sobre o trade-off entre proteção e performance.

## Principais Métricas Utilizadas

* **Performance:** Retorno Anualizado
* **Risco Total:** Volatilidade Anualizada
* **Risco de Mercado:** Alfa e Beta (CAPM)
* **Performance Ajustada ao Risco:** Sharpe Ratio, Sortino Ratio, Calmar Ratio
* **Risco de Cauda (Tail Risk):** Skewness, Kurtosis, Max Drawdown, VaR e CVaR Histórico (95%)

## Como Executar

1.  Clone este repositório.
2.  Crie um ambiente virtual e instale as dependências listadas no arquivo `requirements.txt`:
    ```bash
    pip install -r requirements.txt
    ```
3.  Abra e execute o notebook Jupyter (`cppi_2008.ipynb`).
4. **Autor:** Manoel Barroso Marques
