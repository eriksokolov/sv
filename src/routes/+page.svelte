<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:global(body) {
  height: 100vh;
  display: grid;
  place-items: center;
  font-family: 'EB Garamond';
  font-weight:100;
  background-color: rgb(95,95,95);
}
:global(body)::after {
  content: '';
  position: fixed;
  inset: 0;
  background: rgba(0, 0, 0, 0.1); 
  z-index: 0;
  pointer-events: none;
}

.ScaleWrapper {
  transform: scale(1.5); 
  transform-origin: center center;
}

.Card {
  position: relative;
  padding-top: 1rem;
  padding: 0.5rem;
  height: 11rem;
  width: 19rem;
  background-color: #eae6db;
  box-shadow: 0 4px 4px rgba(5, 5, 5, 0.9);
  overflow: hidden;
  z-index: 0;
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100'><filter id='noiseFilter'><feTurbulence type='fractalNoise' baseFrequency='0.15' numOctaves='2' stitchTiles='stitch'/></filter><rect width='100' height='100' filter='url(%23noiseFilter)' opacity='0.1'/></svg>");
  background-repeat: repeat;
  transform: rotate(-1deg);
  border-radius: 1px;
}

.Head {
  position: absolute;
  top: 1rem;
  left: 1rem;
  right: 1rem;
  display: flex;
  justify-content: space-between;
  font-size: 0.8rem;
}

.Right-Head{
  display:flex;
  justify-items:end;
  flex-direction: column;
  align-items: flex-end;
}

.Head a {
  all: unset;
  cursor: pointer;
}

#at {
  font-size: 0.6rem;
}

.Small-Head {
  font-size: 0.6rem;
  text-align: center;
}

.Center {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}

#Center-head {
  font-size: 1.0rem;
}

#Center-tail {
  font-size: 0.8rem;
}

.Tail {
  position: absolute;
  bottom: 0.6rem;
  left: 1rem;
  right: 1rem;
  display: flex;
  justify-content: center;
  font-size: 0.6rem;
}
.Tail a{
  all: unset;
  cursor: pointer;
}

.Card p,
.Card a,
#Center-head,
#Center-tail {
  color: #000;
  text-shadow:
   1px 1px 1px #fff;
}
</style>

<div class="ScaleWrapper">
  <div class="Card">
    <div class="Head">
      <div class="Left-Head">
        <a href="mailto:21estankevich@gmail.com">21estankevich</a>
        <p id="at">@gmail.com</p>
      </div>
      <div class="Right-Head">
        <a href="https://github.com/erikstankevich">qwerik537</a>
        <p class="Small-Head">github.com</p>
      </div>
    </div>

    <div class="Center">
      <p id="Center-head"><strong>Erik SOKOLOV</strong></p>
      <p id="Center-tail">Network Engineer</p>
    </div>

    <div class="Tail">
      <a href="https://www.linkedin.com/in/erik-stankevich-046784363/">https://www.linkedin.com/in/erik-stankevich-046784363/</a>
    </div>
  </div>
</div>

<link href="https://fonts.googleapis.com/css2?family=EB+Garamond&display=swap" rel="stylesheet">
