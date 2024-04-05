# DIO - Processamento de Liguagem Natural no Azure
Análise de Sentimentos com Language Studio no Azure AI

## 🔎 O que é o Azure AI Speech?	

>O serviço Azure AI Speech transcreve a fala em texto e o texto em fala audível. Você pode usar o AI Speech para criar um aplicativo que possa transcrever notas de reuniões ou gerar texto a partir da gravação de entrevistas.

<sub>Fonte: <https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html></sub>


## Criação do recurso de fala do Azure AI

Em outra guia do navegador, abra o Azure AI Speech Studio (https://speech.microsoft.com/portal), entrando com sua conta da Microsoft.

Clique em **Settings** e depois **+ Create a resource**. Configure-o da seguinte forma:
- *Name of new resource*: Informe um nome exclusivo.
- *Subscription*: Sua assinatura do Azure.
- *Region*: Selecione uma região suportada.
- *Pricing tier*: FO gratuito (se disponível, caso contrário, selecione Padrão S0).
- *Resource group*: Selecione ou crie um grupo de recursos com um nome exclusivo.

Clique em ```Create resource```. Aguarde até que o recurso seja criado e clique em **Use resource**.

## Explore a fala em texto no Speech Studio
Na página **Get started with Speech**, em **Speech to text**, localize **Real-time speech to text**. Clique em **Try out Real-time speech to text**.

Clique em ```Browse files```, navegue até a pasta onde você salvou o arquivo **WhatAICanDo.m4a** e abra.

O serviço Speech transcreve e exibe o texto em tempo real.

## 🔎 O que é o Azure AI Language Studio?

>O Azure AI Language Service inclui análise de texto e recursos de PNL. Isso inclui a identificação de frases-chave no texto e a classificação do texto com base no sentimento. O Processamento de Linguagem Natural (PNL) é um ramo da IA ​​que lida com a linguagem escrita e falada. Você pode usar a PNL para construir soluções que extraiam significado semântico de texto ou fala, ou que formulem respostas significativas em linguagem natural.

<sub>Fonte: <https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html></sub>

## Criação de um recurso de idioma

Abra o portal do Azure em https://portal.azure.com, entrando com a conta da Microsoft associada à sua assinatura do Azure.

Clique no botão ```＋Create a resource``` e pesquise por **Language service**. Crie um plano **Language service**. Irá abrir uma página para selecionar recursos adicionais, mantenha a seleção padrão e clique em ```Continue to create your resource```.

Na página **Create Language**, configure da seguinte forma:
- *Subscription*: Sua assinatura do Azure.
- *Resource group*: Selecione ou crie um grupo de recursos com um nome exclusivo.
- *Region*: Leste dos EUA.
- *Name*: Insira um nome exclusivo.
- *Pricing tier*: F0 grátis ou S se F0 grátis não estiver disponível.
- *Marcar o campo*: By checking this box I acknowledge that I have read and understood all the terms below.

Clique em ```Review + create``` e depois ```Create``` e aguarde a conclusão da implantação.

## Configure seu recurso no Azure AI Language Studio
Abra o Language Studio em https://language.cognitive.azure.com.

Em **Select an Azure resource**, faça as seguintes configurações:
- *Azure directory*: Diretório padrão, o diretório que você está usando;
- *Azure subscription*: Selecione a assinatura que você está usando;
- *Resource type*: Idioma;
- *Resource name*: Selecione o recurso de serviço de idioma que você acabou de criar.

Clique em ```Done```.

## Analise de avaliações no Language Studio

Na página inicial do **Language Studio** clique em ```Classify text``` e, em seguida, selecione o bloco **Analyze sentiment and mine opinions**.

Em **Select text language**, selecione Inglês.

Em **Select your Azure resource**, selecione seu recurso.

Em **Enter your own text**, carregue um arquivo ou use o seguinte texto de exemplo:

```
 Tired hotel with poor service
 The Royal Hotel, London, United Kingdom
 5/6/2018
 This is an old hotel (has been around since 1950's) and the room furnishings are average - becoming a bit old now and require changing. The internet didn't work and had to come to one of their office rooms to check in for my flight home. The website says it's close to the British Museum, but it's too far to walk.
```

Marque a caixa para confirmar que a demonstração incorrerá em uso e poderá incorrer em custos e clique em ```Run```.

Revise a saída. Observe que o documento é analisado quanto ao sentimento, assim como cada frase. Selecione Frase 1 para mostrar a análise de sentimento dessa frase.

Observe que há um sentimento geral seguido por pontuações próximas a três categorias: pontuação positiva , pontuação neutra e pontuação negativa. Em cada uma das categorias é atribuída uma pontuação entre 0 e 1. Essas pontuações de confiança indicam a probabilidade do texto fornecido ser um sentimento específico.

Selecione a frase 1 novamente para fechar.

Clique em ```Clear text box``` e copie e cole a seguinte revisão:

```
 Good Hotel and staff
 The Royal Hotel, London, UK
 3/2/2018
 Clean rooms, good service, great location near Buckingham Palace and Westminster Abbey, and so on. We thoroughly enjoyed our stay. The courtyard is very peaceful and we went to a restaurant which is part of the same group and is Indian ( West coast so plenty of fish) with a Michelin Star. We had the taster menu which was fabulous. The rooms were very well appointed with a kitchen, lounge, bedroom and enormous bathroom. Thoroughly recommended.
```

Clique em ```Run```. Revise o resultado, o sentimento e o nível de confiança.

Clique em ```Clear text box``` novamente e copie e cole a seguinte revisão:

```
Very noisy and rooms are tiny The Lombard Hotel, San Francisco, USA 9/5/2018 Hotel is located on Lombard street which is a very busy SIX lane street directly off the Golden Gate Bridge. Traffic from early morning until late at night especially on weekends. Noise would not be so bad if rooms were better insulated but they are not. Had to put cotton balls in my ears to be able to sleep–was too tired to enjoy the city the next day. Rooms are TINY. I picked the room because it had two queen size beds–but the room barely had space to fit them. With family of four in the room it was tight. With all that said, rooms are clean and they’ve made an effort to update them. The hotel is in Marina district with lots of good places to eat, within walking distance to Presidio. May be good hotel for young stay-up-late adults on a budget
```

Clique em ```Run``` e analise o sentimento juntamente com o nível de confiança. Dê uma olhada no texto e compare-o com a análise de sentimento que o serviço retornou.


## Excluir os recursos utilizados nos testes

Abra o portal do Azure em https://portal.azure.com e selecione o grupo de recursos que contém o recurso que você criou.
Selecione o recurso e clique em ```Delete``` e depois ```Yes``` para confirmar.




## Links utilizados

- https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html

- https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html

- https://language.cognitive.azure.com

