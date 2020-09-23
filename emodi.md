 Programa Python para imprimir Emojis
 
 Última atualização: 20-12-2018
 Existem várias maneiras de imprimir os Emojis em Python. Vamos ver como imprimir Emojis
 com Uniocdes, nomes CLDR e emoji módulo.

# ************************************************************************************ #

 Usando Unicodes:
 Cada emoji tem um Unicode associado a ele. Emojis também têm um nome abreviado CLDR, que também
  pode ser usado.

 Na lista de Unicodes, substitua “+” por “000”. Por exemplo - “U + 1F600” se tornará “U0001F600”
 e prefixará o unicode com “\” e o imprimirá.

 filter_none
 brilho_4
 # grinning face 
 print("\U0001f600") 
  
 # grinning squinting face 
 print("\U0001F606") 
  
 # rolling on the floor laughing 
 print("\U0001F923") 
 Resultado:

# ************************************************************************************ #
 
 Usando o nome abreviado CLDR:

 filter_none
 brilho_4
 # grinning face 
 print("\N{grinning face}") 
  
 # slightly smiling face 
 print("\N{slightly smiling face}") 
  
 # winking face 
 print("\N{winking face}") 
 Resultado:

# ************************************************************************************ #

 Usando o módulo de emoji:

 Emojis também podem ser implementados usando o módulo emoji fornecido em Python. Para instalá-lo, execute o seguinte no terminal.

 pip install emoji
 emojize()A função requer que o nome abreviado CLDR seja passado como o parâmetro. Em seguida, ele retorna o emoji correspondente. Substitua os espaços por sublinhado no nome abreviado CLDR.

 filter_none
 brilho_4
 # import emoji module  
 import emoji 
  
 print(emoji.emojize(":grinning_face_with_big_eyes:")) 
 print(emoji.emojize(":winking_face_with_tongue:")) 
 print(emoji.emojize(":zipper-mouth_face:")) 
 Saída: a

 demojize() função converte o emoji transmitido em seu nome abreviado CLDR correspondente.

# ************************************************************************************ #

 Abaixo está uma lista de alguns Unicodes de emoji comuns com seus nomes abreviados CLDR:

 NOME ABREVIADO DE CLDR	UNICODE
 rosto sorridente	U + 1F600
 rosto sorridente com olhos grandes	U + 1F603
 rosto sorridente com olhos sorridentes	U + 1F604
 rosto radiante com olhos sorridentes	U + 1F601
 rosto sorridente e vesgo	U + 1F606
 rosto sorridente com suor	U + 1F605
 rolando de rir no chão	U + 1F923
 rosto com lágrimas de alegria	U + 1F602
 rosto ligeiramente sorridente	U + 1F642
 cara de cabeça para baixo	U + 1F643
 rosto piscando	U + 1F609
 rosto sorridente com olhos sorridentes	U + 1F60A
 rosto sorridente com auréola	U + 1F607
 rosto sorridente com 3 corações	U + 1F970
 rosto sorridente com olhos de coração	U + 1F60D
 atingido por estrelas	U + 1F929
 cara mandando um beijo	U + 1F618
 rosto beijando	U + 1F617
 rosto sorridente	U + 263A
 beijando rosto com olhos fechados	U + 1F61A
 beijando rosto com olhos sorridentes	U + 1F619
 cara saboreando comida	U + 1F60B
 cara com língua	U + 1F61B
 rosto piscando com língua	U + 1F61C
 cara maluca	U + 1F92A
 rosto apertando os olhos com a língua	U + 1F61D
 cara que fala dinheiro	U + 1F911
 rosto abraçando	U + 1F917
 rosto com mão sobre a boca	U + 1F92D
 cara calada	U + 1F92B
 cara pensativa	U + 1F914
 cara com boca de zíper	U + 1F910
 rosto com sobrancelha levantada	U + 1F928
 rosto neutro	U + 1F610
 rosto sem expressão	U + 1F611
 cara sem boca	U + 1F636
 rosto sorridente	U + 1F60F
 rosto não divertido	U + 1F612
 rosto com olhos revirados	U + 1F644
 rosto fazendo careta	U + 1F62C
 cara mentirosa	U + 1F925
 rosto aliviado	U + 1F60C
 rosto pensativo	U + 1F614
 cara de sono	U + 1F62A
 cara babando	U + 1F924
 rosto adormecido	U + 1F634
 rosto com máscara médica	U + 1F637
 rosto com termômetro	U + 1F912
 rosto com bandagem na cabeça	U + 1F915
 rosto nauseado	U + 1F922

 Folha de referências de emoji: http://www.emoji-cheat-sheet.com/

 Lista oficial de Unicode: http://www.unicode.org/Public/emoji/1.0/full-emoji-list.html

