Nomes: Nicolas Marçal RM: 565982 

Nomes: Vinicius Ribeiro  RM: 564379 

 O sistema utiliza:
Sensor DHT22 para temperatura e umidade
Sensor LDR para luminosidade
LEDs indicadores (verde, amarelo e vermelho)
Buzzer para alerta sonoro
Protocolo MQTT para envio dos dados
As informações são enviadas continuamente para o broker público HiveMQ, permitindo visualização em dashboards ou aplicações web.

Componentes Utilizados
ESP32
Sensor DHT22
LDR
LED Verde
LED Amarelo
LED Vermelho
Buzzer

Funcionamento do Sistema
A cada 2 segundos o ESP32 realiza:
Leitura da temperatura e umidade pelo DHT22
Leitura da intensidade luminosa pelo LDR
Envio dos dados via MQTT
Atualização dos LEDs e alertas
🚨 Regras de Alerta
Temperatura > 30°C:
LED Vermelho ligado
Buzzer ativado
Luminosidade:
Baixa (< 1500): LED Verde ligado
Alta (>= 1500): LED Amarelo ligado

segue a ilustração a seguir
