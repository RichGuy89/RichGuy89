<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday!</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    text-align: center;
    margin: 0;
    padding: 0;
    background-image: url('61sQDm1RVfL.jpg');
    background-size: cover;
    background-position: center;
  }
  .container {
    max-width: 800px;
    margin: 50px auto;
    padding: 20px;
    background-color: rgba(255, 255, 255, 0.9);
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
    border-radius: 10px;
  }
  h1 {
    color: #ff6347;
    font-size: 3em;
    margin-bottom: 20px;
  }
  .cake {
    max-width: 100%;
    height: auto;
    animation: floatCake 5s ease-in-out infinite alternate;
  }
  @keyframes floatCake {
    0% { transform: translateY(0); }
    100% { transform: translateY(-10px); }
  }
  .message {
    font-size: 1.5em;
    margin-bottom: 20px;
  }
  .button {
    display: inline-block;
    padding: 10px 20px;
    background-color: #ff6347;
    color: #fff;
    font-size: 1.2em;
    text-decoration: none;
    border-radius: 5px;
    transition: background-color 0.3s ease;
    margin-top: 20px;
  }
  .button:hover {
    background-color: #e55e3c;
  }
  .photo-gallery {
    margin-top: 30px;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
  }
  .photo-gallery img {
    max-width: 100%;
    height: auto;
    margin: 10px;
    border-radius: 5px;
    box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
    cursor: pointer;
  }
  .photo-gallery img:hover {
    transform: scale(1.1);
  }
</style>
</head>
<body>
  <div class="container">
    <h1>Happy Birthday!</h1>
    <img class="cake" src="C:\Users\SHEESHABLE\Desktop\Website\images.jpg" alt="Birthday Cake">
    <p class="message">Wishing you a fantastic day filled with joy and celebration!</p>
    <a href="#" class="button" id="playButton">Play Birthday Song</a>
    <audio id="birthdaySong">
      <source src="C:\Users\SHEESHABLE\Desktop\Website\Happy Birthday Song!!!.mp3" type="audio/mpeg">
      Your browser does not support the audio element.
    </audio>
    <div class="photo-gallery" id="photoGallery">
      <img src="C:\Users\SHEESHABLE\Desktop\Website\421919934_7894617333982065_4682099443175063670_n.jpg" alt="Photo 1">
      <img src="C:\Users\SHEESHABLE\Desktop\Website\448111982_1545762966283396_233147072179822202_n.jpg" alt="Photo 2">
      <img src="C:\Users\SHEESHABLE\Desktop\Website\449958870_1248996936509218_6477134905423943927_n.jpg" alt="Photo 3">
      <img src="C:\Users\SHEESHABLE\Desktop\Website\450757883_1013548340270220_8558210941013857835_n.jpg" alt="Photo 4">
      <img src="C:\Users\SHEESHABLE\Desktop\Website\451691290_846453846993136_1870461387252226597_n.jpg" alt="Photo 5">
    </div>
  </div>

  <script>
    // Play/pause birthday song functionality
    document.getElementById('playButton').addEventListener('click', function() {
      var audio = document.getElementById('birthdaySong');
      if (audio.paused) {
        audio.play();
        this.textContent = 'Pause Birthday Song';
      } else {
        audio.pause();
        audio.currentTime = 0;
        this.textContent = 'Play Birthday Song';
      }
    });

    // Photo gallery lightbox functionality
    const photos = document.querySelectorAll('.photo-gallery img');
    photos.forEach(photo => {
      photo.addEventListener('click', function() {
        // Create a lightbox overlay
        const overlay = document.createElement('div');
        overlay.style.position = 'fixed';
        overlay.style.top = '0';
        overlay.style.left = '0';
        overlay.style.width = '100%';
        overlay.style.height = '100%';
        overlay.style.backgroundColor = 'rgba(0,0,0,0.7)';
        overlay.style.zIndex = '9999';
        overlay.style.display = 'flex';
        overlay.style.justifyContent = 'center';
        overlay.style.alignItems = 'center';

        // Create the full-size image
        const fullImg = document.createElement('img');
        fullImg.src = photo.src;
        fullImg.style.maxWidth = '90%';
        fullImg.style.maxHeight = '90%';
        fullImg.style.borderRadius = '5px';

        // Append full-size image to overlay
        overlay.appendChild(fullImg);

        // Close overlay on click outside the image
        overlay.addEventListener('click', function(e) {
          if (e.target === overlay) {
            document.body.removeChild(overlay);
          }
        });

        // Append overlay to body
        document.body.appendChild(overlay);
      });
    });
  </script>
</body>
</html>
