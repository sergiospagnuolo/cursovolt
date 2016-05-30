#### VOLT DATA LAB | Outubro 2015

Este é um tutorial ridiculamente detalhado, ainda em fase beta, para publicação simples no GitHub Pages, escrito por [@ProjetoStock][0], com base no curso de programação web básica para jornalistas oferecido pelo Volt Data Lab. Use-o como quiser, se possível com os devidos créditos.

* Site: [www.voltdata.info][1]
* GitHub: [https://github.com/voltdatalab][2]
* Twitter: [@voltmediabr][3]
* Facebook: [www.facebook.com/voltdata][4]


Nesse tutorial, veremos como publicar páginas na Internet utilizando apenas a interface web do GitHub, sem utilizar Git nem outros aplicativos. É um processo pouco óbvio ou intuitivo, mas muito simples. Esse método exige bastante uso do famoso CTRL+C CTRL+V, mas pelo menos você vai conseguir fazer tudo com pouco esforço de configuração, sem quebrar a cabeça com códigos que você não entende.

Para que serve isso? Bem, às vezes, você não quer pagar um provedor para hospedar seu site ou projeto pontual. Às vezes você não quer fazer um blog no Wordpress para colocar seu portfólio. Às vezes, você que experimentar códigos HTML, CSS e JavaScript sem grandes complicações. Às vezes, você está só começando nesse mundo das publicações. Enfim, use como quiser.

*OBS: Esta é uma versão ainda não revisada por um segundo par de olhos. Não nos responsabilizamos por erros de digitação, pelo cenário político brasileiro nem por vistas cansadas*


<br>

- - -
<br>

* Primeiramente, abra uma conta [no GitHub][5]. É gratuito e rápido. Não se esqueça de confirmar a conta, a partir de um email que será enviado para você.



![Siga as setas vermelhas!][6]

* Após essa etapa, dirija-se à sua página do GitHub.



![Vai ser algo assim][7]

* Agora você deve criar um novo repositório, clicando em `New Repository`.



![Não é tão difícil!][8]

* Dê um nome para o repositório. Inicialmente, pode ser /**teste**
* Dê uma breve descrição para o projeto. Algo como: **este é um projeto teste**. É opcional, mas é bom utilizar esse campo por questões de boas práticas organizacionais.
* Certifique-se de selecionar a caixa `Initialize this repository with a README`. **Isso é particularmente importante** porque se você não selecionar, o GitHub vai presumir que você está iniciando e organizando seu repositório não pela interface web, mas sim a partir de um comando em seu computador, um processo diferente. Nós não vamos mexer com isso aqui. Aqui é beginner, mano!



![Setas salva-vidas][9]

* Agora você está na página do repositório onde colocará os seus códigos. Se você tem um HTML e um CSS prontos, ótimo. Se não, pode usar um exemplo do Volt, não cobramos nada por isso! Veja o exemplo aqui: _https://github.com/voltdatalab/Template-para-projetos_
* A página do repositório deve se parecer exatamente com a tela abaixo (claro, sem o “testesampa” escrito na minha descrição de teste):



![][10]

* O que você fará agora é subir os códigos um por um, através de um `CTRL+C + CTRL+V`. Há outras formas de se fazer isso com mais rapidez - principalmente através do aplicativo do GitHub pra desktop - mas são mais trabalhosas para configurar no começo, embora depois poupem bastante trabalho de copiar e colar e deixem os arquivos sincronizados. Mas é melhor que você saiba fazer isso no jeito mais básico primeiro. Haverá tutorial para isso depois (talvez)!
* Coloque uma descrição breve para o projeto de vocês, só para referência, mas **ignore por enquanto** o campo `Website` ao lado.



![Ignorem na cara dura o que está sob o vermelho][11]

* Clique no sinal de `+` do lado do nome do repositório.



![][12]

* Atribua um nome para o arquivo inicial HTML de vocês. Nesse caso, como será a página inicial (e por enquanto única) desse projeto, o nome deverá obrigatoriamente ser `index.html`.
* Cole no campo de texto abaixo de `Edit New File` todo o código HTML.



![Obrigatoriamente <em>index.html</em>][13]

* Role a tela para baixo e dê uma descrição alternativa se quiser, e clique em `Commit New File`. Nesse caso, o `Commit` funciona como o botão “Publicar” de um CMS.
* **Não se preocupe** com a opção _Create a new branch…_, não a usaremos. É útil para quem está mais familiarizado e quem colabora nos códigos, não é o caso agora.



![][14]

* Muito bem! Agora temos um arquivo publicado no nosso repositório. Note que ainda **não** há uma página publicada, o que foi publicado é um arquivo no seu repositório. Segure o andor, chegaremos lá.
* Pois bem, publicamos o HMTL, a estrutura, do nosso projeto. Agora precisamos dar os estilos dele, senão vai parecer aqueles sites da década de 1990, ou até pior.
* Façamos o mesmo processo de publicação anterior, clicando em `+` novamente, só que dessa vez criando um arquivo chamado `qualquernome.css`. Nesse caso, você pode chamar o arquivo do que você quiser, contanto que tenha a extensão `.css` e esteja linkado no `<head> </head>` de seu `index.html`.
* _OBS: para quem não se lembra, é assim que faz o link:_`<link rel="stylesheet" href="qualquernome.css" type="text/css" charset="utf-8">`_ou, se estiver em uma pasta CSS, basta colocar o nome da pasta na frente no href, assim:_`href=“css/qualquernome.css"`
* Dê o _Commit_ novamente para disponibilizar o arquivo no seu repositório.
* Excelente! Agora temos nosso repositório povoado! Mas calma lá, o projeto mesmo ainda não está no ar, só os arquivos necessários para ele.
* O pulo do gato para isso é simples, mas nada, absolutamente nada, óbvio.
* À esquerda do nome do repositório de vocês há um ícone que diz `master`. O que nós vamos fazer aqui é clicar nesse `master` e, no campo de texto, escrever literalmente `gh-pages`. Só assim o GitHub vai entender que você não quer apenas ter um repositório, mas também um site publicado, cuja página principal será o `index.html`. Cliquem em `Create Branch: gh-pages` e voilá!



![Isso é importante pra cacete][15]

* Ops, meu Deus, o que eu fiz de errado? Onde tá publicado? Ainda não publicou, né?
* Não, sinto muito (ufa!), ainda falta mais um passo para isso.
* Naquele campo que ignoramos no começo, o `Website`, precisamos colocar outra coisa muito simples, mas nada óbvia. Como o GitHub usa seu domínio github.com para os repositórios, ele redireciona todos os sites e projetos publicados para um outro domínio dele também, o com a terminação `github.io`.
* No campo `Website`, coloque o seguinte: `http://nome do seu repositório.github.io/**nome do projeto`
* Atente-se às letras maiúsculas. Os nomes deverão estar idênticos.
* Exemplo: http://**voltdatalab**.github.io/**testesampa**
* Não use o MEU nome de repositório, use o SEU!



![Não use o MEU nome de repositório, use o SEU][16]

* Agora sim! Seu projeto estará publicado nessa URL que você completou! Clique nela para ver seu trabalho. Como o GitHub precisa reconhecer as informações salvas, às vezes demora um pouco (tipo 30 segundos até um minuto) para espelhar o resultados, então se não deu certo logo na hora, espere um pouquinho.
* _OBS: Isso serve na hora de atualizar os códigos também, demora para renderizar_!
* Só uma última coisa. Não é fundamental, mas é bom você fazer isso para evitar confusão.
* Como agora você tem dois _branches_ dentro do mesmo repositório, o `master` e o `gh-pages`, você precisa priorizar o _gh-pages_. Isso porque toda vez que você for fazer uma mudança na sua página, se você a fizer no _master_, sua página não espelhará essas mudanças. Sua página só será alterada se você fizer as mudanças no _branch_ do `gh-pages`. Isso é fácil, você pode clicar naquela mesma caixa e selecionar entre `master` e `gh-pages`, mas é contraproducente ficar fazendo isso toda hora - sem contar que você pode depois esquecer de mudar e tudo vira uma confusão.
* Por que manter o `master` então? Bem, você pode apagar se quiser, mas é bom e de graça deixar de backup caso aconteça alguma coisa com seu código sob _branch_`gh-pages`.
* Para tornar o _gh-pages_ o padrão do seu repositório, vamos configurar isso em _Settings_ > _Branches_ > _Selecione o gh-pages na caixa_ > _Update_.



![][17]

* Você receberá uma mensagem de alerta, mas não se preocupe, não é nada demais, só quando várias pessoas trabalham no mesmo código e alguém faz essa mudança inadvertidamente.
* Pronto!


## Nerd! Você agora sabe publicar uma página na Internet.

[0]: http://twitter.com/ProjetoStock
[1]: http://voltdata.info
[2]: https://github.com/voltdatalab
[3]: http://twitter.com/voltmediabr
[4]: http://facebook.com/voltdata
[5]: http://github.com
[6]: https://c1.staticflickr.com/1/719/22346475599_db39a9422d_z.jpg
[7]: https://c1.staticflickr.com/1/607/22544467521_46c261e0cd_z.jpg
[8]: https://c2.staticflickr.com/6/5636/22507327496_b147043129_o.png
[9]: https://c2.staticflickr.com/6/5655/22345977598_c7a2a5f6c3_z.jpg
[10]: https://c2.staticflickr.com/6/5739/22345360900_9b698a4ffa_z.jpg
[11]: https://c1.staticflickr.com/1/690/22519805902_c437a365f6_z.jpg
[12]: https://c1.staticflickr.com/1/590/22533313525_b7fc3c1a3d_o.png
[13]: https://c2.staticflickr.com/6/5768/22507327876_fc823a3103_o.png
[14]: https://c2.staticflickr.com/6/5677/22507327956_9550904276_b.jpg
[15]: https://c2.staticflickr.com/6/5720/22519803312_2c0f356197_o.png
[16]: https://c1.staticflickr.com/1/658/22519803402_5213812875_b.jpg
[17]: https://c1.staticflickr.com/1/733/21910569724_eb3275bddf_b.jpg
