<h1>Projeto Farmácia</h1>

## Diagrama de Classes

```mermaid
classDiagram
class Categoria {
  - id : Long
  - nome : String
  - descricao : String
  - produto : List ~Produto~
  + getAll()
  + getById(Long id)
  + getByTipo(String tipo)
  + post(Categoria categoria)
  + put(Categoria categoria)
  + delete(Long id)
}
class Produto {
  - id : Long
  - nome : String
  - descricao: String
  - quantidade: int
  - laboratorio: String
  - preco: BigDecimal
  - foto: String
  - categoria: Categoria
  + getAll()
  + getById(Long id)
  + getByNome(String nome)
  + post(Produto produto)
  + put(Produto produto)
  + delete(Long id)
}
Categoria --> Produto
```


<h2>Etapas:</h2>


- [x] Criar o Projeto Spring
- [x] Configurar as Dependências do Projeto
- [x] Configurar o Banco de dados
- [x] Criar a Camada Model
- [x] Criar a Camada Repository
- [x] Criar a Camada Controller
- [x] Criar o Relacionamento entre as 2 classes

