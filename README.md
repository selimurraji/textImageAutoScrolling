# textImageAutoScrolling
This project demonstrates a simple implementation of auto-scrolling text and images using only HTML and CSS. Ideal for creating dynamic banners, marquees, or smooth scrolling effects for websites without relying on JavaScript. Fully responsive and customizable.



# 🔄📜🖼️ using 🕸️ & 🎨

This 🛠️ showcases an 🔄-📜 text and 🖼️ slider made with pure 🕸️ & 🎨. It features 🌊 animations, 🎨 styling, and the ability to ↔️ the scroll direction.

## 🌟 Features

- **Pure 🕸️ & 🎨**: No 🧑‍💻 required.
- **🎛️**: 🖌️ colors, fonts, ⏩, and ↔️.
- **📱-🖥️ Design**: Adapts to 📏.
- **🖱️ Pause**: 🎥 stops on 🖱️.
- **↩️ Animation**: Use `reverse="true"` to ↔️ scroll.

## ⚙️ Installation

1. 🌀 the 📦:
   ```bash
   git clone https://github.com/your-username/autoscrolling-html-css.git
   ```
2. 📂 to the project:
   ```bash
   cd autoscrolling-html-css
   ```
3. Open `index.html` in your 🌐 to 📽️ the 💡.

## 🖼️ Usage

### 🕸️ 🛠️
📜 elements inside a 📦:
```html
<div reverse="true" class="autoScrolling">
  <div class="sliderList">
    <div class="item" style="--position: 1"><h2>// ✨</h2></div>
    <div class="item" style="--position: 2"><h2>// ✨</h2></div>
    <!-- ➕ items as needed -->
  </div>
</div>
```

### 🎨 ⚙️
🔑 variables for 🛠️:
```css
:root {
  --clr-bg: 🩵;
  --clr-white: 🪷;
  --clr-black: 🕳️;
  --clr-green: 🌿;
  --clr-olive: 🫒;

  --height: 250px;
  --width: 1000px;
  --quantity: 8; /* # of 🖼️ */
}
```
- **--height**: Height of the 📦.
- **--width**: Width of each 🖼️.
- **--quantity**: Total # of items.

## 🎥 ⚙️
🛠️ 📜 ⏩ or behavior:
1. 🔧 `@keyframes` 🎥:
   ```css
   @keyframes autoRun {
     from {
       left: 100%;
     }
     to {
       left: calc(var(--width) * -1);
     }
   }
   ```
2. Change the `animation-duration` for 🌊 or 🏃‍♂️ 🎥.

## ↔️ Direction
↔️ the 📜 with `reverse="true"`. Applies `reversePlay` 🎥:
```css
@keyframes reversePlay {
  0% {
    left: calc(var(--width) * -1);
    transform: translateX(0);
  }
  100% {
    left: 100%;
    transform: translateX(0);
  }
}
```

## 🌐 Support
Uses modern 🎨 like `@keyframes` & `mask-image`, ensuring compatibility with 🆕 🌐. Some 📜 🌐 may not fully 📯.

## 📝 License
📦 under the 🆓 MIT. 🖌️ & 🛠️ for personal or 🏢 📜.

## 🙏 Acknowledgments
- 🎨 by 💡 CSS 🌊 effects.
- Fonts from [Google Fonts](https://fonts.google.com/).

---

✨ building your 🎥 📜 effect! For ➕ or 🛠️, 👐 a pull request or an issue on the 🛠️ repository.


