# Dashboard IoT – Monitoramento de Temperatura e Umidade em Tempo Real

Este projeto apresenta dados de **temperatura e umidade** coletados por um sensor IoT (ESP32-C3 + DHT11) enviados para o **ThingSpeak**, exibidos em um dashboard web atualizado em tempo real usando Node.js e Chart.js.

---

## 🔹 Funcionalidades

- Captura de dados via API HTTP do ThingSpeak  
- Três tipos de gráficos:
  - Umidade (%)
  - Temperatura (°C)
  - Gráfico combinado (Umidade + Temperatura)  
- Atualização automática a cada 10 segundos  
- Layout moderno com containers estilizados e tooltips interativos  
- Funciona localmente (`localhost`) sem gerar imagens PNG

---

## 🔹 Tecnologias Utilizadas

- **Node.js** – servidor web e requisições à API  
- **Express** – criação de rotas HTTP  
- **Axios** – comunicação HTTP com o ThingSpeak  
- **Chart.js** – gráficos interativos em JavaScript  
- **dotenv** – gerenciamento de variáveis de ambiente

---

## 🔹 Pré-requisitos

- Node.js (recomenda-se v16 ou superior)  
- NPM  
- Canal no ThingSpeak com os campos:
  - `field1`: Temperatura  
  - `field2`: Umidade  

---

## 🔹 Configuração

1. Clone o repositório:  
```bash
git clone <link-do-seu-github>
cd <nome-do-projeto>

## 🔹 Configuração

1. Clone o repositório:  
```bash
git clone <link-do-seu-github>
cd <nome-do-projeto>

Instale as dependências:
npm install express axios dotenv

Crie um arquivo .env na raiz do projeto com as seguintes variáveis:
CHANNEL_ID=XXXXX
READ_API_KEY=XXXXXXX
RESULTS=XXXXXXX

Substitua CHANNEL_ID e READ_API_KEY pelos dados do seu canal ThingSpeak.
