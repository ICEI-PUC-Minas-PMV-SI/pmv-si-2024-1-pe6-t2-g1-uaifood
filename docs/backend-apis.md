# APIs e Web Services

O planejamento de uma aplicação de APIS Web é uma etapa fundamental para o sucesso do projeto. Ao planejar adequadamente, você pode evitar muitos problemas e garantir que a sua API seja segura, escalável e eficiente.

Aqui estão algumas etapas importantes que devem ser consideradas no planejamento de uma aplicação de APIS Web.

[Inclua uma breve descrição do projeto.]


ESTRUTURA DA APLICAÇÃO

Iremos descrever neste documento informações a respeito do UaiFood, uma aplicação cujo o objetivo é permitir que os restaurantes possuam uma alternativa aos grandes players do mercado, que, ao disponibilizar seus serviços de vendas através da internet, abocanham significativa parcela do faturamento bruto destes restaurantes, tornando o produto caro para o consumidor final.
Para resolver esse problema, o UaiFood tem a proposta de ser uma plataforma escalável, em que cada restaurante irá possuir sua própria versão do aplicativo, com toda a sua estrutura apartada, de forma padronizada, facilitando a construção e manutenção da aplicação, e permitindo que vários empreendimentos possam utilizar dos serviços de comercialização online.
Para a construção do app UaiFood, optamos por utilizar o Bubble.io, uma plataforma que permite o desenvolvimento de softwares sem a utilização de código. A escolha foi motivada por alguns aspectos específicos, tais como a praticidade na construção da aplicação, o fato de a própria plataforma hospedar a aplicação construída,e também para permitir que toda a equipe, indiferente da especialização de cada um dos membros pudesse contribuir sem limitações de conhecimento em uma linguagem de programação específica.



## Objetivos da API

O primeiro passo é definir os objetivos da sua API. O que você espera alcançar com ela? Você quer que ela seja usada por clientes externos ou apenas por aplicações internas? Quais são os recursos que a API deve fornecer?

Seu principal propósito é facilitar o desenvolvimento de aplicações web e móveis, oferecendo uma solução fácil de integrar que permite o preenchimento automático de formulários com base no CEP fornecido pelo usuário. Além disso, a API busca garantir a precisão das informações fornecidas, utilizando fontes de dados confiáveis. Ao promover a eficiência operacional e estimular a inovação em diversos setores. Em resumo, a API nossa api visa simplificar e otimizar o acesso a informações de endereço no Brasil, beneficiando os usuarios com essa facilidade.


## Arquitetura


A arquitetura da API ViaCEP é fundamentada nos princípios da arquitetura REST, utilizando comunicação via HTTP, endpoints padronizados e formato de dados estruturado. A comunicação entre clientes e servidor ocorre por meio de solicitações HTTP, seguindo um modelo Cliente-Servidor. A API é stateless e escalável, garantindo eficiência no processamento de um grande volume de solicitações sem comprometer o desempenho. Como estamos utilizando a plataforma bubble.io que possibilita a total integração com a api.

## Modelagem da Aplicação
[Descreva a modelagem da aplicação, incluindo a estrutura de dados, diagramas de classes ou entidades, e outras representações visuais relevantes.]
ESTRUTURA DO BANCO DE DADOS

A modelagem de dados estrela é uma abordagem utilizada em data warehousing, onde os dados são organizados em torno de uma tabela central, chamada de tabela fato, e tabelas secundárias, chamadas de tabelas de dimensão. Na tabela fato, são armazenados os fatos ou medidas centrais do negócio, como vendas ou transações, enquanto as tabelas de dimensão representam diferentes perspectivas dos dados, como tempo, produto ou localização. As chaves estrangeiras na tabela fato estabelecem relacionamentos com as chaves primárias das tabelas de dimensão, permitindo análises multidimensionais. Essa estrutura em forma de estrela simplifica consultas analíticas complexas e facilita a compreensão e a análise dos dados de negócio.

