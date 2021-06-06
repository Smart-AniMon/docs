# Especificações do Sistema
> Descrição das especificações de componentes do Sistema.



**Módulos**

1. [Sensor de Movimento.](#1-sensor-de-movimento)
2. [Sensor de Umidade e Temperatura.](#2-sensor-de-umidade-e-temperatura)
3. [Sistema de Localização e tempo.](#3-sistema-de-localização-e-tempo)
4. [Dispositivo fotográfico.](#4-dispositivo-fotografico)
5. [Hardware do módulo.](#5-hardware-do-modulo)

**Servidor**

6. [Hardware.](#6-hardware-do-servidor)
7. [Serviço de Identificação de Imagens](#7-serviço-de-identificação)

**Energia**

8. [Armazenador de energia.](#8-armazenador-de-energia)
9. [Gerador de energia.](#9-gerador-de-energia)



---



### 1. Sensor de Movimento

| Sensor de Presença e Movimento - PIR|                                |
|:------------------------------------:|:-----------------------------:|
|                **Modelo**                |           DYP ME003           |
|              **Qtd**                 |               1               |
|         **Tensão de Op.**            |           4,5V a 20V          |
|        **Tensão de Dados**           | 3,3V (C/ Mov.) e 0V (S/ Mov.) |
|           **Interface**              |            Digital            |
|            **Pinagem**               |        VCC, GND e Dados       |
|           **Faixa de Alcance**           |            3m a 7m            |
|          **Outras Informações**          |          [Datasheet](https://siccciber.com.br/wp-content/uploads/2020/06/FTC-PIR.pdf)      |

---

### 2. Sensor de Umidade e Temperatura

| Sensor de Umidade e Temperatura |                                                              |
| :-----------------------------: | :----------------------------------------------------------: |
|           **Modelo**            |                            DHT11                             |
|             **Qtd**             |                              1                               |
|        **Tensão de Op.**        |                         3V a 5V (DC)                         |
|          **Corrente**           |                        200uA a 500mA                         |
|     **Faixa Umidade Rel.**      |                       (20% a 90%) ± 5%                       |
|      **Faixa Temperatura**      |                     (0ºC - 50ºC ) ± 2ºC                      |
|          **Precisão**           |                           16 bits                            |
|          **Interface**          |                        Single Serial                         |
|           **Pinagem**           |                     VCC, GND, Dados e NC                     |
|      **Tempo de resposta**      |                              2s                              |
|     **Outras Informações**      | [Datasheet](https://img.filipeflop.com/files/download/Datasheet_DHT11.pdf) |

---

### 3. Sistema de Localização e Tempo

|   Módulo GPS + Antena   |                                                              |
| :---------------------: | :----------------------------------------------------------: |
|       **Modelo**        |                          GY-GPS6MV1                          |
|         **Qtd**         |                              1                               |
|    **Tensão de Op.**    |                        3,3V a 5V (DC)                        |
|      **Interface**      |                       UART, USB ou SPI                       |
| **Tensão da Interface** |                             3,3V                             |
| **Taxa de Tx. Padrão**  |                             9600                             |
|       **Pinagem**       |                      VCC, GND, TX e RX                       |
| **Outras Informações**  | [Datasheet](https://www.usinainfo.com.br/index.php?controller=attachment&id_attachment=97) |

---

### 4. Dispositivo fotográfico
| Dispositivo fotográfico |                                     |
|:-----------------------:|:-----------------------------------:|
|        **Modelo**       |        Camera Module v1 / v2        |
|         **Qtd**         |                  1                  |
|      **Resolução**      |           5 / 8 Megapixels          |
|         **Modo**        | 1080p30, 720p60 and 640 × 480p60/90 |
|         **Luz**         |            Infravermelho            |
|      **Interface**      |            Serial ou USB            |

---

### 5. Hardware do Módulo

| Módulo - Raspberry c/ wifi |               |
| :------------------------: | :-----------: |
|         **Modelo**         | Pi 3 modelo B |
|          **Qtd**           |       1       |
|          **RAM**           |      1GB      |
|        **MicroSD**         |      5GB      |

---

### 6. Hardware do Servidor
|  Servidor  |                    |
| :--------: | :----------------: |
| **Modelo** | Instância em Nuvem |
|  **Qtd**   |         1          |
|  **RAM**   |     4GB (8GB)      |
|   **HD**   |        1 TB        |

---

### 7. Serviço de identificação
|  Cloud Vision API  |                    |
| :--------: | :----------------: |
| **Empresa** | Google |
|  **Interface**   |         APIs REST ou RPC          |
|  **Preço**   |     1 mil a 5 milhões - US$4,50     |
|   **Obs.:**   |        Gratuito até mil imagens        |
|   **Arquivos Suportados**   |        JPEG, PNG8, PNG24, BMP e outros       |
|   **Dimensão mínima**   |        640x480 pixels (aprox. 300 mil pixels)      |
|   **Tamanho máximo**   |        10MB (base64 no JSON)      |
|   **Requisitos**   |        [Supported-files](https://cloud.google.com/vision/docs/supported-files)        |
|   **Outras Informações**   |        [Cloud Vision](https://cloud.google.com/vision)        |

---

### 8. Armazenador de energia
|    Bateria     |            |
|  :----------:  | :--------: |
|  **Modelo**    |     --     |
|    **Qtd**     |     1      |
|  **Tensão**    |     5V     |
| **Corrente**   |     3A     |
| **Capacidade** |  36000mAh  |
| **Interface**  |     USB    |

---

### 9. Gerador de energia
| Painel Fotovoltaico |     |
|:-------------------:|:---:|
|     **Modelo**      |  -- |
|      **Qtd**        |  1  |
|    **Potência**     | 30W |
