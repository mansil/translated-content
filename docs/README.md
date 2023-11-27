# Diretrizes gerais para o conteudo traduzido de MDN

Neste README pode encontrar uma coleção de diretrizes gerais para traduzir
o conteúdo de MDN, que se aplicam a todos os idiomas.

Para diretrizes relacionadas com idiomas específicos, nós temos documentos
específicos de idiomas nas subdiretorias:

- [Guia de tradução de russo / Участие в переводе](ru/translation-guide.md)
- [Guia de chinês simplificado / 简体中文翻译指南](zh-cn/translation-guide.md)
- [Guia de chinês tradicional / 正體中文翻譯指南](zh-tw/translation-guide.md)
- [Guia em espanhol / Guía en español](es/README.md)

Se quiser adicionar um guia para documentar algumas diretrizes específicas para o seu idioma
e este ainda não aparece aqui, pode adicionar um, ou
[falar com as equipas de tradução](https://github.com/mdn/translated-content/blob/main/PEERS_GUIDELINES.md#review-teams)
sobre o mesmo. Da mesma forma, se conseguir pensar numa boa diretriz geral que
gostaria de adicionar aqui, fique à vontade para criar um problema para falar sobre isso.

## Traduzir Ids. de Cabeçalho

Os nossos títulos de artigos quase sempre recebem Ids., para que nós possamos gerar
automaticamente a navegação no artigo, identificar os blocos de código para criar 
amostras ao vivo, e outras razões também. Ao traduzir os títulos, não precisa de traduzir
a ID também; o resto da ''slug'' não é traduzida, então isto mantém tudo consistente.

Por exemplo:

```html
<h2 id="tutorials">Tutoriais</h2>
```

no idioma `fr` (francês) seria

```html
<h2 id="tutorials">Tutoriels</h2>
```

Nós geralmente aconselhamos que escreva todas as Ids. em letras minúsculas. A plataforma
converte-as automaticamente no momento da renderização de qualquer maneira, mas mantendo-as
em letras minúsculas significa que há menos chance de uma hiperligação âncora criada manualmente
não funcionar por causa da conversão.

## Traduzir blocos de código

Ao traduzir os blocos de código, não há problema em traduzir os comentários, entradas,
nomes de variáveis ​​e representações de saída.

Contudo, não traduza os termos do código atual, tal como, sintaxe. O exemplo precisa
de ainda funcionar depois de terminar.

Também, quando considerar a tradução dos exemplos, tenha em mente que alguns exemplos
irão vincular a uma versão ativa ou código-fonte num repositório separado. Também pode
desejar considerar a criação de uma versão traduzida dos exemplos de código externos
para vincular a partir da sua página traduzida.

## Quebras de linha na fonte HTML

Em algun código-fonte dos artigos, pode encontrar quebras de linha no nível do bloco
de elementos que não são estritamente necessários, por exemplo:

```html
<p>O
  método <strong><code>HTMLCanvasElement.transferControlToOffscreen()</code></strong>
  transfere o controle para um objeto {{domxref("OffscreenCanvas")}}, quer seja no
  ''thread'' principal ou num trabalhador.</p>

<pre
  class="brush: js">OffscreenCanvas HTMLCanvasElement.transferControlToOffscreen()</pre>
```

Geralmente nós não utilizamos as quebras de linha como esta no nosso código-fonte, então
fique `avontade para removê-las se desejar e não as adicione quando criar novas traduções.
No entanto, não perca muito tempo tentando removê-las, pois
eles não fazem nenhuma diferença no resultado final renderizado.
