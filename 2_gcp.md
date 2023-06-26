# 2_gcp.md
Este arquivo traz uma introdução ao Google Cloud Platform (GCP).
Este arquivo está organizado da seguinte maneira:

 **1.** O que é *cloud computing*?
 **2.** O que é o GCP?
 **3.** Referências

## 1. O que é *cloud computing*?
Atualmente, muito se fala sobre computação em nuvem:
-   _"Meus dados estão subindo para o Dropbox!"_  ou
-   _"Minha empresa está usando a nuvem como ferramenta de escritório para uso no dia a dia!"_  ou
-   _"Somos uma pequena empresa e utilizamos uma infraestrutura na nuvem"_

### Mas afinal, o que é essa “nuvem”?
Uma nuvem pode ser entendida como um  **conjunto de aplicações, armazenamento e computação**  que tem a  **internet**  como base e plataforma de funcionamento. E esse  _pool_  de serviços possui capacidade suficiente para dar suporte à maioria das necessidades de grande parte dos usuários.
[fonte](https://www.alura.com.br/artigos/cloud)
A computação em nuvem é a entrega de recursos de TI sob demanda por meio da Internet com definição de preço de pagamento conforme o uso. Em vez de comprar, ter e manter datacenters e servidores físicos, você pode acessar serviços de tecnologia, como capacidade computacional, armazenamento e bancos de dados, conforme a necessidade, usando um provedor de nuvem como, por exemplo, o GCP ou a Amazon Web Services (AWS).  
[fonte](https://aws.amazon.com/pt/what-is-cloud-computing/)

Hoje em dia, existem 3 modelos de serviços de _cloud computing_ utilizados para atender às necessidades das empresas. Vale a pena salientar que os riscos e benefícios que cada modelo de computação em nuvem pode trazer devem ser levados em consideração na hora de contratar o serviço.
### IaaS - Infrastructure as a Service

A  **Infraestrutura como Serviço**  oferece recursos de computação, armazenamento e rede. Ou seja, esse modelo disponibiliza um ambiente com uma infraestrutura virtualizada.

Como exemplos de serviços  _IaaS_:

-   [Amazon Web Services](https://www.alura.com.br/artigos/aws);
-   [Google Compute Engine](https://cloud.google.com/compute).

### PaaS - Plataform as a Service

Na  **Plataforma como Serviço**, temos um programa ou aplicativo entregue com o objetivo de facilitar a implementação de algum serviço; ou seja, é criado um ambiente para a  **programação**  e o desenvolvimento de alguma solução.

Alguns exemplos de  _PaaS_  são:

-   [Heroku](https://www.heroku.com/);
-   [Red Hat OpenShift](https://www.redhat.com/pt-br/technologies/cloud-computing/openshift).

### _SaaS - Software as a Service_

No  **Software como Serviço**, o software é executado em um servidor, de forma que o cliente não precisa tê-lo instalado em sua máquina.

Como exemplos de  _SaaS_, encontramos ferramentas como:

-   [Gupy](https://www.gupy.io/), plataforma online de recrutamento e seleção;
-   [Trello](https://trello.com/), plataforma utilizada para gerenciamento de tarefas e projetos.

Esse modelo ainda possui alguns desafios, como a  **integração**  com recursos internos da organização e a  **disponibilidade**, além da segurança da informação.

Atualmente, existem basicamente três tipos de _Cloud_ que podemos contratar. São eles:

### Cloud Pública
Este sem dúvida é o tipo de serviço de  _cloud_  que  **mais vemos em utilização pelas empresas**. Nele, os serviços são mantidos por um determinado provedor de serviços.

Esses provedores possuem uma série de data centers com uma gama de  **servidores interconectados**  que compartilham recursos e serviços pelos utilizadores da nuvem.

### Cloud Privada
Este tipo de serviço oferece uma  **infraestrutura alocada**  para uma única organização. Uma nuvem privada pode estar hospedada no data center mantido pela própria empresa.

### Cloud Híbrida
Uma nuvem híbrida é a  **utilização em conjunto**  da  **nuvem pública e da privada**. Um cenário muito comum seria o de usar uma nuvem pública para manter a execução de algum sistema e manter a fonte de dados da aplicação na nuvem privada.

Quando estamos falando do ambiente de nuvem, podemos nos deparar com o termo  _On Premise_, que é um tipo de organização da nossa estrutura em um ambiente só. Um ambiente  _On Premise_  É quando temos toda a infraestrutura de servidores e máquinas em um espaço físico na empresa, a famosa “sala de servidores” ou CPD. Em contrapartida a esse ambiente, temos o ambiente da nuvem.

## 2. O que é o GCP?
O GCP é um fornecedor de nuvem pública — como os concorrentes [Amazon Web Services (AWS)](https://www.pluralsight.com/resources/blog/cloud/what-is-amazon-web-services-aws) e [Microsoft Azure](https://www.pluralsight.com/resources/blog/cloud/what-is-microsoft-azure) . Com o GCP e outros fornecedores de nuvem, os clientes podem acessar recursos de computador armazenados nos datacenters do Google em todo o mundo gratuitamente ou mediante pagamento conforme o uso.

O GCP oferece um conjunto de serviços de computação para fazer tudo, desde o gerenciamento de custos do GCP até o gerenciamento de dados, passando por ferramentas de IA e aprendizado de máquina.
#### Google Cloud x Google Cloud Platform

O Google Cloud inclui uma combinação de serviços disponíveis na Internet que podem ajudar as organizações a se tornarem digitais. O Google Cloud Platform (que fornece infraestrutura de nuvem pública para hospedar aplicativos baseados na Web e é o foco desta postagem no blog) faz parte _do_ Google Cloud.

Alguns outros serviços que fazem parte do Google Cloud incluem:

-   Google Workspace, anteriormente conhecido como G Suite e Google Apps. Este produto fornece gerenciamento de identidade para organizações, Gmail e ferramentas de colaboração.

-   Versões empresariais do Android e Chrome OS. Esses sistemas operacionais de telefone e laptop são maneiras de os usuários se conectarem a aplicativos baseados na web.

-   Interfaces de programação de aplicativos (APIs) para aprendizado de máquina e serviços de mapeamento corporativo. Eles fornecem comunicação de software para software.

Embora a infraestrutura de nuvem GCP do Google seja a espinha dorsal de aplicativos como o Google Workplace, _não_ estamos falando desses aplicativos quando falamos do GCP. Para esta postagem, estamos nos concentrando no Google Cloud Platform.

### A história do Google Cloud Platform

Voltando um pouco, vamos começar com a história do GCP.

O GCP entrou online pela primeira vez em 2008 com o lançamento de um produto chamado App Engine. Em abril de 2008, o Google [anunciou](https://googleappengine.blogspot.com/2008/04/introducing-google-app-engine-our-new.html) uma versão prévia do App Engine, uma ferramenta de desenvolvedor que permitia aos clientes executar seus aplicativos da Web na infraestrutura do Google. (Para uma perspectiva, isso aconteceu dois anos depois que a Amazon lançou seu serviço de computação em nuvem, começando com o lançamento do armazenamento em nuvem S3 e EC2.)

De acordo com o Google, o objetivo do App Engine era “facilitar o início de um novo aplicativo da Web e, em seguida, facilitar o dimensionamento quando esse aplicativo atingir o ponto em que recebe tráfego significativo e tem milhões de usuários”.

Para obter o feedback necessário para fazer melhorias nesta versão de visualização, o App Engine foi disponibilizado para 10.000 desenvolvedores. Esses desenvolvedores pioneiros poderiam executar aplicativos com 500 MB de armazenamento, 200 milhões de megaciclos de CPU por dia e 10 GB de largura de banda por dia.

No final de 2011, o Google tirou o App Engine do modo de visualização e o tornou um produto oficial do Google com suporte completo. Na década seguinte, o Google construiu e adquiriu mais serviços e produtos para aprimorar a experiência do usuário em sua plataforma de nuvem.

Hoje, o Google Cloud Platform é um dos principais fornecedores de nuvem pública do mundo. Os clientes do Google Cloud incluem Nintendo, eBay, UPS, The Home Depot, Etsy, PayPal, 20th Century Fox e Twitter.
[fonte](https://www.pluralsight.com/resources/blog/cloud/what-is-google-cloud-platform-gcp)

Vários componentes e serviços são um recurso importante do Google Cloud Platform; vamos mergulhar em cada um individualmente e aprender mais sobre o que eles oferecem.

### 1. Compute

O serviço de computação permite computar e hospedar a nuvem. Os vários serviços abrangidos por este são os seguintes:
-   App Engine
-   Compute Engine
-   Kubernetes Engine
-   Cloud Functions
-   Cloud Run

### 2. Armazenamento e Banco de Dados
O serviço de armazenamento e banco de dados permite que o aplicativo armazene arquivos de mídia, backups ou outros objetos semelhantes a arquivos. Os serviços incluem:
-   Cloud Storage
-   Cloud SQL
-   Cloud Bigtable
-   Cloud Spanner
-   Cloud Datastore

### 3. Rede
O serviço de rede nos permite balancear a carga do tráfego entre os recursos, criar registros DNS e muito mais. Alguns dos serviços incluem:
-   VPC
-   Cloud Load Balancing
-   Cloud Armor
-   Cloud CDN
-   Cloud Interconnect
-   Cloud DNS
-   Network Service Tiers

### 4. Big Data
O serviço de big data nos permite processar e consultar big data na nuvem. Alguns dos serviços incluídos são os seguintes::
-   BigQuery
-   Cloud Dataproc
-   Cloud Datalab
-   Cloud Data Studio

### 5. Ferramentas do desenvolvedor
O serviço de ferramentas do desenvolvedor inclui ferramentas que permitem o desenvolvimento de software e aplicativos.
-   Artifact Registry 
-   Cloud SDK
-   Cloud Code
-   CloudBuild
-   Cloud Scheduler
-   Cloud Tasks

[fonte](https://www.simplilearn.com/google-cloud-platform-article)

## 3. Referências
https://aws.amazon.com/pt/what-is-cloud-computing/ 
https://www.alura.com.br/artigos/cloud
https://www.redhat.com/pt-br/topics/cloud
https://www.pluralsight.com/resources/blog/cloud/what-is-google-cloud-platform-gcp