# Templates LaTeX

Sei que não precisa me referenciar para usar os templates.  
Mas dá uma força: compartilha com seus amigos e ajuda a divulgar o que foi feito aqui.

Eu utilizo o VSCode para acelerar o processo de escrita em LaTeX, mas estou aprendendo Neovim.  
Em breve, pretendo criar um repositório com meus snippets para `.tex` que uso no VSCode, antes de migrar 100% para o Neovim.

---

## Aviso Importante
> **Compile sempre com `lualatex`**  
> Esses templates foram pensados para serem usados com LuaLaTeX, garantindo suporte a fontes modernas, pacotes de idiomas e maior compatibilidade com Unicode.  
> Em outros compiladores (como `pdflatex`), alguns recursos podem não funcionar corretamente.

---

## Templates Disponíveis

### Template 1 — Notas de aula
Seguindo boas práticas para organização de código, o template é dividido em 3 pastas principais:

- **`elementos/`**: imagens, arquivos PDF ou qualquer outro recurso externo que será incluído no texto.  
- **`preambulo/`**: onde ficam os pacotes carregados e as definições de estilo/configuração do documento.  
- **`aulas/`**: contém a capa do arquivo e o texto inicial (`aula_1.tex`).  

### Como utilizar?
1. Na capa, troque a imagem por um logo da sua instituição ou outro de sua preferência.  
2. Substitua as partes com os nomes e informações pessoais.  
3. No arquivo `aula_1.tex`, você pode apagar o conteúdo exemplo e começar diretamente pelo seu:   \section{Título da Aula}
4. Crie novos arquivos de aula.tex conforme a matéria for avançando
5. Compile o arquivo `notas_aula.tex` e adicone \input{aulas/nome_da_aula} sempre que criar uma nova aula. Compilando esse arquivo e salvando as alterações nos outros arquivos, seu PDF será atualizado.

### Template 2 - Apresentação em slides
Seguindo boas práticas para organização de código, o template é dividido em 3 pastas principais:

- **`elementos/`**: imagens para incluir nos slides (inclusive a logo da instituição)
- **`preambulo/`**: onde estão os pacotes carregados, o estilo dos slides e o cabeçalho da apresentação
- **`capitulos/`**: onde você define as partes da sua apresentação. Por *default* está dividido em: Introdução, Desenvolvimento e Conclusão.

### Como utilizar?
1. No texto `estilo.tex` do preâmbulo, troque a foto pelo logo da sua instituição ou outro de sua preferência. 
2. Recomendo também, ainda em `estilo.tex` que pegue a paleta de cores da sua instituição e altere as cores principais do slide para melhor adaptar. Existem sites em que você pode identificar o código RGB das cores da instituição para fazer a devida alteração.
3. Nos capítulos, basta adicionar frames, sections, subsections, etc. dentro do respectivo arquivo `.tex`.
4. Caso não queira usar a estrutura *default*, altere no texto principal o \input{} para corresponder aos novos arquivos.

## Próximos templates
Os demais templates serão adicionados em futuros commits deste repositório.

Espero que você aproveite o conteúdo disponível aqui.
Qualquer sugestão, melhoria ou correção é sempre bem-vinda! Entre em contato com o email: puro0550.dev@gmail.com

