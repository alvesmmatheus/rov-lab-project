# Estrutura do Projeto

## 🧭 Visão Geral

Este projeto simula um sistema ROV distribuído com sensores embarcados e interface gráfica em tempo real. A rede de comunicação entre os módulos embarcados utiliza RS-485, enquanto a interface com o topside (Raspberry Pi) é feita via Ethernet com dados em formato JSON.

## 🔌 Arquitetura Modular

- **TOGSNAV**: ESP32 com sensores e RTC
- **Nós RS-485**: Arduino Nano e sensores distribuídos
- **Topside**: Raspberry Pi com Node-RED, InfluxDB e Grafana
- **Conversores de mídia**: Ethernet ↔ Fibra óptica (opcional)

## 📡 Comunicação

- RS-485 com protocolo mestre-escravo
- Strings JSON estruturadas por sensor
- Integração com banco de dados InfluxDB
- Visualização com Grafana via HDMI

## 📋 Estrutura de Diretórios

```
rov-simulado/
├── README.md
├── CRONOGRAMA.md
├── arquitetura/
│   └── diagrama_geral.png
├── codigo/
│   ├── rov_firmware/
│   ├── topside_pi/
├── docs/
│   └── projeto_estruturado.md
└── LICENSE
```
