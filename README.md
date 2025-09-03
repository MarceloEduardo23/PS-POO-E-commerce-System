# Sistema de E-Commerce Simples (Console)

## ✨ Funcionalidades

O sistema possui dois tipos de usuários (Cliente e Administrador), cada um com seu conjunto de funcionalidades.

#### Para Clientes:
- **Autenticação:** Cadastro e Login de usuários.
- **Catálogo de Produtos:** Visualizar produtos, com opções de busca e ordenação (preço e nome).
- **Detalhes do Produto:** Ver informações detalhadas, incluindo reviews de outros clientes.
- **Carrinho de Compras:** Adicionar, remover e visualizar itens no carrinho.
- **Checkout:**
    - Aplicar cupons de desconto (percentuais e fixos).
    - Selecionar endereço de entrega.
    - Simulação de pagamento.
- **Histórico de Pedidos:** Visualizar todos os pedidos já realizados.
- **Avaliações:** Deixar avaliações (nota e comentário) para produtos comprados.
- **Gerenciamento de Perfil:** Alterar senha e gerenciar endereços.
- **Suporte ao Cliente:** Abrir e acompanhar tickets de suporte.

#### Para Administradores:
- Todas as funcionalidades de cliente.
- **Gerenciamento de Produtos:** Adicionar, editar e remover produtos do catálogo.
- **Gerenciamento de Cupons:** Criar, listar e ativar/desativar cupons de desconto.
- **Atendimento ao Cliente:** Visualizar e responder tickets de suporte abertos pelos clientes.

## 🚀 Conceitos de POO Demonstrados

- **Herança:** A estrutura de usuários é um exemplo direto, com as classes `Customer` e `Admin` herdando da classe base `User`. O mesmo ocorre com os cupons (`PercentageCoupon` e `FixedCoupon` herdando de `Coupon`).
- **Polimorfismo:** Implementado de forma clara no sistema de cupons. O método `apply_discount` é chamado da mesma forma, mas se comporta de maneira diferente dependendo se o objeto é um `PercentageCoupon` ou `FixedCoupon`.
- **Encapsulamento:** Os dados e os métodos que os manipulam estão agrupados dentro de classes (`Cart`, `Order`, `Product`), escondendo a complexidade interna.
- **Abstração:** As classes modelam entidades do mundo real (Produto, Pedido, Usuário) de forma simplificada, focando apenas nos atributos e comportamentos relevantes para o sistema.

## 🛠️ Tecnologias Utilizadas

- **Python 3:** O projeto foi desenvolvido inteiramente em Python.
- **Bibliotecas Padrão:** Utiliza apenas bibliotecas nativas do Python, como `os`, `time` e `random`. Não requer instalação de pacotes externos.

## 🔑 Dados de Acesso

O sistema já vem com dois usuários pré-cadastrados para facilitar os testes:

#### 👤 Administrador
- **Login:** `admin`
- **Senha:** `1234`

#### 👤 Cliente
- **Login:** `customer`
- **Senha:** `123`
- Este cliente já possui um endereço cadastrado para agilizar o teste de checkout.
