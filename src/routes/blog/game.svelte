<div class="container">
    <div id="game" class="idjustify-center-flex-column">
        <div id="hud">
            <div id="hud-item">
              <p class="hud-prefix">
                Pregunta
              </p>
              <!-- svelte-ignore a11y-missing-content -->
              <h1 class="hud-main-text" id="questionCounter"></h1>
            </div>
            <div id="hud-item">
              <p class="hud-prefix">
                Puntuación
              </p>
              <h1 class="hud-main-text" id="score">
                0
              </h1>
            </div>
          </div>
        <h2 id="question">What is the answer to this questions?</h2>
        <div class="choice-container">
            <p class="choice-prefix">A</p>
            <p class="choice-text" data-number="1">Choice 1</p>
        </div>
        <div class="choice-container">
            <p class="choice-prefix">B</p>
            <p class="choice-text"data-number="2">Choice 2</p>
        </div>
        <div class="choice-container">
            <p class="choice-prefix">C</p>
            <p class="choice-text"data-number="3">Choice 3</p>
        </div>
        <div class="choice-container">
            <p class="choice-prefix">D</p>
            <p class="choice-text"data-number="4">Choice 4</p>
        </div>
    </div>
</div>
<script src="game.js"></script>