Utilizando de uma arquitetura estrela, o Banco de Dados da aplicação é responsável por abrigar as informações que são processadas no UaiFood.
O Banco de Dados irá contar com uma estrutura SQL que, em várias tabelas, irá consolidar as informações referentes às contas dos usuários do sistema, informações sobre os itens disponíveis nos cardápios de cada restaurante, pedidos realizados, validação dos pagamentos dos pedidos e informações dos restaurantes, de forma individualizada, evitando assim o acesso à base de clientes entre os contratantes da plataforma.
A seguir, trataremos sobre a divisão das tabelas do banco de dados, explicando a divisão e os campos que as mesmas possuem.
Restaurante: Nesta tabela estão dispostas informações sobre o restaurante contratante da solução. Esta tabela personifica o restaurante, com as informações de identificação do restaurante, além de outras informações relevantes. Esta tabela contará com os seguintes campos:
ID_Restaurante: campo de identificação do restaurante com um código. Irá abrigar um valor numérico que identifica o restaurante na base de dados do UaiFood;

descrição_Restaurante: campo que trará ao cliente final informações gerais do restaurante. Irá abrigar um texto;

endereço_Restaurante: campo textual para informar ao consumidor o endereço do restaurante. Abriga um texto;

abertura_Restaurante: campo numérico no formato “hh:mm” que informa o horário de abertura do restaurante;

fechamento_Restaurante: campo numérico no formato “hh:mm” que informa o horário de encerramento das atividades do restaurante;

foto_Restaurante: recebe um arquivo do tipo imagem, para que seja a identidade do restaurante dentro do aplicativo.

Clientes: Esta tabela irá abrigar todas as informações sobre os usuários cadastrados para cada restaurante, tanto para os clientes quanto para os operadores do restaurante, que irão lidar com a resolução dos pedidos.

Id_Conta: campo de identificação do cadastro do cliente do restaurante em questão. Irá abrigar um valor numérico que identifica a conta do cliente na base de dados do UaiFood;

nome_Conta: campo textual que recebe o nome do usuário cadastrado;

email_Conta: campo textual para salvar o email utilizado para o cadastro;
cep_Conta: campo do tipo numérico que irá abrigar o CEP do endereço de entrega para os pedidos;

endereço_Conta: campo do tipo textual que irá abrigar o nome da rua, que será obtido através de uma API utilizada para validar o endereço e auxiliar no preenchimento do cadastro;

número_Conta: campo numérico para inserção do número da residência para entrega dos pedidos realizados;

complemento_Conta: campo textual para inserção do complemento do endereço cadastrado. Não é um campo cujo preenchimento é obrigatório;

bairro_Conta: campo textual para abrigar o nome do bairro do cliente, recebido através da API mencionada anteriormente;

cidade_Conta: campo textual para abrigar o nome da cidade do cliente, recebido através da API mencionada anteriormente;

telefone_Conta: campo do tipo textual que trará o registro de um telefone para contato com o cliente. Este campo é do tipo textual para que seja permitido a utilização de determinados símbolos, como hífens, parênteses e outros comumente utilizados para telefones de contato;

foto_Conta: recebe um arquivo do tipo imagem, para que seja a identidade do cliente do restaurante dentro do aplicativo. Este não é um campo de preenchimento obrigatório;

tipoPagamento_Conta: campo de seleção múltipla que irá identificar o método de pagamento que o cliente irá utilizar em seus pedidos;

númeroCartão_Conta: campo numérico que irá trazer dados do método de pagamento (cartões) utilizado pelo cliente;

validadeCartão_Conta: campo numérico do tipo data (mm/aa) que irá trazer dados do método de pagamento (cartões) utilizado pelo cliente;

cvvCartão_Conta: campo numérico que irá trazer dados do método de pagamento (cartões) utilizado pelo cliente;

nomeCartão_Conta: campo do tipo textual para informação do nome impresso no cartão cadastrado

Staff: Esta tabela específica é responsável por abrigar informações sobre as contas dos funcionários e pessoas que terão acesso ao UaiFood por parte do restaurante.

Id_Staff: campo de identificação do cadastro do funcionário do restaurante em questão. Irá abrigar um valor numérico que identifica a conta na base de dados do UaiFood;

nome_Staff: campo textual que recebe o nome do usuário cadastrado;

email_Staff: campo textual para salvar o email utilizado para o cadastro;

cep_Staff: campo do tipo numérico que irá abrigar o CEP do endereço do funcionário cadastrado;

endereço_Staff: campo do tipo textual que irá abrigar o nome da rua, que será obtido através de uma API utilizada para validar o endereço e auxiliar no preenchimento do cadastro;

número_Staff: campo numérico para inserção do número da residência do funcionário cadastrado;

