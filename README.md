# Sistema de Registro de Produtos

Este projeto é um sistema simples de **CRUD (Create, Read, Update, Delete)** de produtos, desenvolvido em **JavaScript** para ser executado no **console** do navegador. O objetivo é gerenciar produtos, permitindo adicionar, listar, editar, deletar e filtrar produtos. Cada produto é tratado como um objeto, utilizando o conceito de **classes** em JavaScript.

## Funcionalidades

1. **Listar Produtos**: Exibe a lista de todos os produtos cadastrados.
2. **Adicionar Produto**: Permite adicionar um novo produto, especificando o nome e o preço.
3. **Editar Produto**: Atualiza o preço de um produto já existente.
4. **Deletar Produto**: Remove um produto da lista de produtos cadastrados.
5. **Filtrar Produto**: Filtra produtos pelo nome (ou parte do nome) e exibe os resultados.

## Estrutura do Produto

Cada produto é uma instância da classe `Produto`, que contém:

- **nome**: O nome do produto.
- **preco**: O preço do produto.

### Classe Produto

```javascript
class Produto {
    constructor(nome, preco) {
        this.nome = nome;
        this.preco = preco;
    }

    // Exibe as informações do produto
    info() {
        return `${this.nome}: R$ ${this.preco}`;
    }

    // Define o novo preço do produto
    setPreco(novoPreco) {
        this.preco = novoPreco;
    }
}
