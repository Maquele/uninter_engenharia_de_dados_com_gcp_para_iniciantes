# 1_engenharia_de_dados.md
Este arquivo traz uma introdução ao mundo da engenharia de dados.
Este arquivo está organizado da seguinte maneira:

 **1.** O que faz um engenheiro de dados?
 **2.** O que é engenharia de dados?
 **3.** O que é *big data*?
 **4.** Outros conceitos básicos para iniciar a jornada na engenharia de dados
 **5.** Referências

## 1. O que faz um engenheiro de dados?
O  engenheiro de dados é o responsável pela criação do pipeline que transforma os dados brutos que estão nos mais variados formatos, desde bancos de dados transacionais até arquivos de texto, em um formato que permita ao Cientista de Dados começar seu trabalho.

Cabe também ao Engenheiro de Dados manter este pipeline em execução para que os dados possam ser coletados no momento certo, com o nível de segurança exigido pela empresa. O trabalho do Engenheiro de dados é tão importante quanto o trabalho do Cientista de Dados e vem ganhando cada vez mais visibilidade dentro das empresas.

Um Engenheiro de Dados precisa ser bom em:
 - Arquitetar sistemas distribuídos 
 - Criar pipelines confiáveis 
 - Combinar fontes de dados
 - Criar a arquitetura de soluções
 - Colaborar com a equipe de Data Science e construir as soluções certas para essas equipes

