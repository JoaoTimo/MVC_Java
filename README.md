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
 # Interface do Usuário: A View é a parte da aplicação que o usuário vê e interage.
 # Apresentação de Dados: Formata e exibe informações recebidas do Model.
 # Interatividade: Permite que os usuários interajam com a aplicação, capturando entradas e eventos.

**Como funciona: **
 #Recebendo Dados:
A View obtém dados do Controller, que é responsável por buscar as informações no Model.

 #Renderização:
Após receber os dados, a View os apresenta em um formato visual (por exemplo, HTML em aplicações web).

 #Interação do Usuário:
Captura eventos de interação (cliques, envios de formulários) e os envia ao Controller para processamento.

 #Atualizações Dinâmicas:
Em aplicações web, pode atualizar a interface dinamicamente (ex.: usando AJAX) sem recarregar a página.

### Controller:
**O que é: **
**Como funciona: **

### REST
**O que é: **
**Como funciona: **

### CORS
**O que é: **
**Como funciona: **