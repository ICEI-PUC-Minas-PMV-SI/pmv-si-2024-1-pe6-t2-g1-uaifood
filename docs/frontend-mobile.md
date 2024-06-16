# Front-end Móvel
[Inclua uma breve descrição do projeto e seus objetivos.]

A Plataforma UaiFood tem como objetivo fornecer um aplicativo que possa ser utilizado pelos restaurantes, em alternativa às plataformas disponíveis no mercado. Com uma proposta simplificada, os restaurantes poderiam cadastrar as informações de seus empreendimentos, cardápios, horários, promoções, permitir que seus clientes cadastrem suas informações para facilitar as compras. 

A ideia é ter um software simples, de fácil navegabilidade, e que permita pequenas personalizações para que os restaurantes deixem o app com a sua identidade da marca, sem a necessidade de entender de programação.

Especificamente par ao app móvel, o aplicativo tem como objetivo gerenciar as vendas através desta estrutura própria, em que os clientes realizem suas compras com comodidade e praticidade, sendo atendida diretamente pelo restaurante em questão

## Tecnologias Utilizadas
[Lista das tecnologias principais que serão utilizadas no projeto.]

Plataforma de Desenvolvimento:

Bubble.io: Utilizaremos a plataforma Bubble.io, que permite o desenvolvimento de aplicativos web sem a necessidade de codificação tradicional. A Bubble.io facilita a criação de interfaces, a gestão de dados e a implementação de lógica de negócios através de uma abordagem visual.
Bibliotecas e Plugins Disponíveis no Bubble.io:

Plugins de UI/UX: Utilizaremos plugins disponíveis no Bubble.io para aprimorar a interface do usuário (UI) e a experiência do usuário (UX). Exemplos incluem plugins para elementos de design como sliders, carrosséis de imagens, gráficos interativos e animações.
Integrações de API: Plugins que permitem a integração com serviços de terceiros, como Google Maps para geolocalização, Stripe para pagamentos, e Twilio para SMS e notificações.
Ferramentas de Análise: Plugins para integrar ferramentas de análise e monitoramento, como Google Analytics e Hotjar, que ajudarão a monitorar o comportamento dos usuários e a performance do aplicativo.
Segurança: Plugins que adicionam camadas extras de segurança, como autenticação de dois fatores (2FA) e encriptação de dados.

## Arquitetura
[Descrição da arquitetura das aplicação móvel, incluindo os componentes e suas interações.]

A arquitetura do nosso aplicativo no Bubble.io será organizada de forma a maximizar a reutilização de componentes e a eficiência dos fluxos de trabalho. A seguir, uma descrição detalhada dos principais componentes e suas interações:

Componentes Principais:
Frontend:

Páginas de Interface: Cada página do aplicativo (como a página inicial, menu de restaurantes, carrinho de compras, etc.) será criada utilizando os elementos de interface gráfica do Bubble.io. Essas páginas serão projetadas para serem responsivas e intuitivas.
Elementos Reutilizáveis: Componentes comuns, como cabeçalhos, rodapés, e barras de navegação, serão criados como elementos reutilizáveis para garantir consistência e facilitar a manutenção.
Backend:

Banco de Dados: Utilizaremos o sistema de banco de dados integrado do Bubble.io para armazenar informações dos usuários, dados dos pedidos, inventário dos restaurantes, etc. O banco de dados será estruturado em diferentes tabelas com relações apropriadas para garantir integridade e eficiência.
Fluxos de Trabalho: Os fluxos de trabalho (workflows) no Bubble.io serão configurados para gerenciar a lógica de negócios, como processamento de pedidos, atualização de status dos pedidos, notificações em tempo real, e integração com serviços de pagamento.

## Modelagem da Aplicação
[Descreva a modelagem da aplicação, incluindo a estrutura de dados, diagramas de classes ou entidades, e outras representações visuais relevantes.]

![Diagrama dados](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/ca6def10-3609-42d8-bbfc-5576bc56a081)


![Diagrama](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/fb5d044b-2a6d-47ec-bc64-d251810cbd7a)


## Projeto da Interface
[Descreva o projeto da interface móvel da aplicação, incluindo o design visual, layout das páginas, interações do usuário e outros aspectos relevantes.]

