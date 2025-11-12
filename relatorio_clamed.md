# Mini-Projeto — Análise de Dados de Saúde (CLAMED)

**Etapa 6 — Conclusão e Entrega Final**

## 1) Principais padrões identificados

- **Gênero equilibrado** entre Masculino e Feminino.
- **Condições médicas** (Diabetes, Hipertensão, Câncer, Obesidade, Asma, Artrite) com **frequências semelhantes**.
- Predomínio de pacientes **Adultos** e **Idosos** nas faixas etárias.
- **Custo médio de tratamento** varia **entre condições médicas**.
- **Hospitais** e **seguradoras** com distribuição uniforme, sem concentração excessiva.

## 2) Comportamentos inesperados

- Valores **negativos** em `Billing Amount` (possíveis estornos ou dados artificiais).
- **Correlação muito baixa** entre **idade** e **custo**, indicando grande dispersão.
- Algumas datas aparecem com contagem muito alta → forte evidência de dataset sintético.

## 3) Hipóteses para análises futuras

- Condições médicas diferentes podem afetar **tempo de internação**.
- Custos podem depender do **hospital** (estrutura, complexidade de atendimento).
- Seguradoras podem influenciar o **valor final** por regras de cobertura.
- Faixas etárias podem apresentar variabilidade própria de custo.

## 4) Visualizações incluídas

- Gráfico de barras — **custo médio por condição médica**.
  ![Custo por condição médica](custo%20por%20condicao.jpg)

- Gráfico de dispersão — **idade vs custo**.
  ![Relação entre idade e custo](relacao%20entre%20idade%20e%20custo.jpg)

- Gráfico de pizza — **proporção por seguradora**.
  ![Proporção por seguradora](proporcao%20paciente%20seguradora.jpg)

## 5) Confiabilidade após limpeza

- Remoção de duplicados.
- Normalização de nomes e categorias.
- Conversão e ajuste de datas.
- Criação de `length_of_stay`.
- Criação de `age_group`.
- Normalização z-score via `billing_amount_z`.
- Nenhum valor ausente após tratamento.

## 6) Conclusão

O fluxo completo — **importação, limpeza, exploração, enriquecimento e visualização** — permitiu identificar padrões relevantes e levantar novas hipóteses. O dataset está pronto para análises mais profundas, especialmente envolvendo custos, internação e diferenças entre hospitais e seguradoras.
