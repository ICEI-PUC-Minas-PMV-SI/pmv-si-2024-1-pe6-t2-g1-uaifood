# APIs e Web Services

O planejamento de uma aplicação de APIS Web é uma etapa fundamental para o sucesso do projeto. Ao planejar adequadamente, você pode evitar muitos problemas e garantir que a sua API seja segura, escalável e eficiente.

Aqui estão algumas etapas importantes que devem ser consideradas no planejamento de uma aplicação de APIS Web.

[Inclua uma breve descrição do projeto.]


Resumo do Projeto: Facilitando o Cadastro de Endereços com a API ViaCEP

Nosso projeto visa simplificar o processo de cadastro de endereços em um aplicativo de entrega de alimentos. Ao integrar a API ViaCEP, os usuários podem inserir apenas o CEP ao preencher seus dados, eliminando a necessidade de digitar manualmente todas as informações do endereço.

Quando um usuário insere o CEP, nossa aplicação faz uma chamada à API ViaCEP para obter automaticamente o nome da rua, o bairro, a cidade e o estado associados a esse CEP. Essas informações são então preenchidas nos campos relevantes do formulário de cadastro.

Isso não apenas simplifica o processo para o usuário, tornando-o mais rápido e conveniente, mas também reduz a probabilidade de erros de digitação. Além disso, a integração com a API ViaCEP garante que os dados de endereço sejam precisos e atualizados, melhorando a eficiência e a confiabilidade do serviço.





## Objetivos da API

O primeiro passo é definir os objetivos da sua API. O que você espera alcançar com ela? Você quer que ela seja usada por clientes externos ou apenas por aplicações internas? Quais são os recursos que a API deve fornecer?

Seu principal propósito é facilitar o desenvolvimento de aplicações web e móveis, oferecendo uma solução fácil de integrar que permite o preenchimento automático de formulários com base no CEP fornecido pelo usuário. Além disso, a API busca garantir a precisão das informações fornecidas, utilizando fontes de dados confiáveis. Ao promover a eficiência operacional e estimular a inovação em diversos setores. Em resumo, a API nossa api visa simplificar e otimizar o acesso a informações de endereço no Brasil, beneficiando os usuarios com essa facilidade.


## Arquitetura


A arquitetura da API ViaCEP é fundamentada nos princípios da arquitetura REST, utilizando comunicação via HTTP, endpoints padronizados e formato de dados estruturado. A comunicação entre clientes e servidor ocorre por meio de solicitações HTTP, seguindo um modelo Cliente-Servidor. A API é stateless e escalável, garantindo eficiência no processamento de um grande volume de solicitações sem comprometer o desempenho. Como estamos utilizando a plataforma bubble.io que possibilita a total integração com a api.

## Modelagem da Aplicação
[Descreva a modelagem da aplicação, incluindo a estrutura de dados, diagramas de classes ou entidades, e outras representações visuais relevantes.]


A modelagem de dados estrela é uma abordagem utilizada em data warehousing, onde os dados são organizados em torno de uma tabela central, chamada de tabela fato, e tabelas secundárias, chamadas de tabelas de dimensão. Na tabela fato, são armazenados os fatos ou medidas centrais do negócio, como vendas ou transações, enquanto as tabelas de dimensão representam diferentes perspectivas dos dados, como tempo, produto ou localização. As chaves estrangeiras na tabela fato estabelecem relacionamentos com as chaves primárias das tabelas de dimensão, permitindo análises multidimensionais. Essa estrutura em forma de estrela simplifica consultas analíticas complexas e facilita a compreensão e a análise dos dados de negócio.



![Db UaiFood](https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-1-pe6-t2-g1-uaifood/assets/89950016/eba71e07-1ee9-4def-b913-5ff5a8157b31)



## Fluxo de Dados

[Diagrama ou descrição do fluxo de dados na aplicação.]

## Requisitos Funcionais

[Liste os principais requisitos funcionais da aplicação.]

## Requisitos Não Funcionais

[Liste os principais requisitos não funcionais da aplicação, como desempenho, segurança, escalabilidade, etc.]

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
