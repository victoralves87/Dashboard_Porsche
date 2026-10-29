# 🏎️ Porsche Sales Intelligence Dashboard

Um dashboard executivo e interativo para análise de inteligência de vendas da **Porsche**. A aplicação foi desenvolvida em formato *Single File Application* (HTML/CSS/JS contidos em um único arquivo), fornecendo métricas estratégicas, gráficos dinâmicos e leituras de mercado baseadas em filtros em tempo real.

---

## 📌 Visão Geral

O **Porsche Sales Intelligence** tem como objetivo fornecer uma leitura precisa e ágil sobre o desempenho de vendas da marca em diferentes mercados. Ele consolida dados de faturamento, volume de vendas, preferências regionais e mix de produtos para apoiar tomadas de decisão sobre estoque, campanhas locais e condições comerciais.

---

## ✨ Funcionalidades

- **Métricas Executivas (KPIs):**
  - Volume total de vendas analisadas no recorte.
  - Faturamento total registrado em Dólar ($ USD).
  - Modelo Porsche líder em volume de vendas.
  - *Model Year* (Ano-Modelo) de maior incidência.

- **Filtros Dinâmicos e Combináveis:**
  - Filtragem por **Modelo Porsche** (ex: *911 Turbo S*, *Taycan*, *Cayenne*, *Macan*, *718 Cayman*, etc.).
  - Filtragem por **Model Year** (Ano do veículo).
  - Filtragem por **Cidade/Mercado** (ex: *Los Angeles*, *Seattle*, *Miami*, etc.).
  - Filtragem por **Forma de Pagamento** (*Wire Transfer*, *Credit Card*, *Crypto Payment*, *Financing*, *Lease*, etc.).
  - Botão de reset rápido para restaurar o estado inicial da aplicação.

- **Visualizações Gráficas Dinâmicas (Chart.js):**
  - **Top Modelos por Cidade:** Gráfico de barras empilhadas horizontais indicando a distribuição geográfica dos modelos mais populares.
  - **Distribuição por Modelo:** Gráfico tipo *Doughnut* mostrando o *mix* e a porcentagem de participação de cada modelo nas vendas.
  - **Vendas por Ano-Modelo:** Gráfico de barras verticais que evidencia a tendência e o ritmo temporal de cada *Model Year*.

- **Geração de Insights Dinâmicos:**
  - Algoritmo que interpreta em tempo real a seleção de filtros atual e gera pontos de inteligência comercial com foco em mercado, liderança de mix e comportamento do consumidor.

- **Tabela e Ranking Regional:**
  - Tabela detalhada indicando as top cidades, modelo líder local, volume de vendas, ano-modelo mais vendido e percentual de participação no recorte filtrado.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5:** Estruturação semântica e layouts responsivos.
- **CSS3:** Estilização customizada seguindo a identidade visual corporativa e minimalista da Porsche (utilizando *CSS Variables*, *Grid* e *Flexbox*).
- **JavaScript (Vanilla JS - ES6+):** Manipulação do DOM, motor de filtragem de dados e cálculo das métricas.
- **[Chart.js](https://www.chartjs.org/):** Biblioteca para renderização dos gráficos interativos.
- **Google Fonts:** Tipografias *DM Sans* e *Manrope*.

---

## 📁 Estrutura de Dados

A aplicação consome diretamente um conjunto de dados higienizados contendo objetos com a seguinte estrutura:

```json
{
  "id": "7",
  "date": "2024-03-14",
  "model": "911 Turbo S",
  "year": 2024,
  "price": 235000.0,
  "city": "Seattle",
  "state": "WA",
  "pay": "Wire Transfer",
  "status": "Delivered"
}
```

> **Nota:** Registros com campos em branco ou inconsistentes têm tratamento especial para evitar erros de renderização ou distorções nas análises temporais.

---

## 🚀 Como Executar o Projeto

Como o projeto é uma aplicação *client-side* contida em um único arquivo HTML, nenhum servidor backend ou etapa de compilação (*build*) é estritamente necessária.

1. **Clone ou baixe o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/porsche-sales-intelligence.git
   ```

2. **Execute o arquivo:**
   Navegue até a pasta do projeto e abra o arquivo `porsche_index.html` diretamente em qualquer navegador moderno (Google Chrome, Firefox, Safari, Edge).

   *(Opcional)* Caso prefira rodar com um servidor local no ambiente de desenvolvimento:
   ```bash
   # Utilizando Python 3
   python -m http.server 8000
   
   # Ou utilizando a extensão Live Server do VS Code
   ```
   Acesse no navegador através do endereço `http://localhost:8000/porsche_index.html`.

---

## 🎨 Design e Layout

O layout foi concebido para simular uma ferramenta corporativa oficial:
- **Tema:** Fundo claro (*warm gray*) com cartões e painéis em contraste branco e detalhes em *Porsche Red* (`#d5001c`).
- **Responsividade:** Suporte completo a telas *Desktop*, *Tablets* e dispositivos móveis através de *media queries*.

---

## 📄 Licença

[Este projeto é um dashboard demonstrativo para fins de análise e portfólio.](https://porsche-board.vercel.app/)

<img width="1412" height="940" alt="image" src="https://github.com/user-attachments/assets/e2b14fc9-2a42-4175-a0e8-b6b87ee45944" />