Observe que não mencionamos nenhuma ferramenta. Embora ferramentas como Hadoop e Spark e linguagens como Scala e Python sejam muito importantes para o Engenheiro de Dados, é importante também entender bem os conceitos e saber como construir sistemas do mundo real, além de habilidade em **Cloud Computing**.
[fonte](https://blog.dsacademy.com.br/o-que-faz-um-engenheiro-de-dados/)

## 2. O que é engenharia de dados?
A história da Engenharia de Dados começou com artigos da  **Google**. O primeiro, publicado em 2003, abordava o  _Google File System_, um sistema de arquivos distribuídos. Logo em seguida, em 2004, foi publicado outro artigo sobre  _MapReduce_, uma técnica de processamento de grandes volumes de dados.

Esses artigos inspiraram engenheiros do  _Yahoo_  a criarem, em 2006, o  **Hadoop**, que mostrou-se uma ferramenta muito útil para trabalhar com grandes volumes de dados. A partir disso, surgiu a era da  **Engenharia de Dados com Big Data**.

O desafio de  **transformar**  essa grande quantidade e variedade de  **dados**  em  **informações úteis e de qualidade**  é essencial para o time de dados. Mas, para isso, precisamos criar um  **ambiente**  propício para gerar tais informações.

A Engenharia de Dados é a área responsável por  **desenvolver**,  **implementar**  e  **manter**  esse ambiente, que chamamos de  **_Pipeline_**. É nele que vamos criar todas as etapas relacionadas ao fluxo de dados, desde a extração, passando pelo armazenamento, até a distribuição dos dados para consumo.
[fonte](https://www.alura.com.br/artigos/engenharia-dados)

O campo da  ciência de dados  é incrivelmente amplo, abrangendo tudo, desde a limpeza de dados até a implantação de modelos preditivos. No entanto, é raro um único Cientista de Dados trabalhar em todos as áreas da Ciência de Dados. Os Cientistas de Dados geralmente se concentram em algumas áreas, e são complementados por uma equipe de outros Cientistas e Analistas.

A Engenharia de Dados também é um campo amplo. Vejamos primeiro o que é a Engenharia de Dados e depois caminhamos através de descrições mais específicas que ilustram as funções nesta área.

Um Engenheiro de Dados transforma dados em um formato útil para análise. Imagine que você é um Engenheiro de Dados que irá trabalhar em um concorrente do  Uber. Seus usuários têm um aplicativo através do qual eles acessam seu serviço. Eles pedem uma corrida para um destino através do aplicativo, que é encaminhado para um motorista, que os busca e os leva para onde foi solicitado. Após a corrida, eles são cobrados e têm a opção de avaliar como o motorista dirigiu.

Para manter um serviço como este, você precisa:

-   Um aplicativo para dispositivos móveis, para usuários.
-   Um aplicativo para dispositivos móveis, para motoristas.
-   Um servidor que pode passar pedidos de usuários para motoristas e lidar com outros detalhes, como atualizar informações de pagamento.

Como você pode imaginar, esse tipo de sistema vai gerar enormes quantidades de dados. Você terá diferentes tipos de dados para serem armazenados:

-   O banco de dados do seu aplicativo principal. Ele deve conter informações sobre o usuário e o motorista.
-   Logs de análise de servidor:
    -   Registros de acesso ao servidor. Estes contêm uma linha por solicitação feita ao servidor a partir do aplicativo.
    -   Logs de erro do servidor. Estes contêm todos os erros do lado do servidor os quais foram gerados pelo seu aplicativo.
-   Registros de análise de aplicativos:
    -   Registros de eventos da aplicação. Estes contêm informações sobre as ações que os usuários e os motoristas receberam no aplicativo. Por exemplo, você estava logado quando clicou em um botão ou atualizou suas informações de pagamento.
    -   Logs de erro da aplicação. Estes contêm informações sobre erros no aplicativo.
-   Registros de corridas. Estes contêm informações sobre cada corrida para os usuários / motoristas e contêm informações sobre o status da corrida.
-   Registros de Serviços ao Cliente. Estes contêm informações sobre interações com clientes por agentes de atendimento ao cliente. Podem incluir transcrições de voz e registros de e-mail.

Digamos que um Cientista de Dados quer analisar o histórico de ação de um usuário com seu serviço e ver quais ações se correlacionam com os usuários que gastam mais. Para isso, será necessário combinar informações dos logs de acesso do servidor e dos logs de eventos do aplicativo. Será necessário:

-   Reunir regularmente logs de análise de aplicativos de dispositivos do usuário.
-   Combinar os logs da análise do aplicativo com todas as entradas de log do servidor que fazem referência ao usuário.
-   Criar uma API que retorna o histórico de eventos de qualquer usuário.

Para resolver isso, você precisará criar um pipeline que possa registrar o uso dos aplicativos móveis e logs do servidor em tempo real, analisá-los e anexá-los a um usuário específico. Em seguida, você precisará armazenar os registros analisados ​​em um banco de dados, para que possam ser facilmente consultados pela API. Você precisará configurar vários servidores em modo de balanceamento de carga para processar os logs recebidos.

A maioria dos problemas que você vai encontrar serão relativos à confiabilidade dos sistemas distribuídos. Por exemplo, se você tiver milhões de dispositivos para reunir logs e demanda variável (de manhã, você recebe uma tonelada de logs, e quase nenhum à meia-noite), você precisará de um sistema que possa escalar automaticamente a contagem de servidores para cima e para baixo.

Neste momento entra em cena a necessidade de ter um ambiente em nuvem, robusto e seguro, que possa processar esse grande volume de dados. Uma estrutura em nuvem, usando um provedor como o **GCP**, pode ser a melhor alternativa custo/benefício. Os servidores são registrados com um balanceador de carga, e o balanceador de carga envia tráfego para eles com base em como eles estão ocupados. Isso significa que os servidores podem ser adicionados ou removidos conforme necessário.
[fonte](https://blog.dsacademy.com.br/o-que-faz-um-engenheiro-de-dados/)

## 3 O que é *big data*?
O termo  _Big Data_, em português “grande volume de dados”, começou a aparecer quando os métodos tradicionais para  **armazenamento**  começaram a não ser tão eficientes nesse novo ambiente que exigia muito mais do que uma ferramenta de armazenamento conseguia suportar.

De forma geral, o Big Data pode ser definido com  **3 V’s principais**:

1.  Volume;
2.  Variedade;
3.  Velocidade.

### 1) Volume
**Grande quantidade de dados**  para ser  **armazenada**  e  **processada**, com escalas que vão desde terabytes até mesmo zettabytes.

### 2) Variedade
A variedade de dados é um outro pilar do Big Data, pois, dentro do grande volume de dados, temos  **diferentes tipos**  — desde  **dados estruturados**,  **semi-estruturados**  a  **não estruturados**.

### 3) Velocidade
Essa grande quantidade de dados costuma ser  **gerada**  num  **curto espaço de tempo**. Um bom exemplo são as redes sociais, onde temos milhares de mensagens e registros em bancos para serem atualizados.
[fonte](https://www.alura.com.br/artigos/engenharia-dados)

## 4. Outros conceitos básicos para iniciar a jornada na engenharia de dados
Existem quatro palavras que acompanharão a carreira de um Engenheiro de Dados:

·  **Coleta =** na coleta de dados, é necessário que o Engenheiro de Dados saiba escolher ferramentas de forma a acompanhar a entrada das informações. As falhas devem ser imediatamente detectadas (como um equipamento que sofreu curto circuito) e, além disso, as ferramentas devem ser provisionadas de forma a ler todos esses dados e, caso necessário, distribui-los para seus respectivos caminhos;

·  **Transformação =** o dado nem sempre chega na forma que é esperado, e será trabalho do Engenheiro de Dados também relaciona-lo de forma que agregue valor a ele, e que ele seja de fácil entendimento e relação, além de detectar inconsistência e problemas. Os valos inconsistentes devem ser retirados, de forma que não poluam a forma final dos dados. As ferramentas escolhidas devem proporcionar agilidade em carregar e checar estes dados;

·  **Armazenamento =** após o Engenheiro de Dados montar boas relações entre os dados, é preciso armazena-los, de forma centralizada ou distribuída. É necessário que o Eng. de Dados saiba dimensionar os serviços que vão armazenar os dados, de forma correta e eficiente, pensando sempre nos casos de uso dos clientes;

·  **Distribuição =** o Engenheiro de Dados deve disponibilizar os dados de forma simples, segura e eficiente. A distribuição de dados depende da quantidade de profissionais que trabalharão na solução, o que gera  **perfis** dentro da Engenharia de Dados.

Os  **perfis de Engenheiro de Dados (papeis)**  são divididos em:

·  **Analista:** realiza as análises dos dados que, quando bem organizados, fornecem informações importantes sobre o negócio. O valor entregue será o provisionamento em larga escala e um modelo ligado diretamente ao aprendizado de máquina;

·  **Construtor:** é responsável por pensar nas situações em que o negócio se expande e tem seu sistema aplicado a outros locais, provendo um ambiente que contemple as necessidades atuais com a comunicação rápida, munida de backup e alta disponibilidade;

·  **Desenvolvedor:** buscará a solução de questões particulares e/ou otimizadas para demandas especificas, seja uma nova ou uma adaptação da antiga. Os desenvolvedores também vão interagir com os serviços em Nuvem, interligando os dois sistemas, necessitando que o profissional dessa área tenha conhecimentos de  **Arquitetura** e  **Desenvolvimento de Software**;

·  **Generalista:** os conhecimentos deste profissional devem abranger os sistemas locais, o caminho das informações no servidor, como funcionam os bancos de dados, bem como as ferramentas necessárias para a manutenção e construção de softwares. É importante também que ele tenha experiência com ambientes  **Linux**  e  **linguagens de programação**  que lidam com dados.

Além disso, alguns outros  **termos para anotar**  são:

**Data Storages** são bancos de dados usualmente não-relacionais, que são utilizados para armazenar arquivos, e-mails, log, etc.; além de informações utilizando um mapeamento chave-valor. Como cada um possui uma chave única, o arquivo poderá ser subscrita toda vez que algo for recarregada com a mesma chave. Além disso, não há relacionamento entre os itens guardados, como no uso do comando  **JOIN**, que faz a agregação. Com relação ao  **transporte de dados,**  podemos dividi-los em:

·  **Streaming =** corresponde ao processamento em tempo real, ou seja, são processados ou consumidos a medida que são gerados;

·  **Transmissão por Lotes =** lida com maiores volumes de dados. Por exemplo, seria como pães em uma padaria que se originam em lotes de massas assadas, os quais são preparadas após o termino do processo anterior.
[fonte](https://guilherme-manzano.medium.com/introdu%C3%A7%C3%A3o-%C3%A0-engenharia-de-dados-22c07129992a)

## 5. Referências
https://www.alura.com.br/artigos/engenharia-dados
https://guilherme-manzano.medium.com/introdu%C3%A7%C3%A3o-%C3%A0-engenharia-de-dados-22c07129992a
https://blog.dsacademy.com.br/o-que-faz-um-engenheiro-de-dados/