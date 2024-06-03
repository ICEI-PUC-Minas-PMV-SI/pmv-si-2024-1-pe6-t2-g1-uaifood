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

2. Processamento de Dados:

Adição ao Carrinho: Quando o usuário adiciona itens ao carrinho, as informações sobre os pratos selecionados, incluindo quantidade e preços, são enviadas ao backend e temporariamente armazenadas.

3. Armazenamento de Dados:

Banco de Dados: Informações dos usuários, detalhes dos restaurantes, menus de pratos, e pedidos são armazenados no banco de dados. O Bubble.io gerencia o armazenamento e a segurança dos dados utilizando práticas recomendadas.

4. Interações com APIs Externas:

Geolocalização: Para entregas, a API dos correios é utilizada para facilitar o preenchimentos de dados do endereço. 

5. Atualizações e Notificações:

Status do Pedido: Os dados do pedido são constantemente atualizados e disponibilizados para o usuário acompanhar o status em tempo real.

6. Exibição de Dados:

Interface do Usuário: Todos os dados processados e armazenados são apresentados ao usuário através de uma interface intuitiva e responsiva. Informações como menus de restaurantes, detalhes do pedido, e status de entrega são exibidos de forma clara e acessível.

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

## Implantação
[Instruções para implantar a aplicação distribuída em um ambiente de produção.]

1. Defina os requisitos de hardware e software necessários para implantar a aplicação em um ambiente de produção.
2. Escolha uma plataforma de hospedagem adequada, como um provedor de nuvem ou um servidor dedicado.
3. Configure o ambiente de implantação, incluindo a instalação de dependências e configuração de variáveis de ambiente.
4. Faça o deploy da aplicação no ambiente escolhido, seguindo as instruções específicas da plataforma de hospedagem.
5. Realize testes para garantir que a aplicação esteja funcionando corretamente no ambiente de produção.

## Testes
[Descreva a estratégia de teste, incluindo os tipos de teste a serem realizados (unitários, integração, carga, etc.) e as ferramentas a serem utilizadas.]

1. Crie casos de teste para cobrir todos os requisitos funcionais e não funcionais da aplicação.
2. Implemente testes unitários para testar unidades individuais de código, como funções e classes.
3. Realize testes de integração para verificar a interação correta entre os componentes da aplicação.
4. Execute testes de carga para avaliar o desempenho da aplicação sob carga significativa.
5. Utilize ferramentas de teste adequadas, como frameworks de teste e ferramentas de automação de teste, para agilizar o processo de teste.

# Referências
Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.

Documentação Oficial do Bubble.io: Bubble.io Documentation

Fórum da Comunidade Bubble.io: Bubble Forum

Bubble Academy: Bubble Academy

Documentação de Implantação do Bubble.io: Bubble.io Deployment Documentation

Bubble Apps Showcase: Bubble Apps Showcase
