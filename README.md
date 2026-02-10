<h1 align="center">Hey, I'm Aditya <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="28"></h1>

<p align="center">
  <b>Open Source Developer | DevOps Enthusiast | Full Stack Engineer</b>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/aditya-kuchekar-b08555369/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://github.com/aditya-systems-hub"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
</p>

<p align="center">
  <a href="https://github.com/aditya-systems-hub"><img src="https://img.shields.io/github/followers/aditya-systems-hub?label=Followers&style=social" alt="GitHub Followers"></a>
  <img src="https://komarev.com/ghpvc/?username=aditya-systems-hub&label=Profile%20Views&color=0e75b6&style=flat" alt="Profile Views" />
</p>

---

### About Me

```yaml
name: Aditya
role: Open Source Developer
focus: Building tools that solve real problems
motto: "Ship clean code. Automate everything. Contribute back."
```

- Writing code that powers infrastructure and web applications
- Contributing to open source projects that matter
- Automating workflows and building CI/CD pipelines
- Always learning, always shipping

---

### Tech Stack

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>

---

### About Me (Go)

```go
package main

import "fmt"

type Developer struct {
    Name       string
    Role       string
    Focus      []string
    Languages  []string
    Interests  []string
}

func (d Developer) String() string {
    return fmt.Sprintf(
        "👨‍💻 %s\n📌 %s\n🎯 Building: %v\n💻 Languages: %v\n🚀 Passionate about: %v",
        d.Name, d.Role, d.Focus, d.Languages, d.Interests,
    )
}

func main() {
    developer := Developer{
        Name:  "Aditya",
        Role:  "Open Source Developer | DevOps Enthusiast | Full Stack Engineer",
        Focus: []string{"Infrastructure", "Web Applications", "Automation"},
        Languages: []string{"Python", "JavaScript", "Go", "Bash"},
        Interests: []string{"CI/CD", "Kubernetes", "Cloud Native", "DevOps"},
    }
    
    fmt.Println(developer)
}

// Output:
// 👨‍💻 Aditya
// 📌 Open Source Developer | DevOps Enthusiast | Full Stack Engineer
// 🎯 Building: [Infrastructure Web Applications Automation]
// 💻 Languages: [Python JavaScript Go Bash]
// 🚀 Passionate about: [CI/CD Kubernetes Cloud Native DevOps]
```

---

### GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=aditya-systems-hub&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" width="48%" alt="GitHub Stats" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=aditya-systems-hub&theme=tokyonight&hide_border=true" width="48%" alt="GitHub Streak" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=aditya-systems-hub&layout=compact&theme=tokyonight&hide_border=true" width="40%" alt="Top Languages" />
</p>

---

### Contribution Graph

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=aditya-systems-hub&theme=tokyo-night&hide_border=true" width="95%" alt="Contribution Graph" />
</p>

---

### 🐍 Snake Game - Eating Contributions

<details>
<summary>Click to play the snake game that eats your contributions!</summary>

```html
<style>
  #snakeCanvas {
    border: 2px solid #30B87F;
    background-color: #0d1117;
    display: block;
    margin: 20px auto;
  }
</style>

<canvas id="snakeCanvas" width="400" height="400"></canvas>

<script>
  const canvas = document.getElementById('snakeCanvas');
  const ctx = canvas.getContext('2d');
  const gridSize = 20;
  const tileCount = canvas.width / gridSize;
  
  let snake = [{x: 10, y: 10}];
  let food = {x: 15, y: 15};
  let dx = 1;
  let dy = 0;
  let score = 0;
  
  // Contribution colors for the grid
  const contributionColors = ['#0d1117', '#16a34a', '#22c55e', '#4ade80', '#22d3ee'];
  
  function drawGrid() {
    for (let i = 0; i < tileCount; i++) {
      for (let j = 0; j < tileCount; j++) {
        const colorIndex = Math.floor(Math.random() * contributionColors.length);
        ctx.fillStyle = contributionColors[colorIndex];
        ctx.fillRect(i * gridSize, j * gridSize, gridSize - 1, gridSize - 1);
      }
    }
  }
  
  function drawSnake() {
    snake.forEach((segment, index) => {
      ctx.fillStyle = index === 0 ? '#22d3ee' : '#16a34a';
      ctx.fillRect(segment.x * gridSize + 1, segment.y * gridSize + 1, gridSize - 2, gridSize - 2);
    });
  }
  
  function drawFood() {
    ctx.fillStyle = '#f43f5e';
    ctx.fillRect(food.x * gridSize + 1, food.y * gridSize + 1, gridSize - 2, gridSize - 2);
  }
  
  function update() {
    const head = {x: snake[0].x + dx, y: snake[0].y + dy};
    
    if (head.x < 0 || head.x >= tileCount || head.y < 0 || head.y >= tileCount) {
      return false;
    }
    
    for (let segment of snake) {
      if (head.x === segment.x && head.y === segment.y) {
        return false;
      }
    }
    
    snake.unshift(head);
    if (head.x === food.x && head.y === food.y) {
      score++;
      food = {x: Math.floor(Math.random() * tileCount), y: Math.floor(Math.random() * tileCount)};
    } else {
      snake.pop();
    }
    return true;
  }
  
  function gameLoop() {
    drawGrid();
    drawSnake();
    drawFood();
    
    if (update()) {
      setTimeout(gameLoop, 100);
    } else {
      ctx.fillStyle = '#ffffff';
      ctx.font = '20px Arial';
      ctx.fillText(`Game Over! Score: ${score}`, 10, 30);
    }
  }
  
  document.addEventListener('keydown', (e) => {
    switch(e.key) {
      case 'ArrowUp': if (dy === 0) { dx = 0; dy = -1; } break;
      case 'ArrowDown': if (dy === 0) { dx = 0; dy = 1; } break;
      case 'ArrowLeft': if (dx === 0) { dx = -1; dy = 0; } break;
      case 'ArrowRight': if (dx === 0) { dx = 1; dy = 0; } break;
    }
  });
  
  gameLoop();
</script>
```

**How to play:** Use arrow keys to control the snake. Each contribution square you eat increases your score! 🐍💚

</details>

---

<p align="center">
  <i>"Talk is cheap. Show me the code." - Linus Torvalds</i>
</p>

<p align="center">
  <b>Open to collaborations on DevOps tooling, automation, and open source projects.</b>
</p>
