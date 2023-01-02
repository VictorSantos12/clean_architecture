<div align="center">
  <img src="https://user-images.githubusercontent.com/61476935/210269491-dbdd0597-4227-4969-bd84-b72ba65cdf4a.png">
</div>
<br>

A Clean Architecture, ou Arquitetura Limpa, é um padrão de arquitetura de sistemas criado por Rober Cecil Martin, popularmente conhecido na comunidade de tecnologia como [Uncle Bob](https://www.google.com/search?gs_ssp=eJzj4tbP1TcwNKoyyk5PMmD04izNS85JVUjKTwIAVZAHQg&q=uncle+bob&rlz=1C1ASUM_enBR992BR992&oq=Uncle+Bob&aqs=chrome.1.69i57j46i512j0i512l8.3321j0j7&sourceid=chrome&ie=UTF-8). Sendo inicialmente divulgada através do também popular "Arquitetura Limpa - O Guia do Artesão para Estrutura e Design de Software", é bastante difundida no mercado tech e amplamente adotado quando se trata de arquitetura de sistemas.

Antes de adentrar no que caracteriza a Clean Architecture, é importante entender do que se trata o tópico <i>Arquitetura</i> em desenvolvimento de sistemas, porque ela é necessária, e quais são as formas de atender a essa necessidade.

# Arquitetura de Software

Uma definição básica de arquitetura é que ela consiste no conjunto de princípios, normas, técnicas e materiais usdados para criar um espaço arquitetônico. Isso quando tratamos do senso comum da palavra arquitetura. Porém, dentro do universo da computação, esse paradigma se distancia do senso comum e se aproxima de sua definição técnica, que se trata de agrupar os princípios, normas e técnicas para a criação organizada de algo, neste caso, um software.

Com isso, pode-se dizer que <i>Arquitetura de Software compreende os elementos de um sistema, a relação entre eles, e suas propriedades,</i> vinsando ser a solução para problemas recorrentes do ofício, e auxiliar na tomada de decisões do decorrer do desenvolvimento.

## Arquitetura vs Design de Software

É mais comum do que se imagina associar incorretamente os conceitos de arquitetura e design de software. Por mais que haja uma interseção entre ambas, e que essa associação não seja de todo errônia, é importante diferenciar ambos os conceitos. 

A arquitetura de software opera as relações entre os componentes de um sistema, enquanto o design de software se concentra na implementação desses componentes, focando em detalhes. 

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