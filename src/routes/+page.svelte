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
  background-color: rgba(41, 7, 5, 0.9);
}
:global(body)::after {
  content: '';
  position: fixed;
  inset: 0;
  background: rgba(0, 0, 0, 0.2); 
  z-index: 0;
  pointer-events: none;
}

.ScaleWrapper {
  transform: scale(1.5); 
  transform-origin: center center;
}

.Card {
  position: relative;
  padding: 1rem;
  height: 11rem;
  width: 19rem;
  background-color: #eae6db;
  box-shadow: 0 4px 4px rgba(0, 0, 0, 0.9);
  overflow: hidden;
  z-index: 0;
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100'><filter id='noiseFilter'><feTurbulence type='fractalNoise' baseFrequency='0.15' numOctaves='2' stitchTiles='stitch'/></filter><rect width='100' height='100' filter='url(%23noiseFilter)' opacity='0.07'/></svg>");
  background-repeat: repeat;
  transform: rotate(-1deg);
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

.Card p,
.Card a,
#Center-head,
#Center-tail {
  color: #3a2f1c;
  text-shadow:
    0.8px 0.8px 0 #c8c4ba,
   -0.8px -0.8px 0 #f5f2e7;
}
</style>

<div class="ScaleWrapper">
  <div class="Card">
    <div class="Head">
      <div class="Left-Head">
        <p>21estankevich</p>
        <p id="at">@gmail.com</p>
      </div>
      <div class="Right-Head">
        <a href="https://github.com/erikstankevich"><strong>Github</strong></a>
        <p class="Small-Head">QWERik</p>
      </div>
    </div>

    <div class="Center">
      <p id="Center-head"><strong>Erik SOKOLOV</strong></p>
      <p id="Center-tail">Network Engineer</p>
    </div>

    <div class="Tail">
      <p>Carl-von-Ossietky Str. 54, 65197 Wiesbaden</p>
    </div>
  </div>
</div>

<link href="https://fonts.googleapis.com/css2?family=EB+Garamond&display=swap" rel="stylesheet">
