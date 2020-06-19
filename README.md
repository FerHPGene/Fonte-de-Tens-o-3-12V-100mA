# Fonte de Tensão 3-12V 100mA
Projeto de uma fonte de tensão ajustável de 3 a 12 Volts com capacidade de 100 mA, desenvolvido pelo aluno Fernando Henrique Paes Generich(número USP 11795342) para a disciplina de Eletrônica do curso de Ciências de Computação do ICMC-USP.

## Objetivo
O projeto deve levar ao desenvolvimento de uma fonte elétrica que transforma a tensão de corrente de uma tomada(127 volts, neste caso) em uma tensão adequada ao circuito que será alimentado pela fonte, estabelecida entre 3 e 12 volts em corrente contínua.

## O circuito
![CircuitoELETRONICA](https://user-images.githubusercontent.com/61749461/85095912-38572700-b1c9-11ea-89bb-b3e88bd2bbae.png)

## Link para o projeto no [Falstad](https://falstad.com/circuit/circuitjs.html?cct=$+1+0.000005+19.867427341514983+40+5+43%0Av+16+96+16+256+0+1+60+127+0+0+0.5%0A34+zvoltage%5Cq13+0+1.7143528192808883e-7+0+2+13%0Az+480+320+480+240+2+zvoltage%5Cq13%0Ad+208+96+240+176+2+default%0Ad+176+176+208+96+2+default%0Ad+176+176+208+256+2+default%0Ad+208+256+240+176+2+default%0AT+64+96+208+256+0+4+0.16+-0.16716540700167964+-2.7755575615628914e-17+0.999%0Aw+240+176+384+176+0%0Aw+640+176+432+176+0%0Aw+176+176+176+320+0%0Aw+176+320+384+320+0%0Aw+384+320+480+320+0%0Ar+432+176+480+240+0+1200%0Ac+384+176+384+320+0+0.0005+18.62575113963286%0Aw+480+320+544+320+0%0Aw+384+176+432+176+0%0Aw+544+208+480+240+0%0At+608+240+640+240+0+1+-5.732162754763323+0.714801513534411+100%0A174+544+208+544+256+1+10000+0.005+Resistance%0Aw+592+240+608+240+0%0Aw+592+240+560+240+0%0Aw+640+176+640+224+0%0Aw+544+320+640+320+0%0Ar+640+256+640+320+0+120%0Ar+544+272+544+320+0+5500%0As+16+96+64+96+0+0+false%0Aw+64+256+16+256+0%0Ao+1+32+0+4099+20+0.00625+0+2+1+3%0Ao+23+32+0+4099+20+0.2+1+2+23+3%0Ao+13+32+0+4099+40+3.2+2+2+13+3%0A)

## Materiais

|Componente|Especificações|Preço|Função|Justificativa|
|---|---|---|---|---|
|Transformador|Entrada Bivolt e saída 20V|[R$35,80](https://produto.mercadolivre.com.br/MLB-1303044071-transformador-de-forca-110v220v-secundario-20v-400a-_JM#position=1&type=item&tracking_id=ac2214f9-28d9-4c75-94e5-4c0ff189a720)|Fornecer uma tensão de 20V para o circuito a partir da tensão da rede|A voltagem é mais próxima da que vai ser utilizada(3-12V) e apresenta corrente máxima de 400ma|
|Chave|250V e 20A|[R$6,50](https://produto.mercadolivre.com.br/MLB-1346929496-chave-gangorra-kcd4-201n-4t-1520a-250v-onoff-vermelha-neon-_JM?quantity=1#position=10&type=item&tracking_id=fb48c4d1-cddf-42d6-bbff-2e24e2022100)|   |   |
|Diodo||[R$0,32](https://www.baudaeletronica.com.br/diodo-1n5404.html)|   |   |
|Capacitor|400V e 3A|[R$](https://www.baudaeletronica.com.br/diodo-1n5404.html)|   |   |
|Resistor|1.2K|[R$0,07](https://www.baudaeletronica.com.br/resistor-1k2-5-1-4w.html)|   |   |
|Resistor|2 x 2.7K|[R$0,14](https://www.baudaeletronica.com.br/resistor-2k7-5-1-4w.html)|   |   |
|Potenciômetro|   |[R$]()|   |   |
|Transistor|   |[R$]()|   |   |
