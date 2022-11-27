# 5000DOSA 블로그
<!doctype html>
 <html lang="ko">
  <head>
    <h1>체크박스를 클릭해보세요</h1>
    <meta charset="utf-8">
    <title>CSS</title>
    <style>
      .jb {
        margin: 10px 0px;
        width: 100px;
        height: 100px;
        background-color: orange;
      }
      @keyframes run {
        from {
          width: 100px;
        }
        to {
          width: 100%;
        }
      }
      .jb1 {
        animation-name: run;
        animation-duration: 2s;
        animation-fill-mode: forwards;
        animation-play-state: paused;
      }
      input:checked + div {
        animation-play-state: running;
      }
    </style>
  </head>
  <body>
    <input type="checkbox">
    <div class="jb jb1"></div>
  </body>
</html>

<br><br><br><br>

<html lang="ko">
  <head>
    <h1>미니언즈는 바나나를 좋아합니다</h1>
    <meta charset="utf-8">
    <title>CSS</title>
    <style>
      body {
        box-sizing: border-box;
        font-family: Consolas, monospace;
      }
      h1 {
        text-align: center;
      }
      img {
        max-width: 100%;
      }
      .jb-a {
        width: 400px;
        margin: 0px auto;
        position: relative
      }
      .jb-c {
        position: absolute;
        top: 0px;
        left: 0px;
        display: none;
      }
      .jb-a:hover .jb-c {
        display: block;
      }
    </style>
  </head>
  <body>
    
    <div class="jb-a">
      <img src="banana-g6d3f2053f_1280.jpg" alt="" class="jb-b">
      <img src="minions-g72be53c35_1280.jpg" alt="" class="jb-c">
    </div>
  </body>
</html>

<br><br><br><br>


<div class="container">
    <div>
      <h1>막대기를 클릭해보세요</h1>
      <div class="wrapper transition">
        <span class="stick"></span>
        <span class="stick"></span>
        <span class="stick"></span>
      </div>
    </div>
    <div>  
      <p></p>
      <div class="wrapper animation">
        <span class="stick"></span>
        <span class="stick"></span>
        <span class="stick"></span>
      </div>
    </div>
    <div>
      <p></p>
      <div class="wrapper svg">
        <svg viewBox="0 0 130 108" xmlns="http://www.w3.org/2000/svg" version="1.1">
          <rect width="120" height="20" rx="4" >
            <animate dur="0.3s" begin="toggle.begin" attributeName="width" values="120; 136" fill="freeze" calcMode="spline" keySplines="0.2 0 0.2 1;" />
            <animateTransform dur="0.3s" begin="toggle.begin" attributeName="transform" type="rotate" values="0 10 20;45 10 20" fill="freeze" calcMode="spline" keySplines="0.2 0 0.2 1;" />
            <animate dur="0.3s" begin="reverseToggle.begin" attributeName="width" values="136; 120" fill="freeze" calcMode="spline" keySplines="0.2 0 0.2 1;"/>
            <animateTransform dur="0.3s" begin="reverseToggle.begin" attributeName="transform" type="rotate" values="45 10 20; 0 10 20" fill="freeze" calcMode="spline" keySplines="0.2 0 0.2 1;"/>
          </rect>
          <rect y="44" width="120" height="20" rx="4" style="transform-origin: 50%" >
            <animateTransform dur="0.3s" begin="toggle.begin" attributeName="transform" type="scale" values="1; 0.1" fill="freeze" calcMode="spline" keySplines="0.2 0 0.2 1;"/>
            <animateTransform dur="0.3s" begin="reverseToggle.begin" attributeName="transform" type="scale" values="0.1; 1" fill="freeze" calcMode="spline" keySplines="0.2 0 0.2 1;"/>
          </rect>
          <rect y="88" width="120" height="20" rx="4">
            <animate dur="0.3s" begin="toggle.begin" attributeName="width" values="120; 136" fill="freeze" />
            <animateTransform dur="0.3s" begin="toggle.begin" attributeName="transform" type="rotate" values="0 10 88; -45 10 88" fill="freeze" calcMode="spline" keySplines="0.2 0 0.2 1;"/>
            <animate dur="0.3s" begin="reverseToggle.begin" attributeName="width" values="136; 120" fill="freeze" calcMode="spline" keySplines="0.2 0 0.2 1;"/>
            <animateTransform dur="0.3s" begin="reverseToggle.begin" attributeName="transform" type="rotate" values="-45 10 88; 0 10 88" fill="freeze" calcMode="spline" keySplines="0.2 0 0.2 1;" />
          </rect>
  
          <rect width="120" height="108" fill-opacity="0">
            <animate dur="0.01s" attributeName="width" values="120; 0" fill="freeze" id="toggle" begin="click" />
            <animate dur="0.01s" attributeName="width" values="0; 120" fill="freeze" begin="reverseToggle.end" />
          </rect>
          <rect width="0" height="108" fill-opacity="0">
            <animate dur="0.001s" attributeName="width" values="120; 0" fill="freeze" id="reverseToggle" begin="click" />
            <animate dur="0.001s" attributeName="width" values="0; 120" begin="toggle.end" fill="freeze"  />
          </rect>
        </svg>
      </div>
    </div>
    <div>
      
      <div class="wrapper animation-api">
        <span class="stick"></span>
        <span class="stick"></span>
        <span class="stick"></span>
      </div>
    </div>
    <div>
      
      <div class="wrapper animation-api-next">
        <span class="stick"></span>
        <span class="stick"></span>
        <span class="stick"></span>
      </div>
    </div>
  </div>

 