complemento_Staff: campo textual para inserção do complemento do endereço cadastrado. Não é um campo cujo preenchimento é obrigatório;

bairro_Staff: campo textual para abrigar o nome do bairro do funcionário do restaurante, recebido através da API mencionada anteriormente;

cidade_Staff: campo textual para abrigar o nome da cidade do funcionário do restaurante, recebido através da API mencionada anteriormente;

telefone_Staff: campo do tipo textual que trará o registro de um telefone para contato com o funcionário. Este campo é do tipo textual para que seja permitido a utilização de determinados símbolos, como hífens, parênteses e outros comumente utilizados para telefones de contato;

foto_Staff: recebe um arquivo do tipo imagem, para que seja a identidade do colaborador do restaurante dentro do aplicativo. Este não é um campo de preenchimento obrigatório;

banco_Staff: campo numérico que recebe o número de identificação do banco em que o funcionário recebe seu salário;
agencia_Staff: campo numérico que recebe o número de identificação da agência do banco em que o funcionário recebe seu salário;

contaSalario_Staff: campo textual que recebe o número de identificação da conta no banco em que o funcionário recebe seu salário. Este é um campo do tipo textual para que seja possível inserir um “hífen” que separa o número da conta do dígito verificador;

cargo_Staff: Campo textual que traz o cargo do colaborador a qual o cadastro se refere.

Cardápio: Irá compor todos os ítens disponíveis para consumo dos clientes do restaurante. Esta tabela possui campos específicos para a descrição do prato, valor, e uma imagem ilustrativa.

Id_Produto: campo de identificação do prato oferecido pelo restaurante com um código. Irá abrigar um valor numérico para identificação;

nome_Produto: campo textual que recebe o nome do prato cadastrado pelo restaurante;

valor_Produto: campo numérico (moeda) que recebe o valor unitário do prato em questão;

descrição_Produto: campo que trará ao cliente final informações gerais do prato oferecido pelo restaurante. Neste campo, a administração do restaurante irá inserir as características e ingredientes do prato em questão. Irá abrigar um texto;

foto_Produto: recebe um arquivo do tipo imagem, para que seja inserido junto às informações do prato dentro do aplicativo.

Pagamento: Esta tabela irá consolidar as informações sobre os status de pagamentos realizados através da plataforma, e os pedidos a quais se referem.

Id_Pagamento: campo de identificação do pagamento do pedido realizado pelo cliente com um código. Irá abrigar um valor numérico para esta identificação;

status_Pagamento: campo textual com seleção múltipla que irá abrigar as informações a respeito do status do pagamento do pedido realizado.

Pedido: principal tabela da estrutura, esta tabela irá reunir informações de todas as demais, através de campos chave para identificação dos pedidos realizados. Buscando informações sobre os ids dentro das demais tabelas, dentro dos registros de pedidos estarão contidas as informações do solicitante (tabela contas/usuários), os itens solicitados (tabela cardápio), informações sobre o processamento de pagamento (tabela pagamento).

Id_Pedido: campo de identificação do pedido realizado pelo cliente ao restaurante com um código. Irá abrigar um valor numérico;

status_Pedido: campo textual com seleção múltipla que irá abrigar as informações a respeito do status do pedido dentro do ciclo de vida do pedido;

Qtde_Pedido: campo numérico que trará a quantidade pedida pelo cliente, em relação aos itens inseridos no pedido;

total_Pedido: campo numérico do tipo moeda que trará o valor total a ser pago pelo cliente por todos os itens solicitados no pedido realizado.

É importante lembrar que as tabelas também possuem campos que são compartilhados entre elas, geralmente acoplados através dos campos de “IDs” de cada uma das tabelas.

Como exemplo, temos a tabela “Pedido”, que é necessário que haja uma forma de identificação do cliente que fez a solicitação, para isso, essa tabela “importa” campos específicos da tabela “Clientes”.




![Db UaiFood](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/eba71e07-1ee9-4def-b913-5ff5a8157b31)



## Fluxo de Dados

[Diagrama ou descrição do fluxo de dados na aplicação.]

Cadastro de Usuário:
O usuário acessa o aplicativo e inicia o processo de cadastro.
Ele fornece suas informações pessoais, como nome, endereço de e-mail e senha.
Após preencher o formulário de cadastro, o usuário envia os dados para o servidor.
O servidor recebe os dados, valida as informações e armazena o perfil do usuário no banco de dados.

