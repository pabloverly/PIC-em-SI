#### Projeto Integrador de Competências em Sistemas de Informação
Nome.: Pablo Verly 

##### 1) Atividade I
<p>
Muitas vezes, estamos na maior paz na empresa, de repente, seu chefe com a costumeira delicadeza fala:
Você é o responsável pelo projeto de informatização de uma empresa de nosso portfólio. Ele necessita transferir informações entre suas duas filiais (que se encontram geograficamente separadas por uma distância de 350 Km). Diante das opções de meios físicos disponíveis, você deve decidir pela implantação da melhor solução com o menor custo.
Ele passou algumas informações:
• A quantidade de dados que precisa ser transferida todos os dias à noite é de 22 MegaBytes. Não deve ser usada compactação nem compressão.
O tempo disponível para transferência é de 6 horas no máximo.
• O método de transferência deve ser assíncrono, com dois bits de sincronismo (a cada 8 bits transmitidos, 6 bits são de dados e 2 são de parada, 75% de aproveitamento).
• O protocolo de comunicação estabelece o aproveitamento de no mínimo 70% da taxa de transferência efetiva disponível. Os 30% restantes serão gastos com o protocolo e eventuais correções de erro na transmissão.
E, por fim, pediu a gentileza de colocar na mesa dele antes do almoço qual a taxa de transferência efetiva mínima que deve estar disponível, porque ele ia passar para a equipe de campo e para o cliente para deixá-lo tranquilo.
</p>

$$ TX = {22 x 1024x 1024 x 8 bits \over 6 x 60 x60 x 0,7 x 0,75 s} = 16.275 bps $$


<br />

<hr />

##### 1) Atividade II
<p>
Longo dia esse, hein?!
Seu chefe pediu para que você aplique o teste em um candidato a uma vaga para redes e te passou um seguinte problema para você utilizar.
Porém, ele pediu para que você o resolvesse antes, e este é o enunciado:
Imagine que uma pessoa treinou o seu cachorro, o Piteco, para carregar uma caixa de fitas DAT que pode conter até 3 fitas de 5 GBytes.
O cachorro consegue caminhar ao lado de seu dono a uma velocidade de até 15 Km/h.
Para qual faixa de distâncias o cachorro consegue ser mais rápido do que um canal de comunicação de 100 Mbps?
Seu chefe dá aquele sorriso maroto e diz para você que não se trata de um problema de física ou de matemática, mas de operações básicas o que interessa é somente seu entendimento do problema e a correta interpretação para construir a resposta.
Por fim, ele vira para você e diz para você se apressar, pois o candidato chega em 1 hora.
</p>

$$ tempo =  {3 x 5 x 1024 x 1024 x 1024 x 8 \over 100 x 1000 x 1000} = 1288,49    Segundos $$


$$ {1288,4 segundos\over60 segungos} =  21,47 Minutos  $$ 

Velocidade = 15 km/h 

Regra de 3

 $$ {60 min\over 21,4760 min} = {15km\over x} => x = 5,37 km  $$ 
 

<hr />
## Orientações técnicas

* Taxa de transferência

Para calcular a sua taxa de transferência você deve converter a sua conexão para KB e dividir o resultado por 8(1 Byte é composto de 8 Bits) pois a taxa de transferencia é representada em bits.

* Tempo de Download

Para calcular o tempo de download você deve converter o tamanho do arquivo para KB e depois dividir pela taxa de transferência.


* Velocidade de Internet

Primeiro precisamos converter as unidades de MB para KB e de minutos para segundos depois converte  KB/segundos e por ultimo transformando em MB 
