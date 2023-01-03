<div align="center">
  <img src="https://user-images.githubusercontent.com/61476935/210269491-dbdd0597-4227-4969-bd84-b72ba65cdf4a.png">
</div>
<br>

A Clean Architecture, ou Arquitetura Limpa, é um padrão de arquitetura de sistemas criado por Rober Cecil Martin, engenheiro de software americano, popularmente conhecido como [Uncle Bob](https://www.google.com/search?gs_ssp=eJzj4tbP1TcwNKoyyk5PMmD04izNS85JVUjKTwIAVZAHQg&q=uncle+bob&rlz=1C1ASUM_enBR992BR992&oq=Uncle+Bob&aqs=chrome.1.69i57j46i512j0i512l8.3321j0j7&sourceid=chrome&ie=UTF-8). Sendo inicialmente divulgada através do também popular "Arquitetura Limpa - O Guia do Artesão para Estrutura e Design de Software", é bastante difundida no mercado programação e amplamente adotada quando se trata de arquitetura de sistemas.

Antes de adentrarmos no que caracteriza a Clean Architecture, é importante entender do que se trata o tópico <i>Arquitetura</i> em desenvolvimento de sistemas, porque ele é necessário, e quais são as formas de atender a essa necessidade.

# Arquitetura de Software

Uma definição básica de arquitetura é que ela consiste no conjunto de princípios, normas, técnicas e materiais usadados para criar um espaço arquitetônico. Isso quando tratamos do senso comum da palavra arquitetura. Porém, dentro do universo da computação, esse paradigma se distancia do senso comum e se aproxima de sua definição técnica, que não se restringe a um espaço arquitetônico, mas abrange as técnicas que permitem a concepção planejada de qualquer coisa, neste caso, um software.

Com isso, pode-se dizer que <i>Arquitetura de Software compreende os elementos de um sistema, a relação entre eles, e suas propriedades,</i> vinsando ser a solução para problemas recorrentes do ofício, e auxiliar na tomada de decisões no decorrer do desenvolvimento.

## Arquitetura vs Design de Software

É mais comum do que se imagina associar incorretamente os conceitos de arquitetura e design de software. Por mais que haja uma interseção entre ambas, e que essa associação não seja de todo errônia, é importante diferenciar ambos os conceitos:

- Arquitetura: A arquitetura de software opera as relações entre os componentes de um sistema.

- Design: O design de software se concentra na implementação dos componentes, focando em detalhes. 

## Modelos de Arquitetura

Com o intuito de compreender um modelo de arquitetura específico (Clean), é importante conhecer e saber diferenciar as alternativas disponíveis e quando estas devem ser adotadas. Portanto, a seguir estão listados os principais modelos de arquitetura de software utilizados hoje em dia:

- [Model-view-controller (MVC)]()
- [Model-View-ViewModel (MVVM)]()

<!-- ## Model-view-controller (MVC)

Sendo um dos padrões de arquitetura mais populares, o MVC foi introduzido como um possível padrão em 1979 por Trygve Reenskaug, cinetista da computação norueguês. O modelo consiste em separar a aplicação em três camadas independentes: o Model, view e controller, o que permite dissociar a UI das regras de negócio do sistema, o que foi bastante inovador no periodo citado. Além disso, o MVC permite a reutilização de código, uma melhor compreensão e manutenção, e facilita a criação de multiplas interfaces, o que é bastante difundido na stack front-end. O trecho a seguir auxilia no entendimento de cada camada:

<img align="left" style="width: 300px;" src="https://user-images.githubusercontent.com/61476935/210247819-ce99b554-9b11-4032-b4cc-111d14810090.png">

### View

Responsável por conter a interface e tudo o que a compõe. É a partir da view que interação com as demais camadas se inicia e é nela que se encontra os arquivos de template, estilo e etc.

### Controller

Responsável por controllar a interação entre Model e View, recebendo as requisições do usuário (disparadas pela interface) e acessar os models para obter uma resposta concisa.

### Model

Responsável pelo acesso e manipulação de dados da aplicação. É no model que se concentram os métodos reponsáveis por consultar o banco de dados ou por acessar os endpoits de uma API integrada.

Além dos elementos que nomeiam o modelo, também é comum encontrar um quarto conceito: o <i>Router</i>. Este sendo o responsável por associar determinado método da camada de controle a um endereço (rota) do sistema. 

## Model-View-ViewModel (MVVM)

O padrão Model View ViewModel foi pensado pelo Arquiteto de Software John Gossman e a equipe da Microsoft em 2005, tendo como base o MVC e o MVP, com o intuito de possibilitar o <i>Data Binding (compartilhamento estavél e síncrono de informações entre uma fonte e um receptor ou entre duas fontes de dados)</i> junto ao Microsoft Silverlight, usado no desenvolvimento de navegadores e plug-ins. Sua criação também foi creditada à necessidade de dividir sistemas em camadas especializadas em determinadas funções, sendo essas camadas:

<img align="left" style="width: 350px;" src="https://user-images.githubusercontent.com/61476935/210266105-c4669697-15ef-493e-a86d-5fb81c2d8340.png">

### View

Assim como no MVC, a View se reponsabiliza por renderizar as informações obtidas das demais camadas, sendo essencialmente ignorante com relação a forma com que essas informações foram obtidas, se importanto apanas com o formato no qual precisa exibir as informações e com as demais rotinas associadas com a experiência do usuário, como atualizações de estado.

### ViewModel 

A ViewModel por sua vez, tem como intuito disponibilizar uma lógica de apresentação para a View e gerenciar seus de estados através de comandos e Data Binding, sendo a responsável por criar a ponte entre interface e data source, já que ambas não possuem conhecimento uma da outra. Além disso, pode ser função da ViewModel validar o fluxo de dados e garantir a consistência das informções exibidas e enviadas.

### Model

O papel do Model é encapsular a regra de negócio responsável por obter as informações de um outro serviço, seja uma API, banco de dados e etc. É responsabilidade do Model validar as informações obtidas das ações do usuário de acordo com a regra de negócio que atende ou é atendida pela aplicação em questão.

É bastante comum encontrar o padrão MVVM em ambientes Mobile, como Swift, Java, Dart e entre outros, visto que ele é implicitamente recomendado para projetos cujo foco está em desenvolver a interface tendo a regra de negócio como base. Além disso, cabe citar o [Observable Patters](https://www.devmedia.com.br/design-patterns-observer/16875) como referência para gerenciamento de estados em uma arquitetura MVVM; este que está diretamente associado a programação reativa, que por sua vez está muito presente da construção de interfaces de usuário em geral.   

## Microservices (microsserviços)

## Pipes-and-filters (PF)

## Peer-to-Peer (P2P)

## Service-Oriented Architecture (SOA)

## Publish-Subscribe (Pub/Sub)

## Client-server (cliente-servidor)

## Layers (Camadas) -->

# Por que a Clean Architecture ?

A <i>Clean Achitecture</i> se caracteriza pela compartimentação de um sistema em camadas, delegando a cada uma delas uma responsabilidade única, que só é observável pela camada imediatamente acima nas subdivisões da arquitetura. Antes de entendermos tais camadas e suas responsabilidades, é importante compreender as vantagens de aplicar uma arquitetura limpa quando iniciamos um novo projeto:

>Assim como qualquer modelo de arquitetura, a facilitação do entendimento e da manutenção durante a desenvolvimento, são visados quando se trata da arquitetura limpa. Manter o código coeso e fácil de manutenir é desejável quando se escala uma aplicação, porém, o principal trunfo da Clean Achitecture é o nível de desacomplamento das funcionalidades do sistema, ou seja, qualquer entidade que compõe um app pode facilmente ser substituído, pois, o desenvolvimento visa a idependência de cada camada, tendo a regra de negócio como ponto de partida, e como última necessidade a implementação dos mecanismos de obtenção e entrega da informações.

Com isso, a Clean Architecture permite que o sistema funcione independentemente de qualquer agente externo à linguagem, pois estes devem ser facilmente substituíveis. Tal desacoplamento permite ainda com que se execute testes de forma muito mais simples, diretamente nos métodos que compõem a regra de negócio do sistema, sem necessitar um banco de dados, API, ou qualquer fonte de informação. Resumindo, projetos que são desenvolvidos mediante a uma arquitetura limpa possuem:

- Independência de Framework;
- Testabilidade;
- Independência da Inteface do Usuário;
- Independência de Banco de Dados;
- Independência de Qualquer Elemento Externo;

Tendo definido a razão pela qual optar por uma arquitetura limpa é vantajoso, podemos entender seus aspectos em detalhes:

## Layers

<img src="https://user-images.githubusercontent.com/61476935/210369798-adbbebda-92c7-4d20-8f8a-2e096d4b5d67.png">

### Entities

A camada de <i>Entities</i> é a principal camada da arquitetura, e é a que primeiro recebe linhas de código. Nela se concentra tudo o que é pertinente a lógica de negócio, ou <i>Enterprise Business Rules (Regras de Negócio Corporativas)</i>, sendo geralmente um retrato das tabelas do banco de dados dentro do projeto. É na camada inicial que as propriedades, tipos e acessos de cada entidade se encontram, e por definirem uma regra, se repetem nos processos que envolvem as entidades.

### Use Cases

É na camada de <i>Use Cases</i> que são definidas as <i>Application Business Rules</i>, ou seja, é onde definimos o comportamento do sistema com base na comunicação com as regras de negócio corporativas, sendo esta a responsável pela comunicação com as entidades e por abstrair as assinaturas de métodos que serão obrigatóriamente criados na implementação dos casos de uso. Toda e qualquer informação terá que passar pela camada de casos de uso obrigatóriamente.

### Interface Adapters

A camada de <i>Interface Adapters</i> se responsabiliza pela conversão de dados e comunicação entre as camadas externas e internas. É nela que a entrada de dados da interface é adaptada para os casos de uso e entidades, assim como a saída de dados dos casos de uso e entidades são formatados convenientemente para que sejam exibidos na camada de apresentação.

### Frameworks & Drivers

Na camada mais externa estão os elementos alheios a regra de negócio, os que devem ser facilmente subistituíveis, como já foi dito. Nela encontramos os componentes cuja única função é permitir a comunicação com as camadas principais, sendo facilmente indentificados como a interface do usuário, bacos de dados, a web e etc. A ela só se deve expor o mínimo das camadas externas, necessário para a comunicação.

# Implementando a Clean Architecture

Um dos aspectos que torna a adoção da Clean Architecture problemática é, a primeira vista, o seu nível de complexidade. A implementação de multiplas camadas torna o desenvolvimento dificultoso a princípio. Porém, as camadas que definem os componentes da arquitetura limpa, não necessariamente serão implementadas na criação dos arquivos e pastas de um projeto. O que ocorre é a adaptação dessas camadas em três camadas principais. Estas são deicritas no modelo a seguir:

<img align="left" width="500px" src="https://user-images.githubusercontent.com/61476935/210375432-cfadd7b2-91f3-4bcc-9d71-4ec04aee166f.png">

### Presentation Layer



### Domain Layer

### Data Layer
