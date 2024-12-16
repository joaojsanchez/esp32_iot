# Projeto de IoT com ESP32, Simulação no Wokwi e Integração com Node-RED

Trabalho desenvolvido para a disciplina Plataformas de Prototipação para IoT do curso de Especialização em Internet das Coisas do Instituto Federal de São Paulo - Câmpus Catanduva.

<br>

## Visão Geral

A ideia geral do trabalho é realizar o monitoramento do resfriamento do ambiente de um Datacenter da empresa onde os alunos trabalham.
O trabalho é constituído por um sensor de temperatura e umidade DHT11 conectado ao ESP32. Os dados originados no sensor são publicados em um tópico via MQTT. Os dados são acessados por um dashboard Node-RED e armazenados em um banco de dados MySQL.

<br>

## Projeto WOKWI

Wokwi é um simulador de eletrônica online. Você pode usá-lo para simular Arduino, ESP32 e muitas outras placas, componentes e sensores populares.

Abaixo o esquema utilizado no projeto:

<img width="470" src="/Imagens/wokwi-project.png">

O projeto pode ser acessado através do link:

https://wokwi.com/projects/415174869895648257

<br>

## NODE-RED

Foi criado um servidor NODE-RED na instância da AWS. O link para acesso ao mesmo segue abaixo:

http://15.228.74.197:1880

<br>

Abaixo o Fluxo criado.
Os dados são recebidos através da conexão com o servidor MQTT e salvos em um banco de dados MYSQL.

<img width="470" src="/Imagens/nodered-fluxo.jpeg">

<br>

O dashboard exibe os dados e gráficos de Temperatura e Umidade.

<img width="470" src="/Imagens/nodered-controles.jpeg">
