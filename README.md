# Olá, Web Academy: primeiro projeto com Git

> Página HTML "Olá Mundo!" criada em pequenos commits para praticar o fluxo básico do Git.

**Contexto:** IFAC · Técnico em Informática para Internet (TIPI) · Web Academy · 2023

## Sobre

Primeiro repositório feito na Web Academy, em agosto de 2023. O conteúdo é só uma página de apresentação com fundo azul-claro; o que importa aqui é o histórico. Cada mudança virou um commit numerado (v1 a v6) para praticar `git add`, `git commit`, `git push` e a leitura do histórico, incluindo adicionar e depois remover um arquivo binário.

## Funcionalidades

- Página `index.html` com o título "Olá Mundo!" e um parágrafo de apresentação.
- Estilo em `bluestyle.css`: fundo azul-claro e título azul-marinho com recuo à esquerda.
- Histórico de commits que mostra, passo a passo, a criação e a alteração dos arquivos.

### O que cada commit pratica

| Commit | Mensagem | O que mudou |
|---|---|---|
| `134dd38` | Initial commit | Criação do repositório com `LICENSE` e `.gitattributes`. |
| `2f34ae1` | v1 - Readme | Primeiro `Readme.md`. |
| `abcb598` | v2 - Index | Criação do `index.html` ("Hello world!"). |
| `1f524d8` | v3 - Deixando a página mais bonita | Título em português, `<h1>` e criação do `bluestyle.css`. |
| `e1f488c` | v4 - Index com nova linha | Novo parágrafo na página. |
| `db14513` | v5 - Adicionei a imagem | Adiciona `imagem.png`. |
| `0a0ae06` | v6 - Deletei a imagem | Remove `imagem.png` (o arquivo continua acessível no histórico). |

## Tecnologias

- Git e GitHub
- HTML5
- CSS3

## Estrutura do projeto

| Caminho | Descrição |
|---|---|
| `index.html` | Página "Olá Mundo!". |
| `bluestyle.css` | Estilos da página. |
| `.gitattributes` | Normalização automática de fim de linha. |

## Como rodar

### Pré-requisitos

- Git
- Um navegador

### Passo a passo

```bash
git clone https://github.com/itskelme/ifac-tipi-webacademy-ola.git
cd ifac-tipi-webacademy-ola
```

Abra o `index.html` no navegador (duplo clique no arquivo já funciona; não precisa de servidor).

## Como usar

Para estudar o histórico, que é o objetivo do projeto:

```bash
# lista os commits, do mais recente ao mais antigo
git log --oneline

# mostra o que mudou em um commit específico
git show 1f524d8

# volta temporariamente ao estado da v5, quando a imagem existia
git switch --detach db14513
git switch main
```

## Observações

- No commit v4 a tag `<link rel="stylesheet" href="bluestyle.css"` perdeu o `>` de fechamento. O navegador costuma tolerar o erro e ainda carregar o CSS, mas o certo é fechar a tag.

## Referências

- [Pro Git (em português)](https://git-scm.com/book/pt-br/v2), capítulo 2: Fundamentos do Git
- [Documentação do `git log`](https://git-scm.com/docs/git-log) e do [`git show`](https://git-scm.com/docs/git-show)
- [GitHub Docs: sobre repositórios](https://docs.github.com/pt/repositories/creating-and-managing-repositories/about-repositories)
- [MDN: elemento `<link>`](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/link)

## Autores

- Diego Kelme Santos da Silva — [@itskelme](https://github.com/itskelme)

## Licença

Este projeto está sob a licença [CC BY-NC 4.0](LICENSE): uso pessoal e modificação permitidos com atribuição; uso comercial proibido.
