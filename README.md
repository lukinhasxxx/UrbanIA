# UrbanIA

Esse projeto de Machine Learning foi realizado no 1º semestre de 2023 ja USJT para entender melhor sobre Inteligência Artificial e como dados funcionam, como modelar e interpretar. Esses modelos foram feitos utilizando a linguagem Python e bibliotecas como Pandas e Scikit-Learning.
No estudo foram feitos dois teste, um com modelo preditivo e um com modelo classificatório, o que é mais indicado nesse contexto.

# Fonte

Utilizamos um dataset do Kaggle que fica neste link:
https://www.kaggle.com/datasets/crisparada/brazilian-cities?resource=download

# Descrição do projeto

Objetivo:
O objetivo deste projeto é avaliar a qualidade de vida nas cidades brasileiras utilizando o IDHM (Índice de Desenvolvimento Humano Municipal). Embora o IDHM seja um bom indicador geral, queremos ver se modelos de machine learning (ML) podem oferecer uma análise mais detalhada e útil, classificando as cidades em categorias como ruim, média ou boa para viver.

Preparação dos Dados:

Tratamento e normalização: Dados com valores ausentes ou inconsistentes foram ajustados. Também normalizamos os dados para garantir que tudo estivesse no mesmo padrão e pronto para análise.
Análise Estatística: Calculamos médias, desvios padrão e outras estatísticas para entender melhor os resultados/dados.

# Variável alvo e colunas que foram consideradas na análise
Variável alvo:
IDHM (Índice de Desenvolvimento Humano Municipal)
Descrição: Mede o desenvolvimento humano em uma escala de 0 a 1, considerando educação, renda per capita e saúde. Quanto mais próximo de 1, melhor o desenvolvimento da cidade.

Colunas Usadas na Análise:
COMP_E (Número de Instituições de Saneamento)

Descrição: Indica a quantidade de instituições de saneamento básico em um município. Reflete as condições de saúde pública, com cidades com mais instituições possuindo melhores serviços de saneamento.
COMP_O (Número de Instituições de Segurança Social)

Descrição: Contabiliza o número de instituições de segurança social, como empresas e organizações que oferecem serviços de proteção social. Ajuda a avaliar a segurança e proteção social em cada município.
COMP_Q (Número de Companhias de Saúde e Serviços Sociais)

Descrição: Refere-se à quantidade de hospitais e serviços de saúde disponíveis em um município. É crucial para avaliar a qualidade do sistema de saúde local, já que o IDHM inclui saúde como um dos seus pilares.
GDP_CAPITA (Produto Interno Bruto per Capita)

Descrição: Calcula a riqueza média por habitante, dividindo o PIB total da cidade pelo número de habitantes. Este indicador ajuda a entender a prosperidade econômica média dos moradores.
IDHM_Educacao (Índice de Educação)

Descrição: Mede a qualidade da educação em um município. É um dos componentes do IDHM, refletindo o acesso e qualidade dos serviços educacionais disponíveis.
IDHM_Longevidade (Índice de Longevidade)

Descrição: Avalia a expectativa de vida no município, outro componente do IDHM. Reflete a qualidade geral de vida, levando em conta saúde e outros fatores relacionados à longevidade.


# Modelos de Machine Learning Aplicados
Foram utilizados 3 modelos de Machine Learning para tal

  Árvore de Decisão: Criamos um modelo que divide as cidades em categorias com base em diferentes critérios. Isso ajuda a prever a qualidade de vida usando as características das cidades. Utilizamos o modelo de regressão e o modelo de classificação.

  K-Nearest Neighbors (KNN): Este modelo classifica cidades com base na proximidade de características com outras cidades conhecidas. Verificamos se a semelhança entre cidades pode prever a qualidade de vida de forma eficaz.

  Naive Bayes: Um modelo probabilístico que classifica cidades com base nas características observadas. Esse modelo ajuda a entender como cada característica contribui para a classificação da qualidade de vida.

Classificação e Validação:

  Comitê de Classificação: Usamos as previsões dos diferentes modelos para classificar as cidades como ruim, média ou boa para viver.
  Comparação com IDHM: Comparamos as previsões dos modelos com o IDHM para ver se eles fornecem uma visão adicional ou diferente da qualidade de vida.

# Importância

Identificação de padrões: Usando ML, podemos encontrar padrões e relações entre diferentes variáveis que não são óbvias a primeira vista. Isso ajuda a entender melhor o que afeta a qualidade de vida, fora somente uma análise de "Se o IDH está maior, logo é melhor"

Detecção de outliers: A análise pode identificar cidades que, apesar de ter um IDHM baixo, podem ter características que sugerem uma melhor qualidade de vida do que o esperado, e vice-versa.

Orientação para políticas Públicas: Os resultados podem ajudar na formulação de políticas públicas, indicando quais áreas (como educação, saúde, segurança) precisam de mais atenção para melhorar a qualidade de vida.

Decisões informadas: Este projeto fornece uma ferramenta para avaliar a qualidade de vida nas cidades com base em uma análise mais completa, alem do IDHM.
