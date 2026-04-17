# Gateway IoT Multi-Protocolo (MSP430 version)

![Status do Projeto](https://img.shields.io/badge/Status-Desenvolvimento-yellow)
![Microcontrolador](https://img.shields.io/badge/MCU-MSP430FR6005-red)
![PCB](https://img.shields.io/badge/PCB-KiCad-green)

## Descrição
Diferentemente das tradicionais SBCs baseadas em MPUs de alta performance, este circuito de Gateway IoT é baseado em um MCU para aplicações que necessitam gerenciar a sua rede IoT no modo ultra-low power.

<p align="center">
  <img width="613" height="579" alt="Gateway IoT MSP430" src="https://github.com/user-attachments/assets/e052b93b-27cc-4eb5-a4c2-b3a6655ff35e">
</p>

---

## Descrições técnicas
- Microcontrolador: MSP430FR6005;
- Alimentação externa de 5V;
- Possui a capacidade de realizar a comunicação com até 4 periféricos UARTs padrão FAPLO;
- Capacidade de se comunicar por meio do protocolo de comunicação:
  - 4 x UARTs (UART0, UART1, UART2, UART3);
  - 1 x RS-485 (UART2);
  - 1 x I2C (UART1);
  - 2 x SPIs (UART0 e UART1);
- Possui LEDs de troca de dados da UART0;
- Todos os demais pinos dos conectores padrão FAPLO podem ser usados como pinos de propósito gerais.

---

## Estrutura do repositório
Os arquivos de hardware foram desenvolvidos utilizando o KiCad 9.0.
- **`.kicad_pcb`**: Layout da placa de circuito impresso (Board).
- **`.kicad_sch`**: Esquemático eletrônico do sistema (Schematic).
- **`.kicad_pro`**: Gerenciador de projeto do KiCad (Project).

---

## Autor
**Dr. Luiz Fernando Pinto de Oliveira**

*Engenheiro Eletrônico especializado em Sistemas Embarcados e Ultra-Low Power.*
- **Website:** [FAPLO](https://faplo.webnode.page/)
- **LinkedIn:** [lfpo](https://www.linkedin.com/in/lfpo/)

---

Shield: [![CC BY-NC-ND 4.0][cc-by-nc-nd-shield]][cc-by-nc-nd]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-NoDerivs 4.0 International License][cc-by-nc-nd].

[![CC BY-NC-ND 4.0][cc-by-nc-nd-image]][cc-by-nc-nd]

[cc-by-nc-nd]: http://creativecommons.org/licenses/by-nc-nd/4.0/
[cc-by-nc-nd-image]: https://licensebuttons.net/l/by-nc-nd/4.0/88x31.png
[cc-by-nc-nd-shield]: https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg
