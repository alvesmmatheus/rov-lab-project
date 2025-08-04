# SEACOM-X – Módulo de Navegação Embarcado

Este documento descreve a montagem física e a ligação dos sensores ao ESP32 para o módulo NAVCOM-X do projeto ROV simulado.

As conexões de cada sensor são listadas abaixo de suas respectivas imagens.

---

## 📦 ESP32 – Pinout

![ESP32 Pinout](esp32_pinout.png)

---

## 🔹 MPU-6050 (Acelerômetro + Giroscópio)

![MPU-6050](mpu6050.png)

| Pino do Módulo | Vai no ESP32 |
|----------------|--------------|
| VCC            | 3.3V         |
| GND            | GND          |
| SDA            | GPIO 21      |
| SCL            | GPIO 22      |

---

## 🔹 HMC5883L (Bússola)

![HMC5883L](hmc5883l.png)

| Pino do Módulo | Vai no ESP32 |
|----------------|--------------|
| VCC            | 3.3V         |
| GND            | GND          |
| SDA            | GPIO 21 *(compartilhado)* |
| SCL            | GPIO 22 *(compartilhado)* |

---

## 🔹 GPS GY-NEO6MV2

![GPS NEO-6M](neo6m_gps.png)

| Pino do Módulo | Vai no ESP32 |
|----------------|--------------|
| VCC            | 3.3V         |
| GND            | GND          |
| TX             | GPIO 16 *(RX1)* |
| RX             | GPIO 17 *(TX1)* |

---

## 🔹 MAX6675 (Termopar tipo K)

![MAX6675](max6675.png)

| Pino do Módulo | Vai no ESP32 |
|----------------|--------------|
| VCC            | 3.3V         |
| GND            | GND          |
| SCK            | GPIO 18      |
| SO             | GPIO 19      |
| CS             | GPIO 5       |

---

---

## 🔸 Módulo MAX485 (RS-485)

![MAX485](MAX485.png)

| Pino do Módulo | Vai no ESP32 |
|----------------|--------------|
| RO (Receive Out) | GPIO 3 *(RX)*     |
| DI (Driver In)   | GPIO 1 *(TX)*     |
| DE (Enable)      | GND *(fixo ou GPIO controle)* |
| RE (Receive Enable) | GND *(fixo ou GPIO controle)* |
| VCC              | 3.3V ou 5V        |
| GND              | GND               |
| A/B              | Barramento RS-485 |
