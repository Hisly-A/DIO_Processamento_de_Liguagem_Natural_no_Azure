# DIO - Processamento de Liguagem Natural no Azure
Análise de Sentimentos com Language Studio no Azure AI

## 🔎 O que é o Azure AI Speech?	

>O serviço Azure AI Speech transcreve a fala em texto e o texto em fala audível. Você pode usar o AI Speech para criar um aplicativo que possa transcrever notas de reuniões ou gerar texto a partir da gravação de entrevistas.

<sub>Fonte: <https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html></sub>


## Criação do recurso de fala do Azure AI

Em outra guia do navegador, abra o [`Azure AI Speech Studio`](https://speech.microsoft.com/portal), entrando com sua conta da Microsoft.

Clique em **Settings** e depois `+ Create new resource`. 

<div align="center">
    <img width="700" title="LN01" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN01.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN02" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN02.PNG"/>
</div>
<br>

Configure-o da seguinte forma:
- *New feature name*: Informe um nome exclusivo.
- *Signature*: Sua assinatura do Azure.
- *Region*: Selecione uma região suportada.
- *Pricing Type*: FO gratuito (se disponível, caso contrário, selecione Padrão S0).
- *Resource group*: Selecione ou crie um grupo de recursos com um nome exclusivo.

<div align="center">
    <img width="700" title="LN03" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN03.PNG"/>
</div>
<br>

Clique em `Create a resource`. Aguarde até que o recurso seja criado e clique em `Use the feature`.

<div align="center">
    <img width="700" title="LN04" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN04.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN05" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN05.PNG"/>
</div>
<br>

## Explore a fala em texto no Speech Studio
Na página **Get started with Speech**, em **Speech to text**, localize **Real-time speech to text**. Clique em `Try Real-time Speech-to-text`.

<div align="center">
    <img width="700" title="LN06" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN06.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN07" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN07.PNG"/>
</div>
<br>

Clique em `Browse files`, navegue até a pasta onde o arquivo [`Poema Acontecimento Cecília Meireles.ogg`](https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/inputs/Poema%20Acontecimento%20Cec%C3%ADlia%20Meireles.ogg) foi salvo e abra.

<div align="center">
    <img width="700" title="LN08" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN08.PNG"/>
</div>
<br>

O serviço Speech transcreve e exibe o texto em tempo real.

<div align="center">
    <img width="700" title="LN10" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN10.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN11" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN11.PNG"/>
</div>
<br>

## 🔎 O que é o Azure AI Language Studio?

>O Azure AI Language Service inclui análise de texto e recursos de PNL. Isso inclui a identificação de frases-chave no texto e a classificação do texto com base no sentimento. O Processamento de Linguagem Natural (PNL) é um ramo da IA ​​que lida com a linguagem escrita e falada. Você pode usar a PNL para construir soluções que extraiam significado semântico de texto ou fala, ou que formulem respostas significativas em linguagem natural.

<sub>Fonte: <https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html></sub>

## Criação de um recurso de idioma

Abra o portal do [`Azure`](https://portal.azure.com), entrando com a conta da Microsoft associada à assinatura do Azure.

Clique no botão `＋Create a resource` e pesquise por **Language service**.

<div align="center">
    <img width="700" title="LN14" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN14.PNG"/>
</div>
<br>

Irá abrir uma página para selecionar recursos adicionais, mantenha a seleção padrão e clique em ```Continue to create your resource```.

<div align="center">
    <img width="700" title="LN15" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN15.PNG"/>
</div>
<br>

Na página **Create Language**, configure da seguinte forma:
- *Subscription*: Sua assinatura do Azure.
- *Resource group*: Selecione ou crie um grupo de recursos com um nome exclusivo.
- *Region*: Leste dos EUA.
- *Name*: Insira um nome exclusivo.
- *Pricing tier*: F0 grátis ou S se F0 grátis não estiver disponível.
- *Marcar o campo*: By checking this box I acknowledge that I have read and understood all the terms below.

<div align="center">
    <img width="700" title="LN16" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN16.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN17" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN17.PNG"/>
</div>
<br>

Clique em `Review + create` e depois `Create` e aguarde a conclusão da implantação.

<div align="center">
    <img width="700" title="LN18" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN18.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN19" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN19.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN20" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN20.PNG"/>
</div>
<br>

## Configure seu recurso no Azure AI Language Studio
Abra o [`Language Studio`](https://language.cognitive.azure.com) e em **Select an Azure resource**, faça as seguintes configurações:
- *Azure directory*: Diretório padrão, o diretório que você está usando;
- *Azure subscription*: Selecione a assinatura que você está usando;
- *Resource type*: Idioma;
- *Resource name*: Selecione o recurso de serviço de idioma criado.

Clique em `Done`.

<div align="center">
    <img width="700" title="LN21" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN21.PNG"/>
</div>
<br>

## Analise de avaliações no Language Studio

Na página inicial do [`Language Studio`](https://language.cognitive.azure.com) clique em `Classify text` e, em seguida, selecione o bloco **Analyze sentiment and mine opinions**.

<div align="center">
    <img width="700" title="LN22" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN22.PNG"/>
</div>
<br>

Em **Select text language**, selecione Português e em **Select your Azure resource**, selecione seu recurso.

<div align="center">
    <img width="700" title="LN23" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN23.PNG"/>
</div>
<br>

Em **Enter your own text**, use o seguinte texto de exemplo: [`Avaliação de Hotel.txt`](https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/inputs/Avalia%C3%A7%C3%A3o%20de%20Hotel.txt)

<div align="center">
    <img width="700" title="LN28" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN28.PNG"/>
</div>
<br>

Marque a caixa para confirmar que a demonstração incorrerá em uso e poderá incorrer em custos e clique em `Run`.

<div align="center">
    <img width="700" title="LN24" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN24.PNG"/>
</div>
<br>

Revise a saída. Observe que o documento é analisado quanto ao sentimento, assim como cada frase. 

<div align="center">
    <img width="700" title="LN25" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN25.PNG"/>
</div>
<br>

Selecione a Frase 1 para mostrar a análise de sentimento dessa frase, que foi um sentimento positivo:

<div align="center">
    <img width="700" title="LN26" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN26.PNG"/>
</div>
<br>

Já as Frases 2 e 6 tiveram uma análise de sentimento mais negativa:

<div align="center">
    <img width="700" title="LN27" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN27.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN30" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN30.PNG"/>
</div>
<br>

Na Frase 7 a análise de sentimento foi neutra:

<div align="center">
    <img width="700" title="LN29" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN29.PNG"/>
</div>
<br>

Obeserve que a análise também traz uma visão geral do texto:

<div align="center">
    <img width="700" title="LN31" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN31.PNG"/>
</div>
<br>

Clique em `Clear text box` e copie e cole a seguinte revisão:

>Very noisy and rooms are tiny The Lombard Hotel, San Francisco, USA 9/5/2018 Hotel is located on Lombard street which is a very busy SIX lane street directly off the Golden Gate Bridge. Traffic from early morning until late at night especially on weekends. Noise would not be so bad if rooms were better insulated but they are not. Had to put cotton balls in my ears to be able to sleep–was too tired to enjoy the city the next day. Rooms are TINY. I picked the room because it had two queen size beds–but the room barely had space to fit them. With family of four in the room it was tight. With all that said, rooms are clean and they’ve made an effort to update them. The hotel is in Marina district with lots of good places to eat, within walking distance to Presidio. May be good hotel for young stay-up-late adults on a budget.

Em **Select text language**, selecione Inglês:

<div align="center">
    <img width="700" title="LN32" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN32.PNG"/>
</div>
<br>

Clique em `Run` e analise o sentimento juntamente com o nível de confiança. Dê uma olhada no texto e compare-o com a análise de sentimento que o serviço retornou.

<div align="center">
    <img width="700" title="LN33" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN33.PNG"/>
</div>
<br>

Obeserve o sentimento com maior percentual em cada uma das seguintes frases:

<div align="center">
    <img width="700" title="LN34" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN34.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN35" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN35.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN36" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN36.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN37" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN37.PNG"/>
</div>
<br>

## Excluir os recursos utilizados nos testes

Abra o portal do [`Azure`](https://portal.azure.com) e selecione o grupo de recursos que contém o recurso que você criou.
Selecione o recurso e clique em `Delete resource group` e depois `Delete` para confirmar.

<div align="center">
    <img width="700" title="LN12" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN12.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN39" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN39.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN40" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN40.PNG"/>
</div>
<br>

O processo de exclusão será iniciado:

<div align="center">
    <img width="700" title="LN41" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN41.PNG"/>
</div>
<br>
<div align="center">
    <img width="700" title="LN42" src="https://github.com/Hisly-A/DIO_Processamento_de_Liguagem_Natural_no_Azure/blob/main/output/LN42.PNG"/>
</div>
<br>

## Links utilizados

- https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html

- https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html

- https://language.cognitive.azure.com

