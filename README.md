*Título Component Part 2(Aula 10)*

1. 
*MENUCOMPONENT.JS*

*BREVE DESCRIÇÃO PARA QUE SERVE ESSE ARQUIVO DENTRO DO PROJETO. TENTE RESPONDER AS SEGUINTES QUESTÕES:*

*Breve Descrição:* O arquivo MenuComponent.js é uma parte importante do projeto React. Ele cria o componente Menu, que mostra uma lista de pratos como um cardápio interativo. O usuário pode clicar nos pratos para ver mais detalhes. O design é feito com o Reactstrap, deixando a interface bonita e fácil de usar.

*-Quais os imports utilizados? (breve explicação)*
React e useState: necessários para criar componentes React e gerenciar o estado.
Componentes Reactstrap: Card, CardImg, CardImgOverlay, CardText, CardBody e CardTitle são usados ​​para criar interfaces visuais de cartões elegantes e responsivas.

*-HÁ COMPONESTES? O QUE FAZEM?*
-O componente *Menu*: Renderiza uma lista de pratos (cardápio interativo).
-Permite que o usuário selecione um prato e veja os detalhes desse prato.

*PARA QUE SERVE O ONDISHSELECT NO PROJETO?*
Quando o usuário clica em um item do menu, a função atualiza o status do prato selecionado.

*PARA QUE SERVE O RENDERDISH?*
Apresenta detalhes do prato selecionado. Mostra uma prévia com imagem, título e descrição ou um elemento vazio se nenhum prato for selecionado.

*PARA QUE SERVE O PROPS.DISHES.MAP?*
Itera sobre a lista de pratos recebida via props e cria cartões (cards) para cada prato. Isso exibe o cardápio na tela.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

2.
 *DISHES.JS*

*BREVE DESCRIÇÃO PARA QUE SERVE O ARQUIVO:*
O arquivo dishes.js inclui um conjunto de dados estáticos que representam os pratos de um menu. Ele é utilizado para simular ou fornecer informações sobre os pratos, como nome, imagem, categoria, preço e comentários, em um projeto de desenvolvimento web ou aplicativo.

*QUAIS PRIORIDADES?*
Cada prato (objeto no array DISHES) possui as seguintes propriedades:

-id: Identificador único do prato (número).
-name: Nome do prato (texto).
-image: Caminho da imagem do prato (texto).
-category: Categoria do prato (texto, como "mains", "appetizer", "dessert").
-label: Rótulo especial, como "Hot" ou "New" (texto, pode estar vazio).
-price: Preço do prato (texto numérico).
-description: Breve descrição do prato (texto).
-comments: Lista de comentários, onde cada comentário tem:

*id: Identificador único do comentário (número).*
*rating: Avaliação do prato (número de 1 a 5).*
*comment: Texto do comentário (texto).*
*author: Nome do autor do comentário (texto).*
*date: Data do comentário (formato ISO 8601, como "2012-10-16T17:57:28.556094Z").*


*QUE TIPO DE DATA É ULTILIZADO?*
A propriedade date dos comentários utiliza o formato ISO 8601 (YYYY-MM-DDTHH:mm:ss.sssZ), que é um padrão internacional para representar data e hora.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

*APP.JS*

*Breve Descrição do Arquivo:* Este arquivo cria o componente principal (App) em um projeto React. Ele cuida do estado global dos pratos, configura a barra superior com o nome do restaurante e exibe o menu dos pratos.

*PARA QUE SERVE O CONST [DISHES]?*
O const [dishes] usa o hook useState do React para guardar e gerenciar os dados dos pratos. O estado inicial é o array DISHES do arquivo dishes.js. Sem a função de atualização (setDishes), os pratos ficam fixos e não podem ser alterados.

*COMO FUNCIONA O <MENU DISHES={DISHES} />?*
O componente <Menu /> é chamado e recebe o array de pratos (dishes) como uma prop.

*Funcionamento:*
-A prop dishes fornece os dados dos pratos (de DISHES) para o componente filho Menu.
-Dentro de Menu, os dados são usados para mostrar a lista de pratos, provavelmente com um map para renderizar cada prato como um item visual.
-Isso permite que o componente App centralize os dados enquanto Menu cuida da exibição. É uma boa prática para separar responsabilidades.


