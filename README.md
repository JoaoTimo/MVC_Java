# Pesquisa sobre conceitos em Java
## MVC 

### Model

**O que é**:  
O Model representa a lógica de negócio e os dados do aplicativo. Ele é responsável por gerenciar as regras de negócio, acessar e armazenar informações, e, de forma geral, manter o estado da aplicação.

**Como funciona**:  
O Model encapsula a lógica central da aplicação e as interações com a camada de persistência de dados (como bancos de dados). Ele não se preocupa com a interface do usuário ou como os dados são exibidos, o que garante uma separação clara entre dados e apresentação.

#### Em resumo, o Model:
- Manipula os dados e suas validações.
- Interage com o banco de dados ou serviços externos.
- Notifica mudanças de estado para que a **View** seja atualizada.

### View: 
**O que é: **
 1. Interface do Usuário: A View é a parte da aplicação que o usuário vê e interage.
 2. Apresentação de Dados: Formata e exibe informações recebidas do Model.
 3. Interatividade: Permite que os usuários interajam com a aplicação, capturando entradas e eventos.

**Como funciona: **
 --Recebendo Dados:
A View obtém dados do Controller, que é responsável por buscar as informações no Model.

 --Renderização:
Após receber os dados, a View os apresenta em um formato visual (por exemplo, HTML em aplicações web).

 --Interação do Usuário:
Captura eventos de interação (cliques, envios de formulários) e os envia ao Controller para processamento.

 --Atualizações Dinâmicas:
Em aplicações web, pode atualizar a interface dinamicamente (ex.: usando AJAX) sem recarregar a página.

### Controller:
**O que é:**

A camada de controle (Controller) no padrão MVC (Model-View-Controller) é o componente que gerencia o fluxo de dados entre a interface de usuário (View) e a lógica de negócio (Model). Sua função principal é receber as requisições dos usuários, processar essas requisições de acordo com as regras da aplicação e determinar qual será a resposta apropriada, interagindo diretamente com a camada de modelo para realizar operações sobre os dados.

Em uma aplicação Java, essa camada é geralmente implementada com Servlets ou frameworks como Spring MVC, JSF, entre outros.

**Como funciona:**

#### Funções da Camada Controller:

1. **Receber Requisições:** O Controller intercepta as requisições HTTP feitas pelos usuários, identifica o que foi solicitado e direciona a ação correta com base na URL e nos parâmetros.

2. **Processar Requisições:** Ele chama métodos da camada Model para realizar operações de negócios, como inserir, atualizar ou buscar dados, delegando a lógica de negócios para o Model.

3. **Gerenciar Respostas:** Após o processamento, o Controller escolhe qual página (View) será exibida ou redireciona o usuário, enviando dados para a interface se necessário.

4. **Validação e Autenticação:** Verifica se os dados de entrada são válidos e controla o acesso do usuário, garantindo que apenas usuários autenticados realizem certas ações.

### REST
**O que é:**

É um estilo arquitetônico. Ele se fundamenta em princípios que visam facilitar a interação e a comunicação entre sistemas distribuídos, especialmente na web. REST é amplamente utilizado para criar APIs que permitem que diferentes aplicativos se comuniquem de maneira eficiente e escalável.

**Como funciona:**

### RECURSOS
Os recursos são identificáveis por URIs (Uniform Resource Identifiers). Cada recurso tem uma URL única, que permite o acesso e a manipulação.

### MÉTODOS HTTP

As interações com esses recursos são realizadas por meio de métodos HTTP, como GET (para recuperar dados), POST (para criar novos recursos), PUT (para atualizar recursos existentes), PATCH (para atualizações parciais) e DELETE (para remover recursos).

### STATELESS

Uma característica importante do REST é que ele é stateless, ou seja, cada requisição é independente e contém todas as informações necessárias, sem que o servidor armazene estado entre elas.

### REPRESENTAÇÕES

Os dados podem ser retornados em diferentes formatos, como JSON ou XML, permitindo flexibilidade na comunicação entre cliente e servidor.

### CACHE

O uso de cache pode otimizar o desempenho das APIs, armazenando respostas e evitando requisições desnecessárias ao servidor.

### HATEOAS

O conceito de HATEOAS permite que o servidor forneça links nas respostas, ajudando os clientes a descobrir interações disponíveis e facilitando a navegação pela API.

