# Códigos e Exemplos Explicados - ATmega328P


## Descrição

Esse repositório contém exemplos de código Assembly do ATmega328P, com foco na explicação da lógica e funcionamento do microcontrolador.
Cada pasta contém o código e o circuito do exemplo, e um arquivo de texto explicativo.
O objetivo é explicar os exemplos passados em sala da matéria Programação de Software Básico do curso de Ciência da Computação da UFBA.

## Diretórios

**Exemplos** --> Contém os códigos e circuitos utilizados.  
**Extra** --> Contém informações adicionais sobre a matéria.

## Ferramentas
* **Simulide:** Software usado para criar os circuitos eletrônicos.
* **Microchip Studio:** Software usado para programação e compilação dos códigos Assembly.
* **AVRA:** Montador do código.

## Exemplos e Fundamentos abordados
1. **LigarLed:** funcionamento básico dos registradores de *output*.
2. **LigarLedNeg:** lógica negativa de um circuito LED.
3. **PiscarLed:** rotinas de atraso.
4. **ContadorBinario4bits:** rotina de atraso e contagem binária.
5. **BotaoLigarDesligar:** tratamento de *input* e *PINx*.
6. **BotaoIncrementarDecrementar:** implementação de vários *inputs* e lógica negativa
7. **Relogio9seg:** lidar com rotinas de contagem de tempo preciso e *refresh rate*
## Instruções
1. Instalar Microchip Studio (Microsoft) ou AVRA (Linux).
*   No linux: monte um arquivo .asm usando editor de texto. O começo do código deve conter as   seguintes instruções:  
    *.nolist  
    .include "m328Pinc.def"  (o arquivo "m328Pinc.def" deve está presente na mesma pasta do código assembly)  
    .list*

    Para compilar:  
    cd "Diretório onde o arquivo .asm foi salvo"  
    AVRA nome_do_arquivo.asm
* No Windows: monte crie um novo projeto no Microchip Studio e cole o código presente no github. Para compilar, aperte o botão F7 ou clique na opção Build --> Build Solution (F7).

2. Após compilar o código, um arquivo .hex será gerado no diretório onde o arquivo foi compilado (linux) ou na pasta "Debug" associada ao projeto do Microchip Studio. Esse arquivo é o responsável por carregar o código no ATmega328P do Simulide.
3. Por fim, monte o circuito e clique com o botão direito no ATmega328P, vá na opção "Load Firmware" e escolha o .hex do projeto associado. Por fim, basta clicar no botão "Run" presente no topo do Simulide.

## Considerações Finais

O repositório serve como complemento do assunto dado em aula e cada exemplo possui um exercício sugerido para o estudante aplicar a teoria aprendida. Recomendo a leitura dos textos explicativos após o leitor tentar interpretar os códigos sozinhos. 

### Autor
    Pedro Henrique Dias Simão - Ciência da Computação, UFBA.

