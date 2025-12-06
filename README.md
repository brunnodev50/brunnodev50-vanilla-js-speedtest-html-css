# ⚡ Vanilla JS Speed Test (Cyberpunk Edition)

![Project Status](https://img.shields.io/badge/status-finished-success) ![License](https://img.shields.io/badge/license-MIT-blue)

Um medidor de velocidade de internet responsivo, desenvolvido com **Vanilla JavaScript** puro, focado em performance, manipulação do DOM e uma estética futurista **Neon/Cyberpunk**.

![Preview do Projeto](https://via.placeholder.com/800x400?text=Adicione+um+Print+ou+GIF+do+Projeto+Aqui)
*(Dica: Substitua essa imagem acima por um print da tela do seu projeto)*

> "Um medidor de velocidade focado não apenas em métricas, mas na experiência visual do usuário."

## 🚀 Funcionalidades

- **Teste de Download Real:** Realiza o download de um arquivo de teste de 10MB (via servidor confiável) para cálculo preciso de banda em tempo real.
- **Fallback Inteligente:** Sistema de contingência que utiliza a `navigator.connection` API caso o download principal sofra bloqueios (CORS/Adblock).
- **Interface Cyberpunk:** Design imersivo com efeitos de vidro (Glassmorphism), animações de scanner e "glitch text".
- **Visualização de Dados:** Medidor circular (Gauge) feito em SVG dinâmico que reage à velocidade.
- **Totalmente Responsivo:** Layout fluido que funciona perfeitamente em Desktop e Mobile.

## 🛠 Tecnologias Utilizadas

- **HTML5 Semântico:** Estrutura limpa e organizada.
- **CSS3 Avançado:**
  - CSS Grid & Flexbox para layout.
  - `@keyframes` para animações de performance.
  - Variáveis CSS (Custom Properties) para gerenciamento de tema neon.
- **Vanilla JavaScript (ES6+):**
  - `XMLHttpRequest` para monitoramento de progresso de download.
  - `Promises` e `Async/Await` para gerenciamento de fluxo assíncrono.
  - Manipulação direta do DOM (sem frameworks).

## 🔗 Live Demo (Teste Online)

Você pode testar o projeto rodando diretamente no navegador através do link abaixo:

👉 **[Acesse a Demonstração Online Aqui](https://brunnodev50.github.io/brunnodev50-vanilla-js-speedtest-html-css/)**

*(Nota: Certifique-se de ativar o GitHub Pages nas configurações do repositório para que este link funcione)*

## 📂 Como rodar localmente

Se quiser baixar o código para estudar ou modificar:

1. Clone este repositório:
   ```bash
   git clone [https://github.com/brunnodev50/brunnodev50-vanilla-js-speedtest-html-css.git](https://github.com/brunnodev50/brunnodev50-vanilla-js-speedtest-html-css.git)
