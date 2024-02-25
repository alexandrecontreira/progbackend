# Introdução ao Markdown com os Alunos
## O que é Markdown?
Segundo a Wikipedia : 
 > Markdown é uma linguagem de marcação leve com sintaxe de formatação de texto simples projetada para que ela possa ser convertida em HTML e muitos outros formatos usando uma ferramenta com o mesmo nome. Markdown é usado frequentemente para formatar arquivos readme, para escrever mensagens em fóruns de discussão on-line e para criar texto rico usando um editor de texto simples.

## Porque usar?

- FÁCIL : A sintaxe é tão fácil que você pode aprender em um minuto ou dois, em seguida, escreva sem perceber nada estranho ou nerd.
* RÁPIDO : Ele economiza tempo em comparação com outros tipos de arquivos / formatos de texto. Isso ajuda a aumentar a produtividade e os fluxos de trabalho do escritor.
+ LIMPO : Tanto a sintaxe como a saída são limpas, sem confusão com nossos olhos e simples de gerenciar.
FLEXÍVEL : Com apenas algumas configurações, o seu texto será traduzido atravessando qualquer plataforma lá fora, editável em qualquer software de edição de texto e conversível para uma ampla variedade de formatos.


Em resumo, os usuários comuns acharão útil em todos os casos, especialmente quando você precisar de algo melhor que o texto simples, mas menos funcional do que o Microsoft Word.
Para desenvolvedores, Se você é preguiçoso para escrever código HTML, você vai adorar o markdown. Além disso, Github e muitos sites favorecem o markdown para o arquivo readme de projetos. Isso significa que você vai encontrar o markdown em sua vida de uma forma ou de outra.

## Inserindo um bloco de código 

Para inserir um bloco de código usamos o sinal de crase ( ` ) três vezes.

**Exemplo estrutura do codigo HTML**
```
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```
## Lista de tarefas
- [X] Aprender a sintaxe Markdown
- [ ] Aprender Github
- [ ] Aprender Gitbash

## Usar emojis
É possível adicionar um emoji à escrita digitando :EMOJICODE:, dois pontos e, em seguida, o nome do emoji.

@octocat :+1: This PR looks great - it's ready to merge! :shipit:

Captura de tela do GitHub Markdown renderizado mostrando como os códigos de emoji para +1 e shipit são renderizados visualmente como emojis.

Se você digitar :, uma lista de emojis sugeridos será exibida. A lista será filtrada à medida que você digitar algo. Portanto, assim que encontrar o emoji que estava procurando, pressione Tab ou ENTER para completar o resultado realçado.

Para obter uma lista completa de emojis e códigos disponíveis, confira Emoji-Cheat-Sheet.


 * Os vídeos do Youtube requerem algum trabalho adicional. 
  ```
  Eles não podem ser adicionados diretamente, mas você pode adicionar uma imagem com um link para o vídeo como este:
  <a href="http://www.youtube.com/watch?feature=player_embedded&v=YOUTUBE_VIDEO_ID_HERE
  " target="_blank"><img src="http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg" 
  alt="Texto ALT da imagem aqui" width="240" height="180" border="10" /></a>
  ````
* Usando a sintaxe do bloco de código diff para gerar texto colorido. Ainda existem algumas limitações como não conseguir estilizar o texto dentro da caixa diff e poucas cores para a formatação. Isso pode ser aplicável quando você deseja destacar alguma nota ou mostrar a diferença entre dois blocos de código

## Deixar o texto colorido 
>  Usando a sintaxe do bloco de código diff para gerar texto colorido. Ainda existem algumas limitações como não conseguir estilizar o texto dentro da caixa diff e poucas cores para a formatação. Isso pode ser aplicável quando você deseja destacar alguma nota ou mostrar a diferença entre dois blocos de código

```diff
- texto em vermelho
+ texto em verde
! texto em laranja
# texto em cinza
@@ texto em roxo (e negrito)@@
```
## Alertas

Alertas são uma extensão Markdown baseada na sintaxe blockquote que você pode usar para enfatizar informações críticas. Em GitHub, eles são exibidos com cores e ícones distintos para indicar a importância do conteúdo.

Use alertas apenas quando eles forem cruciais para o sucesso do usuário e limite-os a um ou dois por artigo para evitar sobrecarregar o leitor. Além disso, você deve evitar colocar alertas consecutivamente. Os alertas não podem ser aninhados em outros elementos.

Para adicionar um alerta, use uma linha de citação especial especificando o tipo de alerta, seguida pelas informações do alerta em uma citação padrão. Cinco tipos de alertas estão disponíveis:

> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.

## Usando imagens e links

Você pode criar alguns recursos coloridos no momento da renderização. Badges como este são exemplos típicos que você pode encontrar em todo o Github:
- Java - [![Java](https://img.shields.io/badge/Java-%23FFac45.svg?&style=for-the-badge&logo=java&logoColor=white&color=yellow)](https://github.com/)
- HTML - [![HTML](https://img.shields.io/badge/HTML-%23FFac45.svg?&style=for-the-badge&logo=html5&logoColor=white&color=orange)](https://github.com/)
- CSS - [![CSS](https://img.shields.io/badge/CSS-%23FFac45.svg?&style=for-the-badge&logo=css3&logoColor=white&color=blue)](https://github.com/)
- JavaScript - [![JavaScript](https://img.shields.io/badge/JAVASCRIPT-%23FFac45.svg?&style=for-the-badge&logo=javascript&logoColor=white&color=yellow)](https://github.com/) 
- Linkedin - [![Linkedin](https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/)
- Github - [![Github](http://img.shields.io/badge/github-%231877F2.svg?&style=for-the-badge&logo=github&logoColor=white&color=black)](https://github.com/)
- Phyton <img src="https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue"/>

( get some badges [here](https://github.com/Ileriayo/markdown-badges) )

## Trechos de código

![image](https://github.com/alexandrecontreira/progbackend/assets/77118607/693f16ab-5497-42ef-b38e-cc6e0209e91b)


``js example-good
const greeting = "Sou um bom exemplo";
``

`js example-bad
const greeting ="Eu sou um mau exemplo";
`
## Código (Code Highlight)
Há dois modos de adicionar trechos de código ao Markdown:

Código em linha (inline): adicione um acento grave ˋ no início e no final do código.
Múltiplas linhas de código: envolva as linhas de código com três acentos graves ˋˋˋ ou três tils ~~~.

~~~javascript
Esta é uma linha de código em Javascript.
~~~~
~~~php
Esta é uma linha de código em PHP.
~~~~
~~~html
Esta é uma linha de código em HTML.
~~~


## Referências

https://github.com/luong-komorebi/Markdown-Tutorial/blob/master/README_pt-BR.md

https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

https://developer.mozilla.org/pt-BR/docs/MDN/Writing_guidelines/Howto/Markdown_in_MDN#blocos_de_c%C3%B3digo_de_exemplo

https://github.com/luong-komorebi/Markdown-Tutorial/blob/master/README_pt-BR.md
