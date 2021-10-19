# Santander Coders - Módulo 3

Atividade proposta no curso Santander Coders | Web Full-Stack Degree realizado na [Let's Code](https://www.letscode.com.br/). Exercício de fixação em JavaScript referente a Programação Orientada a Objeto.

## The Reading List

_Uma lista de livros orientada a objeto_

### A aplicação

*   Criada uma classe `BookList`
*   Criada outra classe `Book`

*   **BookLists** possuem as seguintes propriedades:
	*   Número de livros marcados como lidos `amountOfReadBooks`
	*   Número de livros marcados como ainda não lidos `amountOfUnreadBooks`
	*   Uma referência ao próximo livro a ser lido (book object) `nextBook`
	*   Uma referência ao livro que está sendo lido no momento (book object) `currentBook`
	*   Uma referência ao último livro que foi lido (book object) `lastBookRead`
	*   Uma array com todos os livros (Books) `allBooks`
*   Cada **Book** possui as seguintes propriedades:
	*   Título `title`
	*   Gênero `genre`
	*   Autor `author`
	*   Livro lido `read` (true or false)
	*   Data de leitura `readDate`, em branco para livros não lidos, e com data de leitura para livros lidos
*   Toda **Booklist** possui os seguintes métodos:
    * .countBooks() _- privado_
      * Conta quantidade de livros lidos e não lidos
  	* .defineNextBook() _- privado_
    	* Determina qual será o próximo a ser lido
  	* .checkIfBookRepeats(book) _- privado_
    	* Verifica se o livro **book** já existe na lista de livros
  	* handleReadBooks(book) _- privado_
    	* Verifica se livro já foi lido e data de leitura e, caso necessário, atualiza o último livro que foi lido
  	* .defineCurrentBook(book) _- privado_
    	* Atualiza livro que está sendo lido no momento
  	* .rearrangeBooks() _- privado_
    	* Remaneja os livros após finalização de um `currentBook`
  	* .addBook(book)
    	* Adiciona o **book** na BookList
  	* .finishCurrentBook()
    	* Marca o `currentBook` como lido e atualiza sua data de leitura `readDate`
    	* Remaneja os livros `lastBookRead`, `currentBook` e `nextBook` chamando o método `.rearrangeBooks()`

### Usando a aplicação