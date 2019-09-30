---
template: post
title: "#04  \U0001F468‍\U0001F4BB Andamento do Projeto - Parte 1"
subtitle: ''
date: 2019-09-23T03:00:00Z
thumb_img_path: ''
content_img_path: ''
excerpt: ''

---
# **Protótipos**

### Protótipos de backend

Nos prototipos de backend que utilizam o firebase e ionic, foram criadas "Interfaces", algo mais similar às classes, entre os conceitos de POO tradicional.

**Protótipo de Login - Firebase**

[![Protótipo de Login](https://i.ibb.co/FYbSSYt/https-i-ytimg-com-vi-VPksu-Vc-Flec-hqdefault.jpg)](https://www.youtube.com/watch?v=VPksuVcFlec "Protótipo de Login")
[Acessar Vídeo](https://www.youtube.com/watch?v=VPksuVcFlec)[↪](https://youtu.be/l9EfHSSs2DA "Acessar vídeo")

No controle de contas e login, a interface em questão é a de User, que possui informações como nome, senha e e-mail. O próprio firebase oferece funções para login e signup, que facilitam o processo, testando apenas criar os formulários para passar essas informações e realizar a ação. Além disso o firebase oferece segurança e mensagens de erro que podem vir a ocorrer, na inserção de informações erradas pelo usuário.

**Protótipo de Product Management - Firebase**

[![Protótipo de Product Management](https://i.ibb.co/T110jwm/https-i-ytimg-com-vi-7-Dtg-GPLw-K04-hqdefault.jpg)](https://www.youtube.com/watch?v=7DtgGPLwK04 "Protótipo de Product Management")
[Acessar Vídeo](https://www.youtube.com/watch?v=7DtgGPLwK04)[↪](https://youtu.be/l9EfHSSs2DA "Acessar vídeo")

No product maanagement foi criado um CRUD que interage com a Interface de produtos, que possui informações como nome, criador e preço. O firebase armazena e passa as informações para que as funções do ionic populem a interface da aplicação. 

**Protótipo de Login e Product Management - Java Web com SQL**

[![Protótipo de Login e Product Management - Java Web com SQL](https://i.ibb.co/th4bghF/https-i-ytimg-com-vi-s0-40f-RYWVI-maxresdefault.jpg)](https://www.youtube.com/watch?v=s0_40fRYWVI "Protótipo de Login e Product Management - Java Web com SQL")
[Acessar Vídeo](https://www.youtube.com/watch?v=s0_40fRYWVI)[↪](https://youtu.be/l9EfHSSs2DA "Acessar vídeo")

No protótipo construído utilizando Java e SQL, obedecendo ao padrão da arquitetura MVC, criamos duas classes modelo: produtos, que recebem descrição preço e nome; e usuários, que recebem username, e-mail e senha, suas respectivas regras de negócio (data access object) com suas conexões ao banco de dados. Foram criadas tabelas que recebem as mesmas variáveis das classes, como colunas.

Para realizar o login, utilizamos um select para comparar o que foi passado nos campos do formulário de login com o que está no banco de dados. Para inscrever um novo usuário, o formulário preenchido passa as informações para um insert que realiza a operação na nossa base em SQL. 
Já na parte da exposição de produtos, a camada view foi feita por JSPs (Java server page), onde é realizado um select que passa para a camada de controle, as servlets com suas regras de interação, as informações a serem populadas na interface web do sistema. Utilizamos Session para manter as informações do usuário enquanto navegamos por diferentes htmls e para futuramente alimentar o cookie.

### Protótipos de Design

##### Protótipos de Baixa Fidelidade

Os protótipos abaixo foram feitos com abordagem "mobile-first", levando em consideração que estatisticamente o acesso a websites se dá através de aparelhos móveis. Na nossa ideia a plataforma final será responsiva e terá versões adaptadas ideais para cada tipo dos aparelhos mais comuns.

**Página principal + Infográficos**

![](/images/00.png)
Página Inicial, com imagens, título, botão "Call to Action", Botões de menu, carrinho e um que leva diretamente para a listagem de produtos. Abaixo da tela há uma ideia de tela de carregamento, se trata da ilustração e animação vetorial(em svg, isto é, compatível com a web) de um de um mascote, apelidado de "Poxa" criado por um dos artesãos.

![](/images/01.png)
Protótipo do menu de contexto, baseado no padrão contemporâneo de menu hamburger, cobrindo a tela inteira e listando as páginas/seções presentes na arquiteruda do sistema. Adicionamos também uma proposta de formato de menu, onde há uma pequena parte inferior para fechar o menu, dando assim uma segunda opção de interação.

![](/images/02.png)
![](/images/03.png)
![](/images/04.png)
Estas três páginas mostram a base para a estrutura do site, conteúdo necessário, infográficos necessários, posicionamento dos grafismos, propostas de diagramação e interação, etc, a ideia é que o menu esteja sempre disponível para navegar e cada seção pode levar para uma página com mais detalhes sobre cada tópico específico.

![](/images/05.png)
Nesta última seção estão disponíveis o rodapé e um pequeno formulário de interesse para contato, a ideia é que nesta parte o usuário seja fidelizado ao demonstrar interesse e disponibilizar seu email para possíveis contatos futuros com a plataforma, recebimento de emails com atualizações, etc.

**Carrinho + Página de Produto**

![](/images/011.png)
Esta tela representa a página com o carrinho aberto, nela você pode consultar os produtos adicionados, adicionar mais ou diminuir em quantidade, checar todos os valores detalhados(inclusive o frete), adicionar cupom de desconto, fechar e continuar a compra. Caso clique em cupom de desconto o usuário é apresentado a uma modal com um formulário e precisa escrever o código necessário. Caso continue o usuário partirá para o checkout da compra com preenchimento de formulário e possivelmente integração com alguma plataforma terceira de vendas(Google Pay, Mercado Livre etc). 

![](/images/012.png)
![](/images/013.png)
Para finalizar, aqui está prototipada a tela para um produto, mostrando valor, ficha técnica, história, cadeia produtiva em relação ao produto etc, o foco é mostrar ao usuário o valor real deste produto e quanto o produtor lucra e trabalha para chegar naquele resultado, sem "dark patterns", tornando o sistema confiável e transparente.


##### Captura de imagens

Na última quarta-feira(25/09) o Matheus Brandão e o Bruno Cidade foram visitar a comunidade de Moita Redonda e captaram algumas imagens para que possamos analisar como podemos utilizar isto no contéudo que estamos criando ou como deixar isto interativo. Foram captadas imagens de drone e câmera 360, que ainda estão sendo curadas pela equipe, por isso não iremos disponibilizar no momento, mas temos este vídeo para mostrar algo:

[Acessar Vídeo](https://drive.google.com/file/d/1odeNwyJrQBwxG9_WmahkkXZ-zgGyCWVl/view?usp=sharing)[↪](https://drive.google.com/file/d/1odeNwyJrQBwxG9_WmahkkXZ-zgGyCWVl/view?usp=sharing "Acessar vídeo")


##### Reunião com especialistas

**Maria Fernandes**

O Mateus Targino faz parte da comunidade de Design de Interação IxDA Fortaleza e foi para o evento do Dia Mundial do Design de Interação(24/09), o tema deste ano era "Trust and Responsability", coincidentemente foi abordado o tema de consumo consciente e Design Social, maior coincidência ainda foi o fato de que havia uma das líderes da comunidade local que desenvolve trabalhos com este teor, participando como voluntária em projetos da Ceart relacionados a artesanato e outros projetos pessoais pelos quais já passou. Na última sexta-feira(27/09), o integrante da equipe fez contato com Maria Fernandes para marcar uma reunião online e preparar algumas perguntas para adquirirmos conhecimento e termos alguma orientação mais pragmática de alguém que trabalha em uma área mais próxima da nossa, não sabemos ainda o dia mas idealmente será esta semana ainda e de preferência juntamente com os integrantes do Varal(Laboratório de Design Social).


