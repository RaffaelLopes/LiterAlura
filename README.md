# Literalura

Descrição

Tem como objetivo facilitar a busca e o acesso a livros disponíveis na API pública Gutendex, oferecendo funcionalidades para visualizar, baixar e ouvir audiolivros, além de gerenciar favoritos e filtros personalizados.

Funcionalidades principais
Busca de livros na API Gutendex com filtros avançados.

Visualização detalhada dos livros, incluindo diversos formatos disponíveis (texto, áudio, etc).

Download, leitura online e audição de audiolivros diretamente pela aplicação.

Consultas assíncronas para respostas rápidas da API.

Navegação por todas as mais de 2.000 páginas de conteúdo da API.

Possibilidade de excluir livros para que não apareçam mais nas buscas.

Salvar livros favoritos para acesso rápido.

Modelo de Dados (Entidades e Relacionamentos)
Livro
id: Identificador único do livro.

titulo: Título do livro.

quantidadeDescargas: Número de downloads do livro.

tipoDeMedio: Tipo do meio (ex: texto, áudio).

autores: Lista de autores (relação muitos-para-muitos com a entidade Autor).

linguagem: Idioma do livro.

categoria: Categoria literária do livro.

formatos: Lista de formatos disponíveis (ex: leitura online, PDF, ePub, audiolivro).

imagem: URL da capa do livro.

estado: Indica se o livro está ativo ou oculto para exclusão visual.

Autor
id: Identificador único do autor.

nome: Nome completo do autor.

anoNasc: Ano de nascimento.

anoMorte: Ano de falecimento (se aplicável).

biografia: Link para a biografia do autor na Wikipedia.

Relação entre Livro e Autor:
A relação é muitos-para-muitos, pois um livro pode ter vários autores e um autor pode ter escrito vários livros. Isso é gerenciado por uma tabela intermediária autor_livro.

Tecnologias utilizadas
PostgreSQL

Java

Spring Boot

Thymeleaf

HTML & CSS

Como usar
Clone este repositório:

bash
Copiar
Editar
git clone https://github.com/seuusuario/Literalura.git
Abra o projeto na sua IDE favorita.

Configure as credenciais e propriedades da API Gutendex no arquivo application.properties ou application.yml.

Execute a aplicação.

Explore as funcionalidades de busca, visualização e gerenciamento de livros.