A interface móvel da nossa aplicação de delivery foi projetada para ser intuitiva, responsiva e visualmente atraente, proporcionando uma experiência de usuário agradável e eficiente. Detalhamos o design visual e aspectos relevantes do projeto da interface.

Design Visual
Uma interface amigável e fácil de navegar.
Uma paleta de cores harmoniosa e consistente.
Usar uma tipografia clara e legível.
Um design que seja responsivo e adaptável a diferentes tamanhos de tela.

Elementos Visuais
Uma paleta principal com cores suaves e complementares, combinados com cores de destaque (como laranja) para botões e chamadas de ação.
Usar fontes modernas e legíveis, com tamanhos adequados para leitura em dispositivos móveis.
Uso de ícones simples e imagens de alta qualidade para ilustrar, pratos e outras informações relevantes.

### Wireframes
[Inclua os wireframes das páginas principais da interface, mostrando a disposição dos elementos na página.]

![Wireframe app - Tela principal - UAIfood](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/blob/main/docs/img/Menu-restaurante.jpg)
![Wireframe app - Detalhes do item - UAIfood](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/blob/main/docs/img/Detalhes_do_item.jpg)
![Wireframe app - Carrinho de pedidos - UAIfood](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/blob/main/docs/img/Carrinho.png)

### Design Visual
[Descreva o estilo visual da interface, incluindo paleta de cores, tipografia, ícones e outros elementos gráficos.]

Paleta de Cores: Cores vibrantes e atraentes para chamar a atenção do usuário. <br>
Tipografia: Fontes modernas e legíveis para garantir uma boa experiência de leitura. <br>
Ícones: Ícones intuitivos para representar diferentes categorias de alimentos e ações do usuário.

### Layout Responsivo
[Discuta como a interface será adaptada para diferentes tamanhos de tela e dispositivos.]

O layout será adaptado para dispositivos móveis com telas de diversos tamanhos, garantindo uma experiência consistente em diferentes modelos de dispositivos.

### Interações do Usuário
[Descreva as interações do usuário na interface, como animações, transições entre páginas e outras interações.]

Animar transições entre páginas para uma experiência mais fluida. Feedback visual para ações do usuário, como adicionar itens ao carrinho ou confirmar um pedido.

## Fluxo de Dados
[Diagrama ou descrição do fluxo de dados na aplicação.]

Fluxo de Dados
O fluxo de dados na nossa aplicação de delivery desenvolvida na plataforma Bubble.io é estruturado para garantir que as informações sejam processadas de maneira eficiente e segura, desde a entrada dos dados pelos usuários até o processamento e armazenamento no banco de dados. 

1. Entrada do Usuário:

Cadastro e Login: Os usuários fornecem suas informações pessoais, como nome, email e senha, para criar uma conta ou fazer login. Esses dados são validados e enviados ao servidor.

![Cadastro](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/dad8715a-0ac7-414c-b047-97c433154c77)

![Login](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/e029d983-0abb-4d66-83e8-62c3a4eb43b2)

2. Processamento de Dados:

Adição ao Carrinho: Quando o usuário adiciona itens ao carrinho, as informações sobre os pratos selecionados, incluindo quantidade e preços, são enviadas ao backend e temporariamente armazenadas.

![Restaurante](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/9771ebcd-77b5-4645-9c95-4384c6ebfcfe)

![Restaurante2](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/a01b9e0b-39a4-40f0-9bbe-1913bbc3f741)

![Cardap 1](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/4c95f5d7-2b1e-47f5-b1e7-dc51021dc4f3)

![Cardap2](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/ee7f0793-6dd9-4b55-9442-c2f027c20a1e)

![Cardap3](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/2249257b-679b-4fdd-96e4-acaa004f054f)

![Carrinho](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/7016de6f-fbce-4dd4-a0d7-a26ec916b8af)

![Carrinho2](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/30c51cd1-d0a5-4fe4-b61e-9c9634488fab)

3. Armazenamento de Dados:

Banco de Dados: Informações dos usuários, detalhes dos restaurantes, menus de pratos, e pedidos são armazenados no banco de dados. O Bubble.io gerencia o armazenamento e a segurança dos dados utilizando práticas recomendadas.

![image](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/699835b1-342d-4863-ac07-fe1ebcd110be)

