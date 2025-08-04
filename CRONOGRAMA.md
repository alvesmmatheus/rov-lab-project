# Cronograma de Desenvolvimento – V1 do Projeto ROV Simulado

| Semana      | Período       | Tarefa                                                                 |
|-------------|---------------|------------------------------------------------------------------------|
| Semana 1–2  | 04/08 – 17/08 | Finalizar diagrama da arquitetura modular                             |
|             |               | Testar comunicação RS-485 ponto-a-ponto (ESP32 ↔ Arduino Nano)        |
|             |               | Montar protótipo de 2 ou 3 nós da rede                                 |
|             |               | Definir protocolo de string (JSON estruturado)                         |
|             |               | Estabilizar comunicação entre ROV e topside via Ethernet              |
| Semana 3–4  | 18/08 – 31/08 | Integrar sensores no TOGSNAV (IMU, temperatura, RTC, tensão, corrente) |
|             |               | Publicar dados via JSON na rede RS-485                                |
|             |               | Construir lógica de polling do interrogador (Arduino Master)          |
|             |               | Sincronizar timestamp via RTC                                         |
| Semana 5–6  | 01/09 – 14/09 | Configurar Raspberry Pi com Node-RED, InfluxDB e Grafana              |
|             |               | Criar serial virtual para receber dados JSON                          |
|             |               | Parsear dados no Node-RED e armazenar no InfluxDB                     |
|             |               | Visualizar dados no Grafana (ângulo, aceleração, temperatura)         |
|             |               | Testar sistema em funcionamento contínuo                              |
| Semana 7–8  | 15/09 – 28/09 | Testes de resiliência (falhas simuladas)                              |
|             |               | Verificar watchdogs, timeout e fail-safe                              |
|             |               | Documentar hardware e software da V1                                  |
|             |               | Preparar post para LinkedIn com vídeo e explicação                    |
