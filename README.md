# BuscasCognitivas-Azure

Este projeto é uma aplicação prática do módulo Service Cloud com IA da trilha Decola Tech 2025 da DIO. O objetivo foi utilizar o o Azure AI Services + Azure Storage para criar um sistema de análise automatizada de reviews (como avaliações de produtos, comentários, etc.)

Com os serviços da Azure, é possível:
✅ Armazenar reviews através de textos, arquivos de reviews (CSV, JSON, etc.) no Azure Blob Storage.
✅ Processar os dados usando Azure AI Services.
✅ Automatizar análises (sentimento, palavras-chave, tradução, categorização).

Passo a passo na prática:
Para utilizar o serviço e demonstrar abaixo, realizei o download do pacote coffee-reviews disponível em https://aka.ms/mslearn-coffee-reviews para utilizar como exemplo prático e seguindo o passo a passo da vídeo aula ministrada por Valéria Baptista.

Alguns passos são bem técnicos e estão relacionados com a necessidade do negócio e também a assinatura de planos junto com a Microsoft. Incluí na pasta /src todo o passo a passo que segui para realizar, mas destaco abaixo quais são os passos que considerei bastante interessante na utilização do serviço.

1. Criação do serviço AI Search: será a ferramenta responsável por processar os dados
![alt text](<src/Passo 1.png>)

2. Criar a conta de armazenamento: É através dela que os arquivos serão armazenados para a integração com a IA criada na Azure
![alt text](<src/Passo 4.png>)

3. Carregar os arquivos que serão utilizados para a análise (aqui foram carregados os arquivos do coffee-review)
![alt text](<src/Passo 8.png>)

6. Após o upload dos arquivo que serão utilizados para esta análise, ao explorar a pesquisa, é possível 
    - A AI Azure processa os dados com modelos pré-treinados (análise de sentimentos, extração de palavras-chave, tradução, etc.).
    - Na pesquisa que fiz como exemplo, utilizei o filtro de conteúdo 'don't like' para extrair as situações que o review mencionava esta expressão;
    - O AI AZure é um modelo pré-treinado pela Microsoft e o serviço devolve metadados como: sentimentos (positivo/neutro/negativo), entidades (nomes de produtos, marcas) e tópicos principais (ex.: "entrega", "qualidade").
    
![alt text](<src/Passo 13.png>)