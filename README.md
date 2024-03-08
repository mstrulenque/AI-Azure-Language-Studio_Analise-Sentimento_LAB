# AI-Azure-Language-Studio_Analise-Sentimento_LAB

---

`LAB Utilizando` : Microsoft **Azure AI | Language Studio**

`Descrição do LAB` : 

LAB - com o passo-a-passo em texto e print screen, configurando o recurso `Language Service`, para realização de atividade de análise de Sentimentos .
     
`Ações que serão realizadas` :

 - `Azure`:
   - Criar um Resource Group
   - Provisionar o Resource `Language Service`
     
  - `Language Studio`
    
     - Configuração:
       -   Selecionar a Instancia do Recurso aprovisionado na Azure
    
     - LAB:
       - Teste 1:
         - Selecionar o Idioma do Texto que iremos utilizar para Análise de Sentimentos.
         - Selecionar o Arquivo 1
           (arquivo encontra-se na pasta "inputs" neste repositório do GitHub)
         - Verificar os resultados:
           - "Sentence Sentiment"
           - "Target" identificado no texto. (objeto/produto que o texto esta referindo)
           - "Assessments" indentificados no texto (palavra associada ao objeto/produto com a classificação: positivo ou negativo)  
       - Teste 2:
         - Selecionar o Idioma do Texto que iremos utilizar para Análise de Sentimentos.
         - Selecionar o Arquivo 2
           (arquivo encontra-se na pasta "inputs" neste repositório do GitHub)
         - Verificar os resultados:
           - "Sentence Sentiment"
           - "Target" identificado no texto. (objeto/produto que o texto esta referindo)
           - "Assessments" indentificados no texto (palavra associada ao objeto/produto com a classificação: positivo ou negativo)  
       - Teste 3:
         - Selecionar o Idioma do Texto que iremos utilizar para Análise de Sentimentos.
         - Selecionar o Arquivo 3
           (arquivo encontra-se na pasta "inputs" neste repositório do GitHub)
         - Verificar os resultados:
           - "Sentence Sentiment"
           - "Target" identificado no texto. (objeto/produto que o texto esta referindo)
           - "Assessments" indentificados no texto (palavra associada ao objeto/produto com a classificação: positivo ou negativo)  

`Arquivos deste Repositório GitHub` : <br>

