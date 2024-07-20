
<div class="progress-container">

  <div class="neon-progress" style="--value: 60; --color: #43ec63;">
    <div class="circle"></div>
    <div class="label">Python</div>
    <div class="percentage">60%</div>
  </div>

  <div class="neon-progress" style="--value: 25; --color: #ffd700;">
    <div class="circle"></div>
    <div class="label">JavaScript</div>
    <div class="percentage">25%</div>
  </div>

  <div class="neon-progress" style="--value: 10; --color: #ff007f;">
    <div class="circle"></div>
    <div class="label">C++</div>
    <div class="percentage">10%</div>
  </div>

  <div class="neon-progress" style="--value: 5; --color: #ffffff;">
    <div class="circle"></div>
    <div class="label">Other</div>
    <div class="percentage">5%</div>
  </div>
  
</div>

<style>
  .progress-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
    margin: 20px;
  }

  .neon-progress {
    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;
    margin: 10px;
  }

  .circle {
    --size: 100px;
    --bg: #222;
    width: var(--size);
    height: var(--size);
    border-radius: 50%;
    background: conic-gradient(var(--color) calc(var(--value) * 1%), var(--bg) 0);
    position: relative;
    box-shadow: 0 0 15px var(--color), 0 0 30px var(--color);
  }

  .circle::before {
    content: "";
    position: absolute;
    width: 80%;
    height: 80%;
    background: var(--bg);
    border-radius: 50%;
    top: 10%;
    left: 10%;
  }

  .percentage {
    font-size: 1.2em;
    color: #fff;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 1;
  }

  .label {
    margin-top: 10px;
    color: var(--color);
    font-size: 1em;
    text-shadow: 0 0 5px var(--color), 0 0 10px var(--color);
  }
</style>
