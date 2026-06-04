```javascript
// script.js

document.addEventListener("DOMContentLoaded", () => {
    const sky = document.querySelector(".sky");

    function createCloud() {
        const cloud = document.createElement("div");

        cloud.classList.add("cloud");

        const size = Math.random() * 120 + 100;
        const topPos = Math.random() * 300;

        cloud.style.width = `${size}px`;
        cloud.style.height = `${size * 0.35}px`;
        cloud.style.top = `${topPos}px`;
        cloud.style.left = "-250px";

        const duration = Math.random() * 20 + 20;

        cloud.animate(
            [
                { transform: "translateX(0)" },
                { transform: `translateX(${window.innerWidth + 400}px)` }
            ],
            {
                duration: duration * 1000,
                iterations: Infinity,
                easing: "linear"
            }
        );

        sky.appendChild(cloud);
    }

    // สร้างเมฆเริ่มต้น
    for (let i = 0; i < 5; i++) {
        createCloud();
    }
});
```