▶️  `README.MD`                  - Passo-a-Passo com Print Screen's; <br><br>
▶️  `inputs/opiniao-celular-maria_p.txt`   - texto do Teste 1, para analisar o sentimento; <br>
▶️  `inputs/opiniao-celular-joao_n.txt`    - texto do Teste 2, para analisar o sentimento; <br>
▶️  `inputs/opiniao-celular-jose_p_n.tx    - texto do Teste 3, para analisar o sentimento; <br>

---

# 👷 - Preparando Ambiente para realizar o LAB: 


## 1 - Acesse o `Portal Azure`: <a href="https://portal.azure.com"> <img width="99" alt="https://portal.azure.com" src="https://github.com/mstrulenque/dio-lab-azure-ML/assets/63933792/4665d721-98e7-4c24-bc97-f7540d64a917"></a> 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; https://portal.azure.com


## 2 - Faça o Login com a sua Conta 🔐
  
## 3 - Crie e Configure um Resource (Recurso)

3.1 - Na `Home`, Clique em `Create Resource`
<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="228" alt="image" src="https://github.com/mstrulenque/AI-Azure-Vision-Studio_Detect-FaceLAB/assets/63933792/dcefd5aa-08ad-42b2-896d-398dc968cbf7">

3.2 - Na página `Create a Resource` no Menu Lateral Esquerdo: <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
▶️  Em `Categories`, Clique em `AI + Machine Learning` ;  <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
▶️  Clique no Link `Create` do Serviço `Language service` na coluna esquerda;  <br>
<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="436" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/952cb67c-14b3-4239-b625-71a45c8bc365">

3.3 - Selecionar Features Adicionais: <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.3.1 - `Custom Features` - Selecionar `Custom text classification, ... Custom sentiment analysis ....`; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.3.2 - Clicar no botão `Continue to Create your Resource`; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="436" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/5e1732b1-b710-45d3-9cd2-6f075c367cbb">

3.4 - Criar Resource Group preenchendo os campos: <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.1 - `Subscription` - Selecione a sua Subscription; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.2.1 - `Resource Group` - Clique no link `Create New` abaixo do campo; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.2.2 - `Resource Group` - Digite um nome para seu Resource Group; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.2.3 - `Resource Group` - Clique no botão `OK`; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.2.4 - `Resource Group` - o nome que você criou aparecerá selecionado no campo de escolha "Resource Group", <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
caso contrário escolha na lista; <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="436" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/e503fade-4a8a-40aa-813b-713a6fa44ec2">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.3 - `Region` - escolha uma Region da Cloud para criação do workspace; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.4 - `Name` Instance = `instanceLanguageLab` <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.5 - `Pricing tier` = `Free F0 (5K Transactions per 30 days)` <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.6 - `Storage` <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.6.1 - `New/Existing storage Account` - Clique em `New Storage Account`; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.6.2 - `Storage Account Name` - digite um nome para a Storage Account; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.6.3 - `Storage Account Type` - escolha a Storage Account type; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.7 - Clique no botão `Review + Create`; <br>
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="436" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/3e27c53c-6978-4e2b-aa4e-22cadf4311da">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.8 - Revise os Dados e estando tudo correto, Clique no botão `Create`; <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="436" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/f2f0b96c-90a3-4fbe-beab-8d8edae0282f">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.4.9 - Após a confirmação o Deploy iniciará, e ao final será apresentada uma pagina similar a pagina abaixo: <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="606" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/681248dd-bb7c-42f4-a5e1-e06405eb4a60">
<br>

## 4 - Acesse o `Language Studio`: <a href="https://language.cognitive.azure.com"> <img width="180" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/6fc4bdd0-80e6-4ab4-ae83-3c4e91bfc360">
</a> 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; https://language.cognitive.azure.com
  
## 5 - Selecione o Resource, aprovisionado no passo acima, p/ utilização no Language Studio

5.1 - Assim que você logar, Na página `Home - Welcome to Language Studio`, Abrirá um popup - `Select an Azure resource`, preencha:
<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
5.1.1 - `Azure Subscription`: selecione a sua Subscription; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
5.1.2 - `Resource Type`: escolha `Language`; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
5.1.3 - `Resource Name`: escolha o Nome da Instancia que criou na Azure; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
5.1.4 - Clique no botão `Done`; <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="668" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/333407ca-fd4f-49fd-beed-f009cb0816be">

---

# 🔬 Realizando o LAB - AI - Azure - Language Studio (Sentiment Analysis): 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (Após Preparação do Ambiente ter sido Finalizado com Sucesso. Vamos iniciar o LAB)

<br>

## 1 - Acesse o `Language Studio`: <a href="https://language.cognitive.azure.com"> <img width="180" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/6fc4bdd0-80e6-4ab4-ae83-3c4e91bfc360">
</a> 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; https://language.cognitive.azure.com
  
## 2 - Escolher - `Language - Sentiment Analysis`

2.1 - Na página `Home - Welcome to Language Studio`: <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
     ▶️  Clique na Guia `Classify Text` ; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
     ▶️  Clique no box `Analyze sentiment and mine opinions` ; <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="520" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/8c38b2e3-675f-46b5-98c1-7f149aefa68d">

## 3 - LAB - `Sentiment Analysis`

3.1 `Teste 1` - Texto 1 : `opiniao-celular-maria_p.txt` <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.1.1 - `Select Text Language` (idioma) - Selecionar: `Portuguese (Brazil)` se for utilizar arquivo texto deste repositório GitHub: <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.1.2 - `Azure Resource` - Selecionar o Resource que foi criado na Azure (Preparação do LAB) <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
3.1.3 - `Teste - 01` <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
    ▶️  `Escolhendo o Texto 1`: `opiniao-celular-maria_p.txt` - pasta: `inputs` - deste repositório GitHub: <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
          ▶️  Clicar no box `Browse a File` ; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
          ▶️ Escolher o Arquivo `opiniao-celular-maria_p.txt` que fez download do repositorio GitHub p/ sua maquina; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
          ▶️ Clique em `Abrir` ; <br>          

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="520" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/43913d1d-1646-4274-b225-aa8f16a75557">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="491" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/4dbe752a-1719-4a5e-8499-03d9b2783657">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
    ▶️  `Executando o Teste - 01`
    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
          ▶️  Clique no botão 'Run`;
   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="475" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/0918be34-a9c0-4653-9ea4-864c06b614dc">


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
    ▶️  `Resultado do Processamento - Texto 1` pelo `Language Studio`: <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img width="577" alt="image" src="https://github.com/mstrulenque/AI-Azure-Language-Studio_Analise-Sentimento_LAB/assets/63933792/3aa05320-5009-4149-a2b0-ee0f647ac387">


<br>
<br>

3.2 `Teste 2` - Texto 2 : `xxxxxxxxxxxxxxxx.txt` <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

EM ANDAMENTO..........

<br>
<br>

3.3 `Teste 3` - Texto 2 : `yyyyyyyyyyyyyyyyyy.txt` <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

EM ANDAMENTO..........



