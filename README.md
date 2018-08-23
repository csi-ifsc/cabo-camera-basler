# cabo-camera-basler
Documentação e códigos referentes à camera Basler aca1300-60gc do laboratório de pesquisa CSI.


[clique aqui](https://docs.baslerweb.com/#t=en%2Faca1300-60gc.htm) para o manual completo.

## Conexões
![diagrama optoacoplador][diag-opto-in]

Para utilizar o modo de trigger, é somente necessário a conexão de um terra e um pino de sinal, 5 e 2 respectivamente, ambos com label física nos fios.

[diag-opto-in]:https://raw.githubusercontent.com/csi-ifsc/cabo-camera-basler/master/drawing_circuit_diagram_ace_usb3_opto_input_th.png

## setup software
para efetuar a captura de imagens utilizando o modo trigger no _pylon_, deve-se:
 * conectar a porta ethernet, e esperar a configuração da conexão
 * conectar-se à câmera desejada.
 * habilitar o trigger, escolher qual borda de clock
 * habilitar o modo de captura contínua.
 a cada vez que for efetuado um pulso no pino de entrada do optoacoplador
![diagrama interno conector][diag-conn]

[diag-conn]: https://raw.githubusercontent.com/csi-ifsc/cabo-camera-basler/master/drawing_ace_gige_pinout.png

## _Troubleshooting_

* caso a câmera não configure uma rede, tente:
    * reinicià-la
    * desconectar e reconectar cabo de rede
 
