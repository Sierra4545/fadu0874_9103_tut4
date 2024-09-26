# fadu0874_9103_tut4

# 1.Imaging Technique Inspiration

## Name of project
### [Simulation of water lily life cycle](https://www.xiaohongshu.com/explore/66f3a461000000001b023a8d?xsec_token=ABXfSaYzubDp4K8m1RBgdSHpuKzGiM_-ZFHZKIkumSv80=&xsec_source=pc_user)


**description：**  
This project focuses on the dynamic presentation of the life cycle of water lilies, including their growth, flowering, and interaction with the environment.

**Why it inspired me:**  
This project creates dynamic images in a three-dimensional form. Through code, it uses ellipse and water lily animations to change over time. It is very vital and artistic. I hope that my code can also show a kind of growth and change.

![water lily 3D](https://github.com/Sierra4545/fadu0874_9103_tut4/blob/main/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87%E7%BC%96%E8%BE%91_20240926233622.jpg)

![water lily 2D](https://github.com/Sierra4545/fadu0874_9103_tut4/blob/main/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20240926233535.png)

# 2.Coding Technique Exploration

**Code implementation:**  

The transformation of lotus leaves and flowers can be achieved with this code

[Game-of-life](https://p5js.org/examples/math-and-physics-game-of-life/)


以下代码展示了如何使用 `p5.js` 库来模拟抽象表现主义中的自由形态和随机性。

```javascript
function setup() {
  createCanvas(windowWidth, windowHeight);
  noLoop();
}

function draw() {
  background(255);
  for (let i = 0; i < 10; i++) {
    let x = random(width);
    let y = random(height);
    let size = random(50, 150);
    let color = [random(255), random(255), random(255)];
    fill(color);
    noStroke();
    ellipse(x, y, size, size);
    stroke(color);
    strokeWeight(random(2, 5));
    line(x, y, random(width), random(height));
  }
}
