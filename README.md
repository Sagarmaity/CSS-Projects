CSS (**Cascading Style Sheets**) is a stylesheet language used to control the appearance and layout of web pages. It allows developers to separate content (HTML) from presentation, making websites visually appealing and responsive.  

---

## 🔹 **Key Concepts in CSS**  

### 📌 1. **Selectors & Properties**  
Selectors target HTML elements, and properties define their styles.  

Example:  
```css
p {
  color: blue; /* Text color */
  font-size: 16px; /* Font size */
}
```

### 📌 2. **Types of CSS**  
- **Inline CSS** (inside HTML elements)  
  ```html
  <p style="color: red;">This is red text.</p>
  ```
- **Internal CSS** (inside `<style>` in HTML `<head>`)  
  ```html
  <style>
    body {
      background-color: lightgray;
    }
  </style>
  ```
- **External CSS** (linked via `<link>` tag)  
  ```html
  <link rel="stylesheet" href="styles.css">
  ```

---

## 🎨 **CSS Properties**  

### 1️⃣ **Text & Font Styling**  
- `color` – Text color  
- `font-size` – Size of text  
- `font-family` – Typeface selection  
- `text-align` – Align text (left, center, right)  
- `text-decoration` – Underline, overline, none  

Example:  
```css
h1 {
  font-family: Arial, sans-serif;
  text-align: center;
}
```

---

### 2️⃣ **Box Model (Spacing & Sizing)**  
Every HTML element is a rectangular box consisting of:  
- **Content** (actual text or image)  
- **Padding** (space inside the border)  
- **Border** (outline around the element)  
- **Margin** (space outside the element)  

Example:  
```css
div {
  width: 200px;
  padding: 10px;
  border: 2px solid black;
  margin: 20px;
}
```

---

### 3️⃣ **Backgrounds & Borders**  
- `background-color` – Fills element background  
- `background-image` – Sets an image as background  
- `border` – Defines a border around an element  

Example:  
```css
div {
  background-color: lightblue;
  border: 2px solid black;
}
```

---

### 4️⃣ **Positioning & Layout**  
- `display` – Defines how elements behave  
  - `block`, `inline`, `flex`, `grid`, `none`  
- `position` – Specifies element positioning  
  - `static`, `relative`, `absolute`, `fixed`, `sticky`  
- `z-index` – Controls overlapping order  
- `overflow` – Controls content overflow  

Example:  
```css
.box {
  position: absolute;
  top: 50px;
  left: 100px;
}
```

---

### 5️⃣ **Flexbox & Grid (Modern Layouts)**  
- **Flexbox** – One-dimensional layout for aligning items  
- **Grid** – Two-dimensional layout for designing full pages  

Example (Flexbox):  
```css
.container {
  display: flex;
  justify-content: center; /* Align items horizontally */
  align-items: center; /* Align items vertically */
}
```

Example (Grid):  
```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr); /* 3 equal columns */
  gap: 10px;
}
```

---

### 6️⃣ **Transitions & Animations**  
- `transition` – Smoothly animates changes  
- `@keyframes` – Defines custom animations  

Example (Transition):  
```css
button {
  background-color: blue;
  transition: background-color 0.5s ease;
}

button:hover {
  background-color: red;
}
```

Example (Animation):  
```css
@keyframes move {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(100px);
  }
}

.box {
  animation: move 2s infinite alternate;
}
```

---

## 🌍 **Responsive Design (Media Queries)**  
Media queries adjust styles based on screen size.  

Example:  
```css
@media (max-width: 600px) {
  body {
    background-color: lightgray;
  }
}
```

---
