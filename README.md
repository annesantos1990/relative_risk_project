<h1 align="center"> </a> Risk Relative   </h1>

**Avaliação do Risco Relativo dos clientes de um Banco**


##

<p align="center">
 
[Caso](#caso)  •  [Objetivo](#objetivo)  •  [Ferramentas](#ferramentas)   •  [Resultados e Discussão](#resultados-e-discussão)  •  [Conclusões](#conclusões)  •  [Recomendações](#recomendações)  •  [LinkedIn](#linkedin)

</p>


## Caso

Devido a um contexto de redução das taxas de juros no mercado, houve um aumento significativo da demanda por crédito, levando a um aumento de solicitações de empréstimo no banco "Super Caja". 

Devido a sobrecarga a análise manual de cada solicitação e a crescente preocupação com a taxa de inadimplência, o banco sentiu a necessidade de aumenta a pressão para identificar e mitigar os riscos associados ao crédito.

Para enfrentar esses desafios, propõe-se a automação do processo de análise de crédito utilizando técnicas de análise de dados e ciência de dados. Com o intuito de melhorar a eficiência, precisão e rapidez na avaliação das solicitações de crédito. 

 <h2>Objetivo</h2> 

- Identificar o perfil de cliente com risco de inadimplência;
- Desenvolver um score de crédito utilizando técnicas de análise de dados e avaliação do risco relativo. Este score permitirá a classificação dos solicitantes de crédito em categorias distintas de risco, com base na sua probabilidade de inadimplência.


## Ferramentas
- Gerenciamento dos dados: BigQuery (SQL), Google Colab (Python)
- Visualização de dados: Looker Studio, Google Colab (Python)
- Implementação do Modelo: Google Colab (Python)
- Apresentação dos dados: Google Colab (Python)
- Ficha técnica: Notion, GitHub


## Biblioteca e Tratamento do Dados

A limpeza, tratamento dos dados e parte das análises dos dados foi feita pelo *Big Query*.
Para mais detalhes da biblioteca e do tratamento do dados, basta clicar nesse link: [Clique aqui](https://github.com/annesantos1990/limpezadedados_reative_risk/)

## Métodos e Técnicas
Para visualizar como foi obtido o risco relativo para diferentes grupos com base nas principais variáveis desse projeto, acesse:[Clique aqui]()
Nesse repositório, além da técnica utilizada para o cálculo do risco relativo, também encontrará:
- A técnica utilizada para classificar os clientes com base no seu score de risco;
- O modelo de regressão logística.

### Visualização dos dados - Looker Studio
Parte dos gráficos que estão apresentados na seção de resultados foi feito no Looker. Para acessar o dashboard feito nessa ferramenta, clique no Link abaixo:
[Clique aqui ou na imagem](https://lookerstudio.google.com/reporting/f2abbd47-882a-4030-9f30-e8dc170a37fd)

[![looker](https://github.com/annesantos1990/relative_risk_project/assets/166059836/6d4b737d-6ddd-458b-a327-7a4663253273)](https://lookerstudio.google.com/reporting/f2abbd47-882a-4030-9f30-e8dc170a37fd)


### Análise dos dados - Google Colab
Várias análises e visualizações desse projeto foi feito no Google Colab. Para visulizar os códigos utilizados para alguns dos resultados que podem ser vista na seção de resultados, acesse o Notebook: [Clique aqui](https://colab.research.google.com/drive/1UTQUppbQ1UxoRsXbzcXoNZf4f_LWFN_I?usp=sharing)

## Apresentação do projeto
Para ver os slides com a apresentação do projeto [clique aqui.](https://github.com/annesantos1990/spotify_project/blob/main/Projeto%20Spotify.pdf)
 
## Resultados e Discussão
A análise detalhada desse projeto com os gráficos e discussões pode ser vista em nossa página pública do Notion: [Clique aqui](https://giddy-shamrock-550.notion.site/Resultados-e-Conclus-es-2099a46cca4e4d98adf88ccde83260a1?pvs=4)


Mas aqui, vou fazer um resumo dos principais resultados encontrados:
### Informações Gerais

- **Adimplência e Inadimplência**:
    - Porcentagem de Adimplentes: 98,25%
    - Porcentagem de Inadimplentes: 1,75%
- **Perfil Socioeconômico Predominante**:
    - Gênero: Masculino (60%)
    - Faixa Etária: Geração X (44 a 59 anos) (38,33%)
    - Salário: R$2.824,00 a R$5.648,00 (47,47%)
    - Número de Dependentes: 1 dependente (60,55%)
- **Grupos com Maior Taxa de Inadimplência**:
    - Faixa Etária: Millenials
    - Salário: <= R$2.824,00
    - Número de Dependentes: 7 dependentes
- **Perfil Financeiro Predominante**:
    - Tipo de Empréstimos: Imobiliários ou outros (62,87%)
    - Índice de Endividamento: Baixo (62,01%)
    - Total de Empréstimos: 6 empréstimos (9,19%)
- **Grupo com Maior Taxa de Inadimplência**:
    - Total de Empréstimos: 2 empréstimos

### Testando Hipóteses
    Para o teste dessas hipóteses, cada uma das variáveis foram separadas em 4 grupos diferentes. Para verificar  como foi feita a separação dos grupos acessar ....... e para ver os principais grupos acessar os [Resultados](https://giddy-shamrock-550.notion.site/Resultados-e-Conclus-es-2099a46cca4e4d98adf88ccde83260a1?pvs=4)

1. **Idade e Risco de Inadimplência**:
    - Clientes mais jovens (21 a 42 anos e 42 a 52 anos) apresentam maior risco de inadimplência.
    - Possivelmente, a menor estabilidade financeira e experiência de crédito contribuem para o maior risco nesse grupo etário.
2. **Número de Empréstimos e Risco de Inadimplência**:
    - Clientes com 1 a 5 e 5 a 8 empréstimos apresentam maior risco, contrariando a hipótese inicial de que mais empréstimos resultariam em maior risco.
    - A gestão eficaz da dívida parece ser mais crucial do que a quantidade de empréstimos na previsão de inadimplência, já que mesmo pessoas que pegam mais emprétimos tem uma menor probabilidade de risco de inadimplência.
3. **Atrasos no Pagamento e Risco de Inadimplência**:
    - Atrasos superiores a 90 dias são fortes indicadores de inadimplência futura.
    - A pontualidade nos pagamentos é crítica para avaliar a saúde financeira do cliente.

### Outras Observações

- **Último Salário**: Salários menores que R$3.944,00 apresentam maior risco de inadimplência.
- **Número de Dependentes**: Pessoas com um ou mais dependentes têm maior risco.
- **Índice de Endividamento**: Índices acima de 0,36 indicam maior risco.
- 
**Salário, número de dependentes e índice de endividamento são fatores críticos na previsão do risco de inadimplência.**


### Modelos de Classificação

- **Score de Crédito**:
  - Foi obtido um modelo de classificação com base no risco relativo.
  - Essa classificação contava com um ponto de corte no qual clientes com valores de score acima de 6 eram considerados "Maus Pagadores" e abaixo que 6 "Bons Pagadores"
  - Modelo apresentou limitações para classificar os "Maus Pagadores", apresentando baixo índice de acerto para esse grupo.
- **Regressão Logística**:
    -  modelo de regressão logística, ajustado para desbalanceamento das classes (class_weight='balanced'), mostrou melhores resultados.
    - Resultados: Recall de 0,95 e baixos falsos positivos.
    - Modelo eficaz em detectar potenciais inadimplentes e minimizar erros na classificação.

## Conclusões
- **Idade e Risco de Inadimplência**: Clientes mais jovens, têm um risco relativo maior de inadimplência, devido à falta de estabilidade financeira e experiência de crédito.
- **Gestão de Dívidas vs. Número de Empréstimos**: Contrariando a expectativa inicial, a quantidade absoluta de empréstimos não correlaciona diretamente com o risco de inadimplência. Gestão eficaz da dívida é mais determinante.
- **Atrasos nos Pagamentos**: Atrasos superiores a 90 dias são fortes indicadores de inadimplência futura, destacando a importância da pontualidade nos pagamentos como indicador de responsabilidade financeira.
- **Fatores de Risco Financeiro**: Salários mais baixos, maior número de dependentes e índice de endividamento elevado estão associados a um maior risco de inadimplência, evidenciando a importância da estabilidade financeira na capacidade de pagamento.
- **Desempenho do Modelo**: O modelo de regressão logística, especialmente com a técnica de *Class Weight*, mostrou-se eficaz na detecção de potenciais inadimplentes, em contraste com o modelo baseado no risco relativo que apresentou baixo desempenho.


## Recomendações
- Implementar políticas específicas de mitigação de risco para clientes mais jovens, como requisitos de garantia mais rigorosos ou limites de crédito mais baixos para novas linhas de crédito.
- Implementar medidas específicas para clientes com salários menores, incluindo limites de crédito mais baixos e condições de pagamento mais flexíveis para reduzir o risco de inadimplência.
- Ao invés de focar no número absoluto de empréstimos, o banco deve considerar a capacidade de gerenciamento de dívidas dos clientes. Isso pode incluir uma análise mais detalhada do histórico de pagamento e da proporção de renda comprometida com dívidas.
- Estabelecer um sistema de alerta para monitorar atrasos nos pagamentos superiores a 90 dias. Clientes que atingirem esse marco devem ser alvo de intervenções preventivas, como planos de reestruturação de dívida ou aconselhamento financeiro.
- Utilizar o modelo de classificação codificado nesse projeto para poder avaliar futuros clientes e os que eles já possuem para verificar o risco de inadimplência desses clientes.

## Limitações
1. **Variáveis Limitadas**: Pode haver outras variáveis relevantes que não foram consideradas neste estudo, como histórico de crédito detalhado, dados socioeconômicos mais específicos dos clientes, entre outros.
2. **Temporalidade dos Dados**: Os dados podem não refletir mudanças recentes nas condições econômicas ou comportamentais dos clientes, o que pode limitar a capacidade do modelo de prever comportamentos futuros.



##  Implementando o Sistema de Classificação
    
   Interface com a implementação do modelo de classificação dos clientes como bons ou maus pagadores feito no meu [Notebook do Google Colab](https://colab.research.google.com/drive/1UTQUppbQ1UxoRsXbzcXoNZf4f_LWFN_I?usp=sharing/) (Acesse a seção **Implementando o modelo**).
    
   Código:
    
    ```python
    # Salvando o modelo
    import joblib
    
    # Treine seu modelo (supondo que já tenha feito isso)
    model.fit(X_train, y_train)
    
    # Salve o modelo
    joblib.dump(model, 'model.pkl')
    ```
    
    ```python
    import pandas as pd
    import joblib
    import ipywidgets as widgets
    from IPython.display import display
    
    # Carregar o modelo salvo
    model = joblib.load('model.pkl')
    
    # Função para fazer a previsão
    def classify_customer(age, last_month, number_dependents, total_loan, total_90_days_overdue, total_lines, debt_ratio):
        new_data = pd.DataFrame({
            'age': [age],
            'last_month': [last_month],
            'number_dependents': [number_dependents],
            'total_loan': [total_loan],
            'total_90_days_overdue': [total_90_days_overdue],
            'total_lines': [total_lines],
            'debt_ratio': [debt_ratio]
        })
        # Certificando de que as colunas estão na mesma ordem e têm os mesmos nomes que foram usadas durante o treinamento
        new_data = new_data[model.feature_names_in_]
        prediction = model.predict(new_data)
        result = "Risco de Inadimplência" if prediction[0] == 1 else "Sem Risco de Inadimplência"
        print(f"Previsão: {result}")
    
    # Criar widgets
    age = widgets.FloatText(description='Idade:', min=18, max=100, value=30)
    last_month = widgets.FloatText(description='Último Salário:', min=1, max=100000, value=1)
    number_dependents = widgets.FloatText(description='Dependentes:', min=0, max=10, value=2)
    total_loan = widgets.FloatText(description='Total de Empréstimos:', value=5000)
    total_90_days_overdue = widgets.FloatText(description='90+ Dias Atraso:', min=0, max=100, value=0)
    total_lines = widgets.FloatText(description='Linhas Totais:', min=1, max=20, value=3)
    debt_ratio = widgets.FloatText(description='Índice de Endividamento:', min=0.0, max=100.0, step=0.01, value=0.3)
    
    # Botão para fazer a previsão
    button = widgets.Button(description="Classificar Cliente")
    
    # Chamar a função quando o botão é clicado
    def on_button_clicked(b):
        classify_customer(age.value, last_month.value, number_dependents.value, total_loan.value, total_90_days_overdue.value, total_lines.value, debt_ratio.value)
    
    button.on_click(on_button_clicked)
    
    # Mostrar widgets
    display(age, last_month, number_dependents, total_loan, total_90_days_overdue, total_lines, debt_ratio, button)
    
    # Debug: Imprimir as colunas do conjunto de treinamento e as do new_data
    #print(model.feature_names_in_)
    new_data = pd.DataFrame({
        'age': [age.value],
        'last_month': [last_month.value],
        'number_dependents': [number_dependents.value],
        'total_loan': [total_loan.value],
        'total_90_days_overdue': [total_90_days_overdue.value],
        'total_lines': [total_lines.value],
        'debt_ratio': [debt_ratio.value]
    })
    #print(new_data.columns)
    ```
    
   **Interface:**
    
   Na interface, é possível colocar as informações do cliente e ao apertar o botão **Classificar Cliente,** o programa classifica o cliente em “Risco de Inadimplência” e “Sem Risco de Inadimplencia”
    
   ![interface](https://github.com/annesantos1990/relative_risk_project/assets/166059836/c1c9c667-4b77-448c-8f65-fe820b3ea211)


## LinkedIn

https://www.linkedin.com/in/eslaine-santos-e-santos-46159a28/

Obrigada por sua atenção!




