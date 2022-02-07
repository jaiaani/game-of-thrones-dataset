![got](./imgs/gotLogo.jpg)

##                              Projeto de final de Módulo 

### Resilia, 3º módulo 

#### Game of Thrones Dataset

Esse projeto utiliza dados sobre a série de televisão Game Of Thrones disponibilizados em .CSV afim de retirar informações relevantes a respeito da série. 

No total, são 3 tabelas que nos fornecem os seguintes dados:



* Personagens 

  * Nome do personagem
  * Nome do Ator 
  * Quantidade de episódios que apareceu
  * Primeira aparição
  * Ultima aparição

  Exemplo: 

  | Nome               | Nome do Ator   | Aparições | Primeira Aparição | Última aparição |
  | ------------------ | -------------- | --------- | ----------------- | --------------- |
  | Tyrion Lannister   | Peter Dinklage | 67        | 2011              | 2019            |
  | Cersei Lannister   | Lena Headey    | 62        | 2011              | 2019            |
  | Daenerys Targaryen | Emilia Clarke  | 62        | 2011              | 2019            |

  

* Episódios    

  * Temporada
  * Episódio(1, 2 , 3...)
  * Título do episódio
  * Data de Lançamento
  * Nota
  * Votos
  * Sumário
  * Escritor 1
  * Escritor 2
  * Principal 1
  * Principal 2
  * Principal 3
  * Avaliações dos Telespectadores
  * Avaliação de críticos
  * Visualizações
  * Duração
  * Diretor

Exemplo: 

| Temporada | Episódios | Título              | Data Lançamento | Notas | Votos |
| --------- | --------- | ------------------- | --------------- | ----- | ----- |
| 1         | 1         | Winter is Coming    | 17-Apr-11       | 9.1   | 38639 |
| 2         | 1         | The North Remembers | 1-Apr-12        | 8.8   | 24837 |
| 3         | 1         | Valar Dohaeris      | 31-Mar-13       | 8.8   | 24808 |



* Casas 
  * Nome
  * Região

Exemplo: 

| Nome                  | Região      |
| --------------------- | ----------- |
| Algood                | Westerlands |
| Allyrion of Godsgrace | Dorne       |



### Diagrama 

Nós utilizamos o site [dbdiagram]([dbdiagram.io - Database Relationship Diagrams Design Tool](https://dbdiagram.io/home)) para criarmos uma visualização mais simples e relacional com os dados. Ao observarmos as tabelas de Game Of Thrones, não conseguimos estabelecer muitos relacionamentos (Chaves estrangeiras) entre elas. Somente observamos que poderia ser interessante relacionarmos o nome do Ator contido na tabela `personagens` com o nome dos atores principais contidos na tabela `episodios`