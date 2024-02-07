<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Drum Machine</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    button {
      font-size: 16px;
      margin: 5px;
      padding: 10px 20px;
    }
  </style>
</head>
<body>

<script>
  // Function to play drum sound
  function playDrumSound(sound) {
    const audio = new Audio(`path/to/${sound}.mp3`);
    audio.play();
  }

  // Function to handle button click
  function handleButtonClick(sound) {
    playDrumSound(sound);
  }

  // Event listeners for each drum button
  document.getElementById('kick').addEventListener('click', () => handleButtonClick('kick'));
  document.getElementById('snare').addEventListener('click', () => handleButtonClick('snare'));
  document.getElementById('hihat').addEventListener('click', () => handleButtonClick('hihat'));
</script>

<!-- Drum buttons -->
<button id="kick">Kick</button>
<button id="snare">Snare</button>
<button id="hihat">Hi-Hat</button>

</body>
</html>
