# Fonte de Tensão 3-12V 100mA
Projeto de uma fonte de tensão ajustável de 3 a 12 Volts com capacidade de 100 mA, desenvolvido pelo aluno Fernando Henrique Paes Generich(número USP 11795342).

## Objetivo
O projeto deve levar ao desenvolvimento de uma fonte elétrica que transforma a tensão de corrente de uma tomada(127 volts, neste caso) em uma tensão adequada ao circuito que será alimentado pela fonte, estabelecida entre 3 e 12 volts em corrente contínua.

## O circuito
![CircuitoFONTE](https://user-images.githubusercontent.com/61749461/85100680-1cf31880-b1d7-11ea-8b64-7cc05b509277.png)

## Link para o projeto no [Falstad](http://tinyurl.com/y5wa9udd)

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

Trabalho proposto pelo professor Eduardo Simões para a matéria de Eletrônica do Curso de Ciência de Computação do Instituto de Ciências Matemáticas e de Computação(ICMC-USP).
