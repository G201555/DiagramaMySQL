# DiagramaMySQL

Sistema de Gestão de Vendas de Quadrinhos
Este projeto é um sistema de gestão para uma empresa de quadrinhos que permite o gerenciamento de clientes, pedidos, formas de pagamento, entregas e produtos (quadrinhos). O sistema permite um controle detalhado sobre as compras realizadas, o status das entregas e a forma como os clientes pagam pelas suas aquisições.

Funcionalidades
Cadastro de Clientes:

Clientes podem ser cadastrados como Pessoa Física (PF) ou Pessoa Jurídica (PJ).
Um cliente pode ter múltiplas formas de pagamento cadastradas.
Gestão de Formas de Pagamento:

O sistema permite que cada cliente registre mais de uma forma de pagamento (cartão de crédito, boleto bancário, etc.).
Pedidos:

Cada pedido é associado a um cliente e pode incluir múltiplos produtos (quadrinhos).
O status do pedido pode ser alterado para acompanhar o progresso (Em Processamento, Enviado, Finalizado).
Entregas:

O sistema rastreia as entregas, permitindo o acompanhamento através de um código de rastreio.
O status da entrega pode ser atualizado conforme o andamento (Pendente, Enviado, Entregue).
Cadastro de Quadrinhos:

Cada quadrinho possui informações como título, autor e preço.
Quadrinhos podem ser associados aos pedidos realizados pelos clientes.
Estrutura do Banco de Dados
O banco de dados é composto pelas seguintes tabelas:

Clientes:

Armazena as informações dos clientes, como nome, tipo de cliente (PF ou PJ) e contato.
Formas de Pagamento:

Armazena as formas de pagamento possíveis que podem ser associadas aos clientes.
Clientes_Formas_de_Pagamento:

Tabela de relacionamento entre clientes e formas de pagamento (múltiplas formas por cliente).
Pedidos:

Armazena as informações sobre cada pedido realizado, como cliente associado, status e total.
Entregas:

Armazena os dados de entrega de cada pedido, incluindo status e código de rastreio.
Quadrinhos:

Armazena as informações dos quadrinhos disponíveis para venda (título, autor, preço).
Pedidos_Quadrinhos:

Tabela de relacionamento entre pedidos e quadrinhos, indicando quais quadrinhos foram comprados em cada pedido.
Tecnologias Utilizadas
MySQL: Banco de dados relacional para gerenciamento de dados.
MySQL Workbench: Ferramenta utilizada para modelagem de banco de dados.