![image](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/037b631c-b706-4be7-bf1b-49ab0307a01d)

Seleção de Pratos:
O usuário final (consumidores do restaurante) poderão selecionar os pratos disponíveis. Nesta tela, cada usuário poderá selecionar dentre todos os pratos, aquele(s) que irá solicitar.
Após selecionar o(s) prato(s), o usuário seguirá para as telas de confirmação de pedidos, quantidades, endereço para entrega e formas de pagamento, até que finalizae o seu pedido ao restaurante.

![image](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/ee5f48be-9a82-412c-927e-cfc7ea59d635)

Cadastro do Restaurante:
O restaurante acessa a plataforma e inicia o processo de cadastro.
Ele fornece informações sobre o restaurante, como nome, endereço, tipo de culinária, horário de funcionamento, entre outros.
O restaurante também insere detalhes do cardápio, incluindo pratos disponíveis, descrições e preços.
Após preencher o formulário de cadastro, o restaurante envia os dados para o servidor.
O servidor recebe os dados, valida as informações e armazena o perfil do restaurante juntamente com o cardápio no banco de dados.

![image](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/5c04c9fa-f8cd-4a1d-9652-3a28a92421a4)
![image](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/f9e637ce-86f3-4792-815b-5cd2b9bcf061)
![image](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/f16ded0c-afc1-4295-aac1-208e63b64ec5)

Gerenciamento de Informações:
O restaurante pode acessar seu perfil a qualquer momento para atualizar informações, como horário de funcionamento, cardápio ou detalhes de contato.
Essas atualizações são enviadas ao servidor, que verifica e atualiza as informações no banco de dados.
Os usuários do aplicativo podem navegar pelos restaurantes cadastrados e visualizar seus respectivos cardápios e informações.
Quando um usuário faz um pedido, os detalhes são enviados ao restaurante correspondente, que pode então preparar e entregar o pedido.


## Requisitos Funcionais

- Cadastro e edição de pratos;
- Cadastro e edição de usuários;
- Realização de pedidos;

## Requisitos Não Funcionais

[Liste os principais requisitos não funcionais da aplicação, como desempenho, segurança, escalabilidade, etc.]
- Escalabilidade: ser possível ser utilizada para mais de um restaurante;
- Não apresentar gargalos em picos de utilização;
- Disponibilidade 

## Tecnologias Utilizadas

Existem muitas tecnologias diferentes que podem ser usadas para desenvolver APIs Web. A tecnologia certa para o seu projeto dependerá dos seus objetivos, dos seus clientes e dos recursos que a API deve fornecer.

[Lista das tecnologias principais que serão utilizadas no projeto.]

Escolhemos como tecnologias o Bubble.IO como plataforma de desenvolvimento e publicação e o dbdesign para a criação da base de dados.

## API Endpoints

[Liste os principais endpoints da API, incluindo as operações disponíveis, os parâmetros esperados e as respostas retornadas.]

