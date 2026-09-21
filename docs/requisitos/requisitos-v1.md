\# Requisitos do Sistema - V1



\## 1. Objetivo



Desenvolver um sistema para controle de estoque e movimentação de móveis,

substituindo o controle realizado atualmente por anotações e conferência física.



O sistema deverá permitir controlar produtos, cores, volumes, localizações,

pedidos, entradas, saídas, reservas, avarias, trocas e movimentações de estoque.



\## 2. Plataformas



O sistema será dividido em três aplicações:



\- Desktop: administração do sistema.

\- Web: utilização pelos funcionários.

\- Mobile: utilização pelos funcionários.



Todas as aplicações utilizarão o mesmo backend e banco de dados.



\## 3. Usuários



Inicialmente o sistema será utilizado por quatro pessoas:



\- Diego

\- Maurilio

\- Paulo

\- Lorran



O sistema utilizará acesso simplificado compartilhado.



Cada movimentação deverá registrar o responsável pela operação.



\## 4. Produtos



Cada produto deverá possuir:



\- Nome

\- Categoria

\- Cor ou acabamento

\- Código/número da cor, quando existir

\- Quantidade de volumes

\- Fornecedor



Exemplo:



Categoria: Rack

Produto: Rack Rubi 2 Portas

Cor: Freijó / Off-White



\## 5. Categorias



Os produtos serão organizados por categorias.



Exemplos:



\- Rack

\- Guarda-roupa

\- Cômoda

\- Cozinha

\- Armário

\- Mesa

\- Cadeira

\- Colchão



Novas categorias poderão ser cadastradas.



\## 6. Cores e acabamentos



As cores deverão ser cadastradas separadamente dos produtos.



Uma cor poderá possuir:



\- Código ou número

\- Nome



Exemplo:



Código: 32

Nome: Freijó / Off-White



O estoque deverá diferenciar produtos de acordo com sua cor/acabamento.



\## 7. Volumes



Produtos que possuem mais de uma caixa deverão ter seus volumes

controlados individualmente.



Exemplo:



Guarda-Roupa X:

\- Volume 1/3

\- Volume 2/3

\- Volume 3/3



Um produto somente deverá ser considerado completo quando todos os

volumes necessários estiverem disponíveis.



\## 8. Fornecedores



Cada fornecedor deverá possuir:



\- Nome da empresa

\- Nome do vendedor

\- CNPJ



Os produtos e pedidos poderão ser relacionados aos seus fornecedores.



\## 9. Pedidos aos fornecedores



Quando um pedido for realizado, deverão ser registrados:



\- Fornecedor

\- Data do pedido

\- Produtos

\- Cores

\- Quantidades

\- Quantidade de volumes



Os produtos pedidos deverão aparecer com o status "Para chegar".



Quando a mercadoria for recebida, a quantidade correspondente deverá

deixar de constar como "Para chegar".



\## 10. Entrada de mercadorias



A entrada deverá permitir registrar:



\- Produto

\- Cor

\- Quantidade

\- Volumes

\- Local de armazenamento

\- Data do recebimento

\- Responsável pelo recebimento

\- Fornecedor



Antes de confirmar a entrada, o funcionário deverá conferir as

quantidades recebidas.



A leitura automática de PDF, DANFE e imagens não fará parte da V1.



\## 11. Localização do estoque



Inicialmente existirão os seguintes locais:



\- Loja

\- Casa

\- Casa do Paulo



Novos locais poderão ser cadastrados posteriormente.



O mesmo produto poderá possuir unidades armazenadas em locais diferentes.



\## 12. Consulta de estoque



O sistema deverá permitir pesquisar produtos por:



\- Nome

\- Categoria

\- Cor

\- Fornecedor

\- Localização



Ao pesquisar um produto e uma cor, deverão ser apresentadas informações como:



\- Quantidade disponível

\- Quantidade para chegar

\- Quantidade reservada

\- Quantidade avariada

\- Quantidade aguardando troca

\- Localização das unidades

\- Situação dos volumes



\## 13. Reserva



Quando um produto for vendido, mas ainda não tiver sido retirado para

montagem ou entrega, deverá ficar como "Reservado".



Produtos reservados não deverão ser considerados disponíveis para uma nova venda.



\## 14. Saída



A saída deverá registrar:



\- Produto

\- Cor

\- Quantidade

\- Local de origem

\- Motivo

\- Data

\- Responsável



Exemplos de motivo:



\- Venda

\- Entrega

\- Troca

\- Ajuste



\## 15. Transferência



O sistema deverá permitir transferir mercadorias entre locais.



Exemplo:



Loja -> Casa do Paulo



A transferência não deverá alterar a quantidade total do estoque,

apenas sua localização.



\## 16. Avarias



Produtos avariados deverão ser identificados separadamente dos produtos disponíveis.



Situações previstas:



\- Avariado

\- Troca solicitada

\- Aguardando troca

\- Substituído



O sistema deverá permitir registrar observações sobre a avaria.



\## 17. Ajuste de estoque



Será possível realizar ajustes manuais quando houver diferença entre

o estoque físico e o estoque registrado no sistema.



Todo ajuste deverá possuir:



\- Quantidade ajustada

\- Motivo

\- Data

\- Responsável



O ajuste deverá permanecer registrado no histórico.



\## 18. Histórico de movimentações



O sistema deverá manter histórico das operações realizadas.



Exemplos:



\- Entrada

\- Saída

\- Reserva

\- Transferência

\- Avaria

\- Troca

\- Ajuste de estoque



O histórico deverá registrar data, operação e responsável.



\## 19. Dashboard



A aplicação Desktop deverá apresentar uma visão simples contendo:



\- Produtos disponíveis

\- Produtos para chegar

\- Produtos reservados

\- Produtos avariados

\- Produtos aguardando troca

\- Últimas movimentações



\## 20. Funcionalidades futuras



Não fazem parte da V1:



\- Leitura automática de DANFE

\- Importação automática de PDF

\- Reconhecimento de pedidos por imagem

\- Cadastro de clientes

\- Sistema completo de vendas

\- Controle de entregas

\- Controle de montagem

\- Relatórios avançados



Essas funcionalidades poderão ser implementadas em versões futuras.



\## 21. Tecnologias planejadas



\- C#

\- .NET

\- ASP.NET Core Web API

\- Entity Framework Core

\- SQL Server

\- WPF

\- Blazor

\- .NET MAUI

\- Git

\- GitHub

