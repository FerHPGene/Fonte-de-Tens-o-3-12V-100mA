# Fonte de Tensão 3-12V 100mA
Projeto de uma fonte de tensão ajustável de 3 a 12 Volts com capacidade de 100 mA, desenvolvido pelo aluno Fernando Henrique Paes Generich(número USP 11795342).

## Objetivo
O projeto deve levar ao desenvolvimento de uma fonte elétrica que transforma a tensão de corrente de uma tomada(127 volts, neste caso) em uma tensão adequada ao circuito que será alimentado pela fonte, estabelecida entre 3 e 12 volts em corrente contínua.

## O circuito
![CircuitoFONTE](https://user-images.githubusercontent.com/61749461/85100680-1cf31880-b1d7-11ea-8b64-7cc05b509277.png)

## Link para o projeto no [Falstad](https://falstad.com/circuit/circuitjs.html?cct=$+1+0.000005+19.867427341514983+40+5+43%0Av+16+96+16+256+0+1+60+127+0+0+0.5%0A34+zvoltage%5Cq13+0+1.7143528192808883e-7+0+2+13%0Az+480+320+480+240+2+zvoltage%5Cq13%0Ad+208+96+240+176+2+default%0Ad+176+176+208+96+2+default%0Ad+176+176+208+256+2+default%0Ad+208+256+240+176+2+default%0AT+64+96+208+256+0+4+0.16+-0.33798016264608133+0+0.999%0Aw+240+176+384+176+0%0Aw+640+176+432+176+0%0Aw+176+176+176+320+0%0Aw+176+320+384+320+0%0Aw+384+320+480+320+0%0Ar+432+176+480+240+0+1200%0Ac+384+176+384+320+0+0.00047+18.88822742883686%0Aw+480+320+544+320+0%0Aw+384+176+432+176+0%0Aw+544+208+480+240+0%0At+608+240+640+240+0+1+-15.250287220201377+0.6782129226519498+100%0A174+544+208+544+256+1+5000+0.9950000000000001+Resistance%0Aw+592+240+608+240+0%0Aw+592+240+560+240+0%0Aw+640+176+640+224+0%0Aw+544+320+640+320+0%0Ar+640+256+640+320+0+120%0Ar+544+272+544+320+0+2200%0As+16+96+64+96+0+0+false%0Aw+64+256+16+256+0%0Ao+1+32+0+4099+20+0.00625+0+2+1+3%0Ao+23+32+0+4099+10+0.1+1+2+23+3%0Ao+13+32+0+4099+40+1.6+2+2+13+3%0A)

## Materiais

|Componente|Especificações|Preço|Função|Justificativa|
|---|---|---|---|---|
|Transformador|Entrada Bivolt e saída 20V|[R$35,80](https://produto.mercadolivre.com.br/MLB-1303044071-transformador-de-forca-110v220v-secundario-20v-400a-_JM#position=1&type=item&tracking_id=ac2214f9-28d9-4c75-94e5-4c0ff189a720)|Fornecer uma tensão de 20V para o circuito a partir da tensão da rede|A voltagem é mais próxima da que vai ser utilizada(3-12V) e apresenta corrente máxima de 400ma|
|Chave|250V e 20A|[R$6,50](https://produto.mercadolivre.com.br/MLB-1346929496-chave-gangorra-kcd4-201n-4t-1520a-250v-onoff-vermelha-neon-_JM?quantity=1#position=10&type=item&tracking_id=fb48c4d1-cddf-42d6-bbff-2e24e2022100)|Ligar e desligar o circuito|Suporta até 20A e é estilosa|
|Diodo|400V e 3A|[R$0,32](https://www.baudaeletronica.com.br/diodo-1n5404.html)|Faz com que a corrente percorra o circuito em apenas um sentido|Permite a transformação de AC em CC com a ponte de diodos|
|Diodo Zener|13V e 1W|[R$0,18](https://www.baudaeletronica.com.br/diodo-zener-1n4743-13v-1w.html)|Manter a corrente limitada a 13 V no máximo|A tensão comporta o valor que queremos que seja a saída da fonte(12V)|
|Capacitor|470 uF e 25V|[R$1,58](https://produto.mercadolivre.com.br/MLB-1452528217-capacitor-eletrolitico-470uf-25v-20-85-10x14mm-05pcs-_JM?quantity=1#position=3&type=item&tracking_id=afc603e6-7c55-4c17-95ec-4f410a0dfa64)|Permite que corrente percorra o circuito durante a inversão da corrente da tomada e consequente interrompimento da corrente fornecida pela ponte retificadora|Comporta até 5 Volts e 470uF permitem armazenar energia o suficiente para alimentar o circuito|
|Resistor|1.2KΩ|[R$0,07](https://www.baudaeletronica.com.br/resistor-1k2-5-1-4w.html)|Trata a corrente que passará pelo diodo zener e que irá para a base do NPN|Valor escolhido de forma a limitar a potência dissipada no zener(inferior a )|
|Resistor|2.2KΩ|[R$0,07](https://www.baudaeletronica.com.br/resistor-2k2-5-1-4w.html)|Limitar a tensão final|Valor que leva a tensão final a ser no mínimo 3V|
|Potenciômetro|5KΩ|[R$1,52](https://www.submarino.com.br/produto/212584212/potenciometro-linear-5k-16mm-eixo-estriado?pfm_carac=potenciometro%205k&pfm_page=search&pfm_pos=grid&pfm_type=search_page)|Variar a tensão|O potenciômetro escolhido consegue alternar a tensão entre 3 e 12V|
|Transistor NPN|modelo Bc337|[R$0,36](https://produto.mercadolivre.com.br/MLB-1189306444-50-x-transistor-bc337-25-bc337-25-npn-bc337-25-bc337-_JM?quantity=1#position=7&type=item&tracking_id=f3d70a25-c083-4c69-a338-b8571588ee84)|Controlar corrente e tensão de saída|Foi escolhido por suportar até 50V e 800mA|
|TOTAL|   |R$46,40|   |   |

## Projeto no EAGLE

Foram feitos os projetos esquemático e no PCB da fonte, ambos baseados nos componentes descritos acima, quando disponíveis, e quando não substituídos por componentes semelhantes, com escessão do Transformador que não apresenta modelo no programa.

### Schematic
![image](https://user-images.githubusercontent.com/61749461/88470100-cf9d5180-cece-11ea-824d-2d0ebd4d03ef.png)

### PCB
![PCBFonte](https://user-images.githubusercontent.com/61749461/88470116-feb3c300-cece-11ea-9d18-eabb4426d7d5.png)


Trabalho proposto pelo professor Eduardo Simões para a matéria de Eletrônica do Curso de Ciência de Computação do Instituto de Ciências Matemáticas e de Computação(ICMC-USP).
