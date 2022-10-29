# write-up-CTF-OSINT
Realizado no canal do Discord Menina de cybersec  e desafios criados em conjunto com Sabrina Ramos e Lais Camargo
https://linktr.ee/meninadecybersec


## Resolução de Geolocalização:
Geolocalização - Difícil: 1000 pontos 

O objetivo do Challenge de geolocalização era trazer o nome de uma cidade.
As pistas eram a medalha de bronze, o mapa de fundo e o ano '1975' inscrito na medalha.
Se caso você fizesse uma busca rápida, fazendo essas combinações e considerando a temática do nosso servidor (One Piece), muito provavelmente você identificaria a flag.
O mapa ao fundo mostra uma região no Japão, onde estava localizada uma estátua de bronze do Luffy (personagem principal do anime One Piece) em homenagem ao mangaka/criador do anime, Eiichiro Oda, nascido em 01/01/1975. A homenagem, além de dizer respeito a cidade em que o mangaka nasceu, Kumamoto, deve-se também a ajuda que Oda ofereceu a região após esta ter sofrido uma catástrofe natural.

Flag: MC{Kumamoto}

## Resolução de Poder em Roma
O Poder em Roma - Médio: 500 pontos

A principio as informações recebidas eram:
Um txt com um user!
A presunção pelo @ determina que pode ser provavelmente um perfil numa rede social como Twitter ou Instagram. 
No instagram você acharia um perfil com uma "red flag" (que sinalizava a bandeira do ctf).
Nela você encontraria 4 posts e TODOS, absolutamente todos possuem conexão com a flag final, eles estão ali para te certificar do caminho certo. 
Vamos fazer um roadmap?
Análise do primeiro POST: 
Vocês conhecem a história do Júlio Cesar? )
 - Primeiro ponto de observação: 
   Sabemos que algo envolve a história do Julio Cesar.
Análise do segundo POST:
Meus amigos me dizem que quando estou sorrindo me pareço com ele. 
 - Pesquisando pelo Google Lens, você descobre que o personagem faz parte de um anime chamado ONE PIECE. 
Agora, o que tem haver ONE PIECE com Júlio César? kkk.
Análise terceiro POST:
 - Férias em Roma, aqui é uma pista "solta".
Análise quarto POST:
As pizzas romanas são as melhores!
http://encurtador.com.br/Y2ZvQ1U=
 - Agora sim, sua primeira pista real. 
 Ao abrir o Link encurtado você visualiza que ele retorna com um erro, certo? 
Mas preste bem atenção no mesmo, perceba o "=". 
O link está codificado em base64. 
Ao acessar um decodificador de base64, você conseguirá ter o link real e acessar uma calculadora de Cifra de César!
Agora faz sentido toda a história do Julio César e Roma né?
Cifra de César era um meio de comunicação bem legal usada por ele! 
E caso você não conseguisse chegar dessa maneira... 
Análise quinto POST:
Bom, temos aqui um flaticon de uma "roda" e um qr code. 
Vamos começar pelo flaticon, jogando ele no Google Lens e pesquisando um pouco mais você vai chegar em "Chiffre cesar - Icones sﾃｩcuritﾃｩ gratuites - Flaticon" (verificar)
Ao acessar o QR-CODE, você receberá um "código" letras bagunçadas. 
Mas.... 
Não é atoa! 
Jogando a frase "Hrbth-uv-tp"
Você chega em:
Akuma-no-mi (que é uma frase especial do one-piece) e tcharam, sua flag está ai!
Você poderia usar o Yandex também, conhecido como o "google" russo que é uma ótima ferramenta para imagem em osint.

A flag era: MC{Akuma-no-mi}

## Resolução de A Hermione pode ajudar

A hermione pode ajudar - Fácil: 250 pontos
Esse desafio é inspirado em Harry Potter e a dica você percebe no título do chall.
Você recebe o título como primeira dica e uma foto, onde constam os números "62442".
Assim como acontece no filme do Harry Potter: Quando Arthur Weasley leva Harry Potter ao Ministério da Magia, ele digita os números de um código secreto num telefone. Os números são 62442, as letras abaixo desses números no teclado de um telefone normal soletram a palavra “magic”. 

E essa era a flag: MC{Magic}

## Resolução de Originou os humanos
Originou os humanos - Fácil: 250 pontos

Esse desafio é inspirado no planeta natal de origem dos humanos em Star Wars.
A dica é um arquivo .png nomeado com o nome "planeta" já sendo a primeira dica.
Na imagem consta o texto clássico que aparece em cada filme da franquia.
O planeta de origem dos humanos em Star Wars é Coruscant.

A flag era: MC{Coruscant}
