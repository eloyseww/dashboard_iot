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

🔹 Estrutura do Projeto

thingspeak_projeto/
│
├─ index.js        # Servidor Node.js e dashboard
├─ .env            # Configurações do ThingSpeak
└─ README.md       # Este arquivo

🔹 Demonstração

Gráfico de Umidade: exibe histórico e valores atuais

Gráfico de Temperatura: exibe histórico e valores atuais

Dashboard combinado: visualiza os dois indicadores simultaneamente

Atualização em tempo real sem necessidade de recarregar a página

🔹 Observações

É possível alterar o intervalo de atualização no código (setInterval) de acordo com sua necessidade.
Projeto ideal para aprendizado de visualização de dados IoT e integração com ThingSpeak.