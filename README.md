
<style>
  .progress-circle {
    --size: 100px;
    --bg: #eee;
    --fg: #00bfff;
    width: var(--size);
    height: var(--size);
    border-radius: 50%;
    background: conic-gradient(var(--fg) calc(var(--value) * 1%), var(--bg) 0);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.5em;
    position: relative;
  }

  .progress-circle span {
    position: absolute;
    font-size: 1.2em;
    color: #333;
  }
</style>


<div class="progress-circle" style="--value: 90;">
  <span>90%</span>
</div>

<div class="progress-circle" style="--value: 40;">
  <span>40%</span>
</div>



<img src="https://i1.wallbox.ru/wallpapers/main/201132/oboi-na-rabochiy-stol-krasivye-oboi-tekstura-dc76913.jpg" alt="Картинка" width=100% height=200>

