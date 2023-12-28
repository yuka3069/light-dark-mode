nav {
z-index: 10;
position: fixed;
font-size: 24px;
letter-spacing: 3px;
padding: 25px;
width: 100vw;
background: rgb(255 255 255 / 50%);
}

z-index:10 :默认值是 1，这里确保在图层上面
position fixed 确保不被划走

<hr>

section {
min-height: 100vh;
display: flex;
justify-content: center;
align-items: center;
flex-direction: column;
}
min-height: 100vh; 确保每个 section 都能填满整个页面

<hr>

<i class="fab fa-github"></i> 使用的是 Font Awesome 图标库的样式类，而不是 Bootstrap Icons。要使 Font Awesome 图标正确渲染在网页上，您需要确保以下几点：

引入 Font Awesome 库：确保您已经正确地引入了 Font Awesome 库。您可以在 HTML 文档的 <head> 部分添加以下链接标签来引入 Font Awesome 库：

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

<hr>

.button {
cursor: pointer;
} 将鼠标指针变成按键，提示可以点击

/_ Projects Section _/
.buttons {
margin-top: 15px;
margin-bottom: 50px;
}

button {
min-width: 100px;
height: 40px;
cursor: pointer;
border-radius: 10px;
margin-right: 10px;
border: 2px solid var(--primary-color);
font-size: 15px;
outline: none;
}

button:disabled {
opacity: 0.4;
cursor: default;
}

button:hover:not(.outline) {
filter: brightness(110%);
}

.primary {
background: var(--primary-color);
color: var(--on-primary);
}

.secondary {
border: 2px solid var(--secondary-color);
}

.secondary,
.secondary:hover,
.outline.secondary:hover {
background: var(--secondary-color);
color: var(--on-primary);
}

.outline {
background: var(--background);
color: var(--on-background);
}

.outline:hover {
background: var(--primary-color);
color: var(--on-primary);
}
