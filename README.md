# Auto-Scrolling Text and Images using HTML & CSS
This project demonstrates a simple implementation of auto-scrolling text and images using only HTML and CSS. Ideal for creating dynamic banners, marquees, or smooth scrolling effects for websites without relying on JavaScript. Fully responsive and customizable.



# Auto-Scrolling Text and Images using HTML & CSS

This project showcases an auto-scrolling text and image slider made with pure HTML & CSS. It features smooth animations, customizable styling, and the ability to reverse the scroll direction.

## Features

- **Pure HTML & CSS**: No JavaScript required.
- **Customizable**: Adjust colors, fonts, speed, and direction.
- **Responsive Design**: Adapts to various screen sizes.
- **Mouse Pause**: Animation stops on hover.
- **Reversible Animation**: Use `reverse="true"` to reverse the scroll direction.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/autoscrolling-html-css.git
   ```
2. Navigate to the project directory:
   ```bash
   cd autoscrolling-html-css
   ```
3. Open `index.html` in your browser to view the project.

## Usage

### HTML Structure
Wrap your elements inside a container:
```html
<div reverse="true" class="autoScrolling">
  <div class="sliderList">
    <div class="item" style="--position: 1"><h2>// personalize</h2></div>
    <div class="item" style="--position: 2"><h2>// personalize</h2></div>
    <!-- Add more items as needed -->
  </div>
</div>
```

### CSS Configuration
Define key variables for customization:
```css
:root {
  --clr-bg: aliceblue;
  --clr-white: #f6fcdf;
  --clr-black: #1a1a19;
  --clr-green: #859f3d;
  --clr-olive: #31511e;

  --height: 250px;
  --width: 1000px;
  --quantity: 8; /* Number of images */
}
```
- **--height**: Height of the container.
- **--width**: Width of each item.
- **--quantity**: Total number of items.

## Animation Configuration
Customize the animation speed or behavior:
1. Define the `@keyframes` for animation:
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
2. Change the `animation-duration` for faster or slower animation.

## Reversible Direction
Reverse the scroll direction by adding `reverse="true"`. This applies the `reversePlay` animation:
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

## Browser Support
This project uses modern CSS features like `@keyframes` and `mask-image`, ensuring compatibility with newer browsers. Some older browsers may not fully support these features.

## License
This project is licensed under the MIT License. Feel free to use and modify it for personal or commercial purposes.

## Acknowledgments
- Inspired by creative CSS animation effects.
- Fonts sourced from [Google Fonts](https://fonts.google.com/).

---

Happy building your scrolling animation effect! For questions or contributions, open a pull request or an issue on the repository.




