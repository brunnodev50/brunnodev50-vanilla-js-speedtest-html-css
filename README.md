# ⚡ Vanilla JS Speed Test (Cyberpunk Edition)

![Project Status](https://img.shields.io/badge/status-finished-success) ![License](https://img.shields.io/badge/license-MIT-blue) ![Technology](https://img.shields.io/badge/tech-Vanilla%20JS-yellow)

Um medidor de velocidade de internet responsivo, desenvolvido com **Vanilla JavaScript** puro. O projeto combina performance técnica, manipulação avançada do DOM e uma estética imersiva **Neon/Cyberpunk**.

![Preview Desktop](https://github.com/user-attachments/assets/78853eb8-e83a-46f5-b899-59e09e60a230)

---

### 🟢 Teste Agora (Live Demo)
O projeto está hospedado e funcionando em tempo real. Clique abaixo para testar sua conexão:

## 👉 [Acessar Demonstração Online](https://brunnodev50.github.io/brunnodev50-vanilla-js-speedtest-html-css/)

---

## 📸 Previews (Responsividade)

O layout foi projetado seguindo a metodologia *Mobile First*, adaptando-se perfeitamente a diferentes resoluções.

| Desktop View (Início) | Mobile View 1 | Mobile View 2 |
| :---: | :---: | :---: |
| ![Desktop](https://github.com/user-attachments/assets/6b3c15e1-aa10-47dd-a40c-8cc56d7bfc09) | ![Mobile 1](https://github.com/user-attachments/assets/aeea7098-8cba-4067-a50d-7b70fcf49087) | ![Mobile 2](https://github.com/user-attachments/assets/b337d83d-3088-458b-b593-021e431fc952) |

## 🚀 Funcionalidades

- **Teste de Download Real:** Realiza o download de um arquivo de teste de 10MB (via servidor confiável) para cálculo preciso de banda em tempo real.
- **Fallback Inteligente:** Sistema de contingência que utiliza a `navigator.connection` API caso o download principal sofra bloqueios (CORS/Adblock), garantindo que a UI nunca trave.
- **Interface Cyberpunk:** Design com efeitos de vidro (Glassmorphism), animações de scanner, grid 3D e tipografia técnica.
- **Visualização de Dados:** Medidor circular (Gauge) feito em **SVG dinâmico** que reage instantaneamente à velocidade detectada.
- **Totalmente Responsivo:** Layout fluido que se adapta a qualquer tamanho de tela.

## 🛠 Tecnologias Utilizadas

- **HTML5:** Estrutura semântica.
- **CSS3:**
  - `Grid` e `Flexbox` para layout.
  - `@keyframes` para animações de performance (60fps).
  - Variáveis CSS (Custom Properties) para gerenciamento de tema neon.
- **Vanilla JavaScript (ES6+):**
  - `XMLHttpRequest`: Para monitoramento granular do progresso de download (`onprogress`).
  - `Promises` & `Async/Await`: Para gerenciamento de fluxo assíncrono.
  - `DOM Manipulation`: Atualização da UI sem uso de frameworks virtuais.

## 🧠 Como Funciona a Lógica

O cálculo de velocidade segue o seguinte algoritmo:

1. **Start:** O script inicia o download de um arquivo binário de tamanho conhecido (ex: 10MB).
2. **Timestamp:** Marca o tempo inicial (`performance.now()`).
3. **Progress:** Durante o download, o evento `onprogress` calcula quantos bytes foram baixados.
4. **Cálculo:**
   ```javascript
   Velocidade (bps) = (Bytes Carregados * 8) / Tempo Decorrido (s)
   Mbps = Velocidade / (1024 * 1024)