![image](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/0fdc1bb1-ddd3-4a4b-95d1-01cea7c172ce)


4. Interações com APIs Externas:

Geolocalização: Para entregas, a API dos correios é utilizada para facilitar o preenchimentos de dados do endereço. 

![Perfil](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/fe9ec10e-1de1-4fe7-bc15-331391eb3d36)


5. Atualizações e Notificações:

Status do Pedido: Os dados do pedido são constantemente atualizados e disponibilizados para o usuário acompanhar o status em tempo real.

![pedido](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/f67fd1dd-aaee-4860-9f27-e1669534116d)


6. Exibição de Dados:

Interface do Usuário: Todos os dados processados e armazenados são apresentados ao usuário através de uma interface intuitiva e responsiva. Informações como menus de restaurantes, detalhes do pedido, e status de entrega são exibidos de forma clara e acessível.

Apresentado nas imagens anteriores. 

## Requisitos Funcionais

[Liste os principais requisitos funcionais da aplicação.]

RF01 - Gerenciar informações pessoais<br>
RF02 - Disparar notificações na alteração do status<br>
RF03 - Gerenciar pedidos<br>
RF04 - Visualizar catálogo do restaurante<br>
RF05 - Gerenciar carrinho<br>
RF06 - Avaliar restaurante/pedidos

## Requisitos Não Funcionais

[Liste os principais requisitos não funcionais da aplicação, como desempenho, segurança, escalabilidade, etc.]

RNF01 - Garantir a disponibilidade do app em 95% do tempo<br>
RNF02 - Tratar requisições em até 5s<br>
RNF03 - Permitir 100 conexões simultâneas

## Considerações de Segurança
[Discuta as considerações de segurança relevantes para a aplicação distribuída, como autenticação, autorização, proteção contra ataques, etc.]
Para autenticação Utilize o sistema de autenticação do Bubble, que suporta autenticação por email e senha.
Considere a implementação de autenticação multifator (MFA) para adicionar uma camada extra de segurança.
Bubble armazena senhas de forma segura usando hashing, garantindo que as senhas não sejam armazenadas em texto plano.
Autorização no Bubble para controlar quem pode ver, modificar ou deletar dados. Essas regras podem ser baseadas em funções de usuário definidas no banco de dados.
Utilize workflows para definir permissões específicas e garantir que cada usuário tenha acesso apenas às funcionalidades necessárias para sua função.

Proteção contra ataques o Bubble abstrai o acesso ao banco de dados através de sua interface visual, o que ajuda a prevenir injeções de SQL, pois não há inserção direta de código SQL.


## Implantação
[Instruções para implantar a aplicação distribuída em um ambiente de produção.]

1. Defina os requisitos de hardware e software necessários para implantar a aplicação em um ambiente de produção.

Não há requisitos específicos de hardware, pois utilizarei o Bubble.io, uma plataforma de desenvolvimento no-code que gerencia a infraestrutura necessária. Isso significa que não precisarei configurar servidores físicos ou virtuais.
Para acessar e gerenciar minha aplicação no Bubble.io, utilizarei um navegador da web moderno e atualizado, como Google Chrome, Mozilla Firefox, Microsoft Edge ou Safari. Além disso, é necessário uma conexão à Internet estável.

3. Escolha uma plataforma de hospedagem adequada, como um provedor de nuvem ou um servidor dedicado.

A hospedagem será feita diretamente no Bubble.io, que oferece uma plataforma de hospedagem integrada. Esta é a maneira mais simples e eficiente para implantar minha aplicação.
Caso minha aplicação necessite de mais recursos ou personalização no futuro, considerarei planos de preços mais elevados do Bubble.io, que oferecem maior capacidade de processamento, armazenamento e suporte.
   
5. Configure o ambiente de implantação, incluindo a instalação de dependências e configuração de variáveis de ambiente.

O Bubble.io gerencia todas as dependências necessárias para executar a aplicação, eliminando a necessidade de instalação manual.
No editor do Bubble.io, irei para Configurações e depois para a aba "API".
Adicionarei minhas variáveis de ambiente na seção "Secrets", como chaves de API e URLs de endpoints externos.

6. Faça o deploy da aplicação no ambiente escolhido, seguindo as instruções específicas da plataforma de hospedagem.

