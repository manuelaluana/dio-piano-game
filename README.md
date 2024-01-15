# Desafio Piano Virtual

O desafio é desenvolver um Piano virtual! Este piano vai possuir a opção de toca-lo utilizando o mouse ou as teclas
do próprio teclado do computador, além de controle de volume e a opção de ocultar as letras sobre as teclas.

## Linguagem de programação utilizada

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## Explicando o Sistema

Neste sistema estamos trabalhando com manipulação de _dom_, adicionar e remover classes com JS, _toggle_, _eventListeners_ e uma estilização mais profunda do HTML principalmente de _inputs_!

Onde:

> data-key: Permite fornecer a tag html um valor que será utilizado no JS para permitir que utilizemos o teclado do computador para tocar.

> addEventListener: Fica "escutando" uma ação, neste caso, clicks, keydown, input. Sempre verificando caso uma alteração tenha sido feita para disparar um evento.

> toggle: Adiciona e remove uma classe de um elemento.

## playTune

Sempre que houver interação com o Piano esta função será chamada, capturando o elemento html através de um _dataset_ e tocando o audio correspondente a ele, fazendo também o controle da tecla ativa através da adição/remoção da classe **active**.

### mapedKeys

Array responsável por armazenar o valor das keys. É utilizado no projeto para verificar se as teclas pressionadas no teclado do computador são compativeis com as teclas disponiveis no piano, assim evitando erros e garantindo que a tecla pressionada é a tecla compativel com um som.

## volumeSlider

Utiliza um eventListener para verificar modificações do input do tipo _range_, sendo 0 o menor valor disponivel de volume e 1 o maior. Esta função utiliza de uma outra **handleVolume**, responsável por capturar o valor gerado (entre 0 e 1) assim permitindo alteração de volume do Piano.

## KeysCheck

Utiliza de um eventListener para verificar se ocorre o evento de click no input do tipo _checkbox_. Esta função utiliza de outra **showHideKeys**, responsável por mapear as teclas do Piano e acionar um _toggle_ da classe **hide**, assim permitindo esconder o valor presente nas teclas que representam um teclado de computador.

Esta projeto faz parte do Bootcamp potência tech ifood - Desenvolvimento de Jogos! Ao qual me inscrevi.

[Projeto original DIO](https://github.com/felipeAguiarCode/js-music-keyboard-virtual);
