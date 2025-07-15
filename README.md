# Kalpli-mesaj HTML (index.html)*

```html
<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Sana Özel Mesaj</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="container">
    <div class="heart"></div>
    <h1>Seni seviyorum ❤️</h1>
    <p>Kendine dikkat et lütfen 🌙</p>
  </div>
</body>
</html>
```

🎨 *CSS (style.css)*

```css
body {
  margin: 0;
  background: linear-gradient(135deg, #ffdee9, #b5fffc);
  font-family: 'Segoe UI', sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  overflow: hidden;
}

.container {
  text-align: center;
  animation: fadeIn 2s ease-in;
}

h1 {
  font-size: 2.5em;
  color: #e91e63;
}

p {
  font-size: 1.5em;
  color: #555;
}

.heart {
  width: 100px;
  height: 90px;
  position: relative;
  margin: 0 auto 20px;
  animation: pulse 1s infinite;
}

.heart::before,
.heart::after {
  content: "";
  position: absolute;
  width: 100px;
  height: 90px;
  background: red;
  border-radius: 50%;
}

.heart::before {
  left: -50px;
}

.heart::after {
  top: -50px;
}

@keyframes pulse {
  0% { transform: scale(1);}
  50% { transform: scale(1.1);}
  100% { transform: scale(1);}
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(-20px);}
  to { opacity: 1; transform: translateY(0);}
}
```

---