Clicaremos no botão "Deploy" (Implantar) no canto superior direito.
Selecionarei "Deploy to Live" (Implantar para Produção).
Confirmarei o deploy para mover minha aplicação do ambiente de desenvolvimento para o ambiente de produção.
Verificarei se todas as alterações estão refletidas na versão de produção.

7. Realize testes para garantir que a aplicação esteja funcionando corretamente no ambiente de produção.

Vamos verificar  se todas as funcionalidades principais da aplicação estão funcionando conforme esperado, testando fluxos de usuário como login, cadastro, navegação e transações.
Avaliaremos também o tempo de carregamento das páginas e a resposta do servidor. Embora o Bubble.io otimize automaticamente o desempenho, monitorarei para garantir uma boa experiência de usuário.
testaremos a segurança da aplicação, incluindo a verificação de autenticação, autorização e proteção contra vulnerabilidades comuns como XSS e CSRF.
Alem de verificar a interface do usuário em diferentes dispositivos e navegadores para garantir que a aplicação seja responsiva e acessível.
E por fim testaremos todas as integrações com serviços externos, como APIs de pagamento e serviços de email.

## Testes
[Descreva a estratégia de teste, incluindo os tipos de teste a serem realizados (unitários, integração, carga, etc.) e as ferramentas a serem utilizadas.]

1. Crie casos de teste para cobrir todos os requisitos funcionais e não funcionais da aplicação.

Desenvolveremos casos de teste detalhados que cobrem todos os requisitos funcionais e não funcionais da aplicação. Cada caso de teste descreverá um cenário específico, incluindo os passos a serem seguidos, as entradas necessárias e os resultados esperados.
Garantiremos que todos os requisitos especificados no documento de requisitos do projeto estejam cobertos pelos casos de teste. Isso incluirá funcionalidades principais como login, registro, processamento de pedidos, pagamento, etc., bem como requisitos não funcionais como desempenho, segurança e usabilidade.
   
2. Implemente testes unitários para testar unidades individuais de código, como funções e classes.

Testar unidades individuais de código, como funções, métodos e classes, para garantir que funcionem corretamente de forma isolada.
Utilizaremos o framework de teste do Bubble.io, que permite a criação e execução de testes unitários diretamente na plataforma. Caso seja necessário, também consideraremos ferramentas externas que possam ser integradas ao Bubble.io.
Escreveremos testes unitários para cada componente crítico da aplicação, verificando a lógica de negócios, manipulação de dados e outras funcionalidades isoladas.

3. Realize testes de integração para verificar a interação correta entre os componentes da aplicação.

Verificaremos a interação correta entre diferentes componentes da aplicação e garantir que eles funcionem juntos conforme o esperado. Além das ferramentas integradas ao Bubble.io, que permitem automatizar os testes de integração após cada mudança no código.
Realizaremos testes de integração que abrangem fluxos de trabalho completos, como o processo de login e registro, a realização de um pedido e o processamento de pagamentos. Esses testes garantirão que os componentes individuais interajam corretamente entre si.

4. Execute testes de carga para avaliar o desempenho da aplicação sob carga significativa.

Avaliaremos o desempenho da aplicação sob carga significativa e identificar pontos de falha ou gargalos de desempenho.
Os recursos de testes de carga do Bubble.io para simular múltiplos usuários acessando a aplicação simultaneamente.
Executaremos testes de carga simulando diferentes cenários de uso, como um grande número de usuários acessando a aplicação ao mesmo tempo, picos de tráfego durante horários de alta demanda e operações intensivas em recursos, como processamento de pedidos em massa.

5. Utilize ferramentas de teste adequadas, como frameworks de teste e ferramentas de automação de teste, para agilizar o processo de teste.

Utilizaremos sistema de monitoramento do Bubble.io para rastrear a performance e identificar problemas em tempo real. Geraremos relatórios detalhados para analisar os resultados dos testes e identificar áreas de melhoria.

# Referências
Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.

Documentação Oficial do Bubble.io: Bubble.io Documentation

Fórum da Comunidade Bubble.io: Bubble Forum

Bubble Academy: Bubble Academy

Documentação de Implantação do Bubble.io: Bubble.io Deployment Documentation

Bubble Apps Showcase: Bubble Apps Showcase
