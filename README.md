# 💌 Carta Interativa

Um pequeno projeto interativo desenvolvido para praticar **HTML, CSS e JavaScript**.

A proposta é criar uma cartinha divertida com uma pergunta simples: **"Você quer ser meu namorado?"** 💖

O projeto mistura um visual retrô com interações em JavaScript, incluindo corações animados e um botão "Não" que foge quando o mouse se aproxima. 👀

---

## 🎀 Preview

A página apresenta:

* 💌 Uma carta com uma pergunta
* 💗 Botão **Sim**
* 🙈 Botão **Não** que foge do mouse
* 💖 Corações que aparecem ao clicar em "Sim"
* ✨ Animações e efeitos visuais
* 🎮 Fonte retrô `Press Start 2P`
* 🌸 Fundo com gradiente em tons de rosa e azul

---

## 🛠️ Tecnologias utilizadas

* **HTML5** — estrutura da página
* **CSS3** — estilização, posicionamento e animações
* **JavaScript** — interações e manipulação dos elementos
* **Google Fonts** — fonte `Press Start 2P`

---

## 📚 O que pratiquei

### HTML

Neste projeto pratiquei:

* Estrutura básica de uma página HTML
* Títulos com `<h1>`
* Parágrafos com `<p>`
* Botões com `<button>`
* Classes e `id`
* Importação de arquivo CSS externo
* Importação de fonte do Google Fonts
* Eventos diretamente nos elementos HTML

---

## 🎨 CSS

No CSS pratiquei:

* `display: flex`
* `flex-direction`
* `justify-content`
* `align-items`
* `linear-gradient`
* `border-radius`
* `box-shadow`
* `text-shadow`
* `position: absolute`
* `transition`
* `transform`
* `:hover`
* `:active`
* `@keyframes`
* Animações CSS

### 💌 Animação da carta

A carta possui uma animação de brilho criada com `@keyframes`:

```css
@keyframes brilho {
    0% {
        box-shadow: 0 0 10px rgba(255, 105, 135, 0.3);
    }

    100% {
        box-shadow: 0 0 20px rgba(255, 105, 135, 0.7);
    }
}
```

Isso cria um efeito de brilho que fica se repetindo.

---

## 💻 JavaScript

Essa foi a parte principal do exercício.

### 💖 Criando corações

Ao clicar no botão **Sim**, a função `clicou()` é executada.

Ela utiliza um `for` para criar vários corações:

```javascript
for (let i = 0; i < 10; i++) {
```

Depois, um novo elemento HTML é criado através do JavaScript:

```javascript
const coracao = document.createElement("div");
```

O coração recebe o emoji:

```javascript
coracao.innerHTML = "💖";
```

E também recebe a classe CSS:

```javascript
coracao.classList.add("coracao");
```

---

### 🎲 Posições aleatórias

Cada coração aparece em uma posição diferente utilizando `Math.random()`:

```javascript
coracao.style.left = Math.random() * 500 + "px";
coracao.style.top = Math.random() * 500 + "px";
```

Assim, a posição dos corações muda a cada clique.

---

### ⏱️ Removendo os corações

Depois de 1 segundo, o coração é removido da página:

```javascript
setTimeout(() => {
    coracao.remove();
}, 1000);
```

Isso permite criar o efeito de aparecer, subir e desaparecer.

---

## 🙈 O botão "Não"

A parte mais divertida do projeto é o botão **Não**.

Quando o mouse passa sobre ele, a função `teste()` é chamada:

```javascript
function teste() {
    const botao = document.getElementById("nao");

    const x = Math.random() * 500;
    const y = Math.random() * 500;

    botao.style.left = x + "px";
    botao.style.top = y + "px";
}
```

O JavaScript encontra o botão através do seu `id` e modifica sua posição usando coordenadas aleatórias.

Resultado: **o botão foge do mouse.** 😂

---

## 🧠 Conceitos de JavaScript praticados

Neste exercício comecei a trabalhar com:

* `function`
* `for`
* `let`
* `const`
* `document.createElement()`
* `document.getElementById()`
* `classList.add()`
* `innerHTML`
* `style`
* `Math.random()`
* `setTimeout()`
* `remove()`
* Eventos como `onclick` e `onmouseover`

---

## 💖 Projeto

**Carta Interativa**
Um exercício de HTML, CSS e JavaScript criado durante meus estudos de desenvolvimento web.

💌 ✨ 💖 🎮
