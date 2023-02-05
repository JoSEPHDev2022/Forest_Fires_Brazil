<kbd><img src="https://www.preferredbynature.org/sites/default/files/2020-03/FireTopCapture.PNG" width=1000 height=350></kbd>

<h1>
    <p align="center">
        Incêndios Florestais Brasileiros (1998-2017) 🔥🌳
    </p>
</h1>

---

## Objetivo 🎯

Nesse projeto, o objetivo foi realizar uma análise exploratória de um [Dataset](https://www.kaggle.com/datasets/gustavomodelli/forest-fires-in-brazil) que contém dados da série histórica de incêndios florestais no Brasil entre 1998 e 2017. O foco dessa análise exploratória foi buscar compreender esses incêndios que afetam a mata brasileira, analisando diversos fatores como:

- Região dos estados afetados pelos incêndios;
- Em qual período de qual governante os incêndios ocorreram e com qual intensidade;
- Análise dos incêndios com um olhar focado nas estações do ano.
 
Em mais detalhes, outro objetivo é concluir essa análise seguindo alguns passos:

- 🎲 Checar as características gerais dos dados, como formato, tipo dos dados, quantidade de valores nulos e outliers (se existirem), etc;

- 🧹 Realizar a limpeza e tratamento necessários dos dados;

- 📊 Utilizar de visualizações gráficas para gerar insights acerca dos dados;

Também criei um Dashboard no PowerBI utilizando os dados limpos no Python, com o objetivo de criar uma visualização dinâmica dos dados encotrados na análise exploratória.

--- 

## Tecnologias Utilizadas 💻

[![Kaggle](https://img.shields.io/badge/Kaggle-035a7d?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/) ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white) ![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

---

## Conteúdos do Repositório 📁

Neste reposítório, você vai encontrar:

> Uma pasta chamada **data** que possui o arquivo csv da base de dados utilizado para a análise;
>
> Uma pasta chamada **dashboard** que contém prints do Dasboard e o arquivo .pbix em si;
>
> Um Notebook chamado **relatorio.ipynb** que contém o projeto em si.

---

## Run-down do Projeto 📑

Como um resumo de todo o processo de desenvolvimento do projeto:

- ***Primeira Etapa: Coleta e Descrição***

> O primeiro passo foi coletar os dados do Kaggle e trazê-los para o VScode, onde foi criado o Jupyter Notebook para as análises.
> Essa primeira etapa foi onde realizei as primeiras análises descritivas dos dados, buscando compreender as características gerais deles como:
>   - Dimenões, tipos de dados, quantidade de nulos, outliers, distribuição dos dados.
>
> Enfim, a primeira etapa foi de reconhecimento, para que eu pudesse conhecer os dados na qual estava trabalhando.

- ***Segunda Etapa: Limpeza, Tratamento e Adições***

> Nessa segunda etapa o objetivo era tratar os dados e corrigir características que não achei ideal no Dataset, além disso, foi aqui que inseri novas colunas com novos dados ao Dataset original. Em mais detalhes, adicionei quatro novas variáveis aos dados:
>   - **UF** > Uma coluna que contém a Unidade da Federação de cada estado dos dados (SP, RJ, BA, etc). O objetivo dessa coluna era de proporcionar uma padronização para a identificação dos estados, tando para a análise exploratória tanto para a criação do Dashboard no Power BI.
>
>   - **Region** > Uma coluna que contém a região em que cada estado pertence no Brasil. A criação dessa coluna foi realizada para dar mais profundidade as análises possíveis com os dados.
>
>   - **President** > A coluna mais relevante criada para esse dataset, ela armazena o nome e mandato do presidente em vigência no ano em que os incêndios ocorreram. Essa coluna proporciona muita dinâmica e profundidade para a análise, sendo ela a responsável pela maior parte das análises e insights históricos retirados dos dados.
>
>   - **Season** > Uma coluna que informa em qual estação do ano cada incêndio ocorreu. Essa coluna proporciona uma visão mais aprofundada das relações entre estação do ano e incêndios florestais e também foi muito útil durante as análises.
>
> Com a limpeza dos dados e criação de novas variáveis, a próxima (e principal) etapa vem a seguir.

- **Terceira Etapa: Análises, Insights e Visualizações**

> Como o próprio nome sugere, foi nessa etapa que o trabalho central de análise ocorreu. Nela, busquei utilizar da melhor forma possível todas as variáveis disponíveis nos dados (tanto originais quanto as criadas por mim psoteriormente), com o objetivo de responder a 4 perguntas centrais:
>
> 1. Quais os estados e regiões mais e menos afetados por incêndios durante toda a série histórica?
>2. Durante qual período de qual governante brasileiro tivemos mais e menos incêndios no Brasil?
> 3. Como o número de incêndios nas diferentes regiões e estados se comportam ao longo da série histórica?
> 4. Qual a estação do ano em que se houve mais e menos incêndios no Brasil?
>
> Ao responder essas perguntas, pude desenvolver análises e estabelecer relações entre as colunas e dados fornecidos pelo Dataset.

- **Quarta Etapa: Criação de um Dashboard no Power BI**
> Utilizando o Power BI, subi os dados para a plataforma e tive que realizar pequenas mudanças nos dados importados:
> - Junção das colunas `Year` e `Month` em uma única coluna no estilo Datetime. Para essa modificação, foi utilizada a linguagem DAX.
>
> Com essas alterações, foram criados dois relatórios:
> - **Estados e Regiões**: Visão acerca dos incêndios florestais com um foco nos estados e regiões do Brasil;
> - **Governos e Estações do Ano**: Visão dos incêndios lorestais com um enfoque nos diferentes governantes brasileiros e estações do ano.
> 
> Abaixo, seguem imagens do Dashboard.

---

## Dashboard 🗺️

![capa_dash](https://github.com/JoSEPHDev2022/Forest_Fires_Brazil/blob/main/dashboard/capa.png)

---

![estados_regioes](https://github.com/JoSEPHDev2022/Forest_Fires_Brazil/blob/main/dashboard/estados_regiao.png)

---

![governos_clima](https://github.com/JoSEPHDev2022/Forest_Fires_Brazil/blob/main/dashboard/governos_clima.png)

---

## Contatos 📧

Quer me mandar uma mensagem? Tem dicas e conselhos de melhoria e aprimoramento do projeto? Você pode entrar em contato comigo por e-mail ou acessando meu perfil do LinkedIn, estou sempre por lá!

e-mail: jl_ferreira_16@hotmail.com

LinkedIn: [![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jose-luiz-ferreira-junior/)