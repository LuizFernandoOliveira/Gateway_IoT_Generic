# Gateway IoT Multi-Protocolo 🌐

![Status do Projeto](https://img.shields.io/badge/Status-Desenvolvimento-yellow)
![Plataforma](https://img.shields.io/badge/Hardware-ESP32--WROOM--32U-blue)
![PCB](https://img.shields.io/badge/PCB-KiCad-green)

## 📝 Descrição
Este projeto consiste no desenvolvimento de um **Gateway IoT de baixo custo e alta eficiência**, projetado para servir como ponte de comunicação entre redes de sensores sem fios e a nuvem (Cloud). 

O hardware foi desenvolvido com foco em versatilidade, permitindo a integração de diferentes tecnologias de comunicação em uma única PCB compacta, ideal para aplicações em **Agricultura 4.0**, cidades inteligentes e monitorização industrial.

---

## 🛠 Especificações de Hardware

O coração do Gateway é o **ESP32-WROOM-32U**, escolhido pela sua robustez e conetividade nativa.

### Conetividade Suportada:
- **Wi-Fi & Bluetooth (Dual-mode):** Nativo do ESP32.
- **LoRa (Long Range):** Interface dedicada para módulos LoRa (como o RFM95W).
- **RS-485 / Modbus:** Circuito integrado para comunicação industrial e sensores cabeados de longa distância.
- **Expansão I2C/SPI:** Barramentos expostos para sensores adicionais ou displays.

### Gestão de Energia:
- Entrada de alimentação: 5V - 12V DC.
- Reguladores de tensão de alta eficiência para operação estável.
- Proteção contra inversão de polaridade.

---

## 📂 Estrutura do Repositório

- `/hardware`: Ficheiros de projeto do KiCad (Esquemático, PCB, Libs).
- `/gerber`: Ficheiros para fabricação da placa de circuito impresso.
- `/docs`: Datasheets dos componentes principais e esquemas em PDF.
- `/firmware`: Código de exemplo para inicialização dos protocolos (ESP-IDF / Arduino).

---

## 🚀 Como Utilizar

### 1. Hardware
Os ficheiros de fabricação estão na pasta `/gerber`. Recomendamos a utilização de placas com acabamento **HASL (Lead Free)** ou **ENIG** para melhor soldabilidade dos módulos SMD.

[Imagem da PCB 3D - Se tiver uma imagem, insira o link aqui]

### 2. Firmware (Requisitos)
Para programar o gateway, utilize o VS Code com a extensão **PlatformIO** ou a **Arduino IDE**.
Bibliotecas recomendadas:
- `LoRa` por Sandeep Mistry.
- `ModbusMaster` para comunicações RS-485.
- `PubSubClient` para integração com Brokers MQTT.

---

## 🏗 Arquitetura do Sistema
O gateway atua como um concentrador (SINK node). Ele recebe dados via LoRa/RS-485 de nós sensores remotos, processa as informações localmente e envia-as via MQTT/HTTP para uma plataforma de dashboard.



---

## 👨‍🔬 Autor
**Dr. Luiz Fernando Pinto de Oliveira**
*Especialista em Sistemas Microcontrolados e IoT.*
- **Website:** [FAPLO](https://faplo.webnode.page/)
- **LinkedIn:** [Seu link aqui]

## 📄 Licença
Este projeto está sob a licença [MIT](LICENSE). Sinta-se à vontade para utilizar, modificar e distribuir, desde que mantidos os créditos originais.

---
*Projeto desenvolvido para fomentar o ecossistema de hardware aberto no Brasil.*
