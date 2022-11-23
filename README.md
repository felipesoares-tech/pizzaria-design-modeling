# Modelagem de Banco de Dados 💻

## Versão 4.0

### Sumário

<a href="#1-informações-do-projeto" style="color:#fff;"><h2>1 INFORMAÇÕES DO PROJETO</h2></a>

        1.1 Propósito do Documento

        1.2 Perspectiva do Sistema

**2 DESCRIÇÃO DO CONTEXTO**

        2.1 Funcionalidades
        2.2 Modelo de Entidade e Relacionamento
        2.3 Modelo Relacional
        2.4 Requisistos Não Funcionais
        2.4.1 Requisitos de Software
        2.4.2 Requisitos de Ambiente
        2.4.3 Regras de Negócio

**3 DESENVOLVIMENTO**

        3.1 Diagrama de Entidade e Relacionamento

**4 CONSIDERAÇÕES FINAIS**


## **1 INFORMAÇÕES DO PROJETO**

DESENVOLVEDOR: Felipe Soares Santana.

PROJETO: Projeto Disk Pizzas.

EMPRESA: Disk Pizzas.

DESCRIÇÃO PROJETO: Desenvolvimento de um banco de dados para um sistema de
vendas de pizza.

### **1.1 Propósito do Documento**

>Apresentar as análises realizadas, construção e resultados para a construção do Banco de Dados para a solução Projeto Disk Pizzas que será desenvolvido pelo estudante Felipe Soares Santana para a empresa Disk Pizzas, exibindo as funcionalidades do produto, formas e métodos de interação com outros sistemas existentes, especificações técnicas e outras características necessárias para orientar o desenvolvimento do produto.

### **1.2 Perspectiva do Sistema**

>Identificamos a necessidade de implementar um banco de dados de maneira que seja possível que todas as informações referente aos clientes, atendentes e estoque, fiquem devidamente organizadas e de fácil acesso. A metodologia atualmente utilizada pela pizzaria acaba sendo um tanto quanto ineficaz. Atualmente é muito complicado consultar alguma venda, ou obter algum tipo de relatório, visto que não existe um sistema que facilite esse tipo de transação. Com a implantação de um SGBD esperamos resolver todos os problemas citados acima, para que assim possamos ter uma base de dados sólida e eficiente.

## **2 DESCRIÇÃO DO CONTEXTO**

>Atualmente o Disk Pizzas funciona sem a utilização de um banco de dados, onde todos os dados vêm sendo registrados em planilhas, porém tal método acaba sendo muito cansativo e ineficaz visto que em alguns momentos é muito complicado a manipulação destes dados, além de não ser um método que possa garantir a integridade destes e de não previnir erros que possam eventualmente ser cometidos pelos atendentes em razão de uma demanda muito grande de atendimentos. Sendo assim, iremos implementar um SI que seja capaz de gerenciar todos os pedidos, estoque, usuários, sabores, bebidas etc.. Será implementado diversas funções a fim de facilitar o trabalho dos funcionários, visto que o método atual além de ineficaz, acaba sendo um tanto quanto cansativo. Teremos funcionalidades tais como: Cadastro de usuários, onde será possível cadastrar clientes e atendentes, tal função se torna interessante para manter a organização da empresa, visando ter um login próprio para os funcionários, e quanto aos clientes será interessante no quesito de alguma promoção ou até mesmo para possibilidade de faturamento de vendas. Também teremos o Cadastro de grupos/subgrupos para os produtos, onde será possível cadastrar um determinado grupo para um tipo de produto, afim de facilitar na emissão de relatórios detalhados referente aos mesmos, exemplo: criação de um grupo de Bebidas, e dentro deste grupo de bebidas será possível cadastrar subgrupos tais como: refrigerante, cerveja e suco. Tal funcionalidade irá ajudar bastante na emissão de relatórios e manutenção destes dados. Pois assim será possível listar um grupo ou subgrupo de produtos para realizar algum tipo de manutenção, como exemplo no preço ou no nome e até mesmo desativar um determinado grupo de produto. Teremos também a funcionalidade de desativar determinado produto, tal função irá auxiliar no controle de estoque, onde um produto que não será mais vendido poderá ser desativado e talvez em um momento futuro ser ativado novamente caso volte a ser vendido.

### **2.1 Funcionalidades**

| Funções | Descrição |
| ----------- | ----------- |
| Acessar o sistema | Este caso de uso tem a responsabilidade de iniciar a abertura do sistema validando o nome de usuário e senha, permitindo ou negando acesso ao sistema. |
| Visualizar informações | Função que exibe as informações presentes no sistema. |
| Gerenciar usuários | Esse caso de uso tem a função de cadastrar e incluir usuários do sistema (clientes, atendentes e entregadores). |
| Cadastrar Produtos | Função para cadastrar os diversos tipos de produtos vendidos pela pizzaria, tais como: bebidas, sabores de pizzas, bombonieres etc.. |
| Desativar Produto | Função para desativar produtos que não serão mais vendidos |
| Cadastrar Grupos/SubGrupos | Função que possibilitará o cadastro de grupos e subgrupos para os diversos tipos de produtos. |

### **2.2 Modelo de Entidade e Relacionamento**

>Com base na descrição fornecida pelo cliente, redigida anteriormente neste documento, foi construído um Modelo de Entidade e Relacionamento para auxiliar na abstração dos dados para construção do projeto.