### Endpoint 1
- Método: GET
- URL: /endpoint1
- Parâmetros:
  - param1: [descrição]
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "message": "Success",
      "data": {
        ...
      }
    }
    ```
  - Erro (4XX, 5XX)
    ```
    {
      "message": "Error",
      "error": {
        ...
      }
    }
    ```

    Consulta por CEP:
Endpoint: GET https://viacep.com.br/ws/{CEP}/json/
Descrição: Este endpoint permite obter informações detalhadas de endereço com base no CEP fornecido. Ao fazer uma solicitação para este endpoint, substitua {CEP} pelo CEP desejado para consulta. Por exemplo, se você quiser informações sobre o CEP "01001-000", a URL completa seria https://viacep.com.br/ws/01001000/json/.
Parâmetros:
{CEP}: O CEP que você deseja consultar. Deve ser um valor numérico de 8 dígitos.
Exemplo de Resposta (JSON):
json
Copy code
{
  "cep": "01001-000",
  "logradouro": "Praça da Sé",
  "complemento": "lado ímpar",
  "bairro": "Sé",
  "localidade": "São Paulo",
  "uf": "SP",
  "ibge": "3550308",
  "gia": "1004",
  "ddd": "11",
  "siafi": "7107"
}
Descrição dos Campos:
cep: O CEP consultado.
logradouro: O logradouro associado ao CEP.
complemento: Complemento do endereço, se houver.
bairro: O bairro associado ao CEP.
localidade: A cidade associada ao CEP.
uf: A sigla do estado associado ao CEP.
ibge: O código IBGE da cidade.
gia: O código GIA da cidade.
ddd: O DDD da cidade.
siafi: O código SIAFI da cidade.
Este endpoint fornece informações precisas de endereço com base no CEP fornecido, facilitando o desenvolvimento de aplicações que requerem dados de localização no Brasil.

![image](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/ad983916-7868-4609-946a-6029c177d691)


## Considerações de Segurança

[Discuta as considerações de segurança relevantes para a aplicação distribuída, como autenticação, autorização, proteção contra ataques, etc.]

Para garantir a segurança ao usar o Bubble.io e a API ViaCEP em nosso projeto, foi fundamental implementar medidas de segurança como autenticação robusta, validação de entrada de dados, criptografia de dados sensíveis e monitoramento contínuo de atividades. Além disso, é importante manter o software atualizado e adotar práticas de segurança recomendadas para proteger os dados dos usuários e garantir a integridade da aplicação.

## Implantação

[Instruções para implantar a aplicação distribuída em um ambiente de produção.]

1. Defina os requisitos de hardware e software necessários para implantar a aplicação em um ambiente de produção.
2. Escolha uma plataforma de hospedagem adequada, como um provedor de nuvem ou um servidor dedicado.
3. Configure o ambiente de implantação, incluindo a instalação de dependências e configuração de variáveis de ambiente.
4. Faça o deploy da aplicação no ambiente escolhido, seguindo as instruções específicas da plataforma de hospedagem.
5. Realize testes para garantir que a aplicação esteja funcionando corretamente no ambiente de produção.

Para implantar a API ViaCEP no Bubble.io que foi o sistema que escolhemos para desenvolver nosso trabalho fizemos:

Criação de uma Chamada na API:
Dentro do seu aplicativo no Bubble.io, vá para a seção "Data" e clique em "API Connector" para criar uma nova chamada à API.
Configurar a Chamada à API:
Adicione o URL do endpoint da API ViaCEP para consulta por CEP (por exemplo, https://viacep.com.br/ws/01001000/json/) e defina o método HTTP como GET.
Parâmetros da Chamada:
Adicione um parâmetro para o CEP que você deseja consultar. Você pode configurar isso como um campo dinâmico se o CEP for inserido pelos usuários do seu aplicativo.
Processar a Resposta:
No Bubble.io, você pode mapear os campos da resposta JSON da API ViaCEP para campos em seu aplicativo. Por exemplo, você pode mapear o campo "logradouro" para um campo de texto em seu formulário.


## Testes

[Descreva a estratégia de teste, incluindo os tipos de teste a serem realizados (unitários, integração, carga, etc.) e as ferramentas a serem utilizadas.]

1. Crie casos de teste para cobrir todos os requisitos funcionais e não funcionais da aplicação.
2. Implemente testes unitários para testar unidades individuais de código, como funções e classes.
3. Realize testes de integração para verificar a interação correta entre os componentes da aplicação.
4. Execute testes de carga para avaliar o desempenho da aplicação sob carga significativa.
5. Utilize ferramentas de teste adequadas, como frameworks de teste e ferramentas de automação de teste, para agilizar o processo de teste.

Casos de Teste:

Verificamos se a API retorna as informações corretas de endereço com base no CEP fornecido.
Testamos se a aplicação lida corretamente com casos de erro, como CEP inválido ou não encontrado.
Testamos a velocidade de resposta da API para garantir que seja rápida o suficiente para uma boa experiência do usuário.

Testes Unitários:
Implementamos testes unitários para as funções ou workflows específicos que interagem com a API ViaCEP. 

Testes de Integração:
Realizamos testes de integração para garantir que a interação entre o Bubble.io e a API ViaCEP esteja ocorrendo corretamente. Isso inclui verificar se os dados retornados pela API estão sendo processados e exibidos corretamente em seu aplicativo.

Ferramentas de Teste:
Utilizamos a propria plataforma e seus recursos.

# Referências

Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.

As referencias principais foram o forum da plataforma bubble.io e tutorias e aulas sobre a plataforma no youtube.
