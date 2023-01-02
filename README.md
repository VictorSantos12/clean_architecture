# clean_architecture

A Clean Architecture, ou Arquitetura Limpa, é um padrão de arquitetura de sistemas criado por Rober Cecil Martin, popularmente conhecido na comunidade de tecnologia como [Uncle Bob](https://www.google.com/search?gs_ssp=eJzj4tbP1TcwNKoyyk5PMmD04izNS85JVUjKTwIAVZAHQg&q=uncle+bob&rlz=1C1ASUM_enBR992BR992&oq=Uncle+Bob&aqs=chrome.1.69i57j46i512j0i512l8.3321j0j7&sourceid=chrome&ie=UTF-8). Sendo inicialmente divulgada através do também popular "Arquitetura Limpa - O Guia do Artesão para Estrutura e Design de Software", é bastante difundida no mercado tech e amplamente adotado quando se trata de arquitetura de sistemas.

Antes de adentrar no que caracteriza a Clean Architecture, é importante entender do que se trata o tópico <i>Arquitetura</i> em desenvolvimento de sistemas, porque ela é necessária, e quais são as formas de atender a essa necessidade.

# Arquitetura de Software

Uma definição básica de arquitetura é que ela consiste no conjunto de princípios, normas, técnicas e materiais usdados para criar um espaço arquitetônico. Isso quando tratamos do senso comum da palavra arquitetura. Porém, dentro do universo da computação, esse paradigma se distancia do senso comum e se aproxima de sua definição técnica, que se trata de agrupar os princípios, normas e técnicas para a criação organizada de algo, neste caso, um software.

Com isso, pode-se dizer que <i>Arquitetura de Software compreende os elementos de um sistema, a relação entre eles, e suas propriedades,</i> vinsando ser a solução para problemas recorrentes do ofício, e auxiliar na tomada de decisões do decorrer do desenvolvimento.

## Arquitetura vs Design de Software

É mais comum do que se imagina associar incorretamente os conceitos de arquitetura e design de software. Por mais que haja uma interseção entre ambas, e que essa associação não seja de todo errônia, é importante diferenciar ambos os conceitos. 

A arquitetura de software opera as relações entre os componentes de um sistema, enquanto o design de software se concentra na implementação desses componentes, focando em detalhes. 

## Modelos de Arquitetura

Com o intuito de compreender um modelo de arquitetura específico (Clean), é importante conhecer e saber diferenciar as alternativas disponíveis e quando estas devem ser adotadas. Portanto, a seguir há uma descrição básica dos principais modelos de arquitetura de software utilizados hoje em dia:

## Model-view-controller (MVC)

Sendo um dos padrões de arquitetura mais populares, o MVC foi introduzido como um possível padrão em 1979 por Trygve Reenskaug, cinetista da computação norueguês. O modelo consiste em separar a aplicação em três camadas independentes: o Model, view e controller, o que permite dissociar a UI das regras de negócio do sistema, o que foi bastante inovador no periodo citado. Além disso, o MVC permite a reutilização de código, uma melhor compreensão e manutenção, e facilita a criação de multiplas interfaces, o que e bastante difundido na stack front-end. O trecho a seguir auxilia no entendimento de cada camada:

<img align="left" style="width: 250px;" src="https://user-images.githubusercontent.com/61476935/210247819-ce99b554-9b11-4032-b4cc-111d14810090.png">

### Model

Responsável pelo acesso e manipulação de dados da aplicação. É no model que se concentram os métodos reponsáveis por consultar o banco de dados ou por acessar os endpoits de uma API integrada.

### View

Responsável por conter a interface e tudo o que a compõe, sendo onde se encontra os arquivos HTML, de template e etc.

### Controller

Responsável por controllar a interação entre Model e View, recebendo as requisições do usuário (disparadas pela interface) e acessar os models para obter uma resposta concisa.

Além dos elementos que nomeiam o modelo, também é comum encontrar um quarto conceito: o <i>Router</i>. Este sendo o responsável por associar determinado método da camada de controle a um endereço (rota) do sistema. 

### Microservices (microsserviços)



## Pipes-and-filters (PF)

## Peer-to-Peer (P2P)

## Service-Oriented Architecture (SOA)

## Publish-Subscribe (Pub/Sub)

## Client-server (cliente-servidor)

## Layers (Camadas)