# A.KPower
Original Songs by A.K Power listen and download for free (Enjoy!!!)
<!DOCTYPE html>
<html>
<head>
  <title>My Songs</title>
  <style>
    body { font-family: Arial, sans-serif; padding: 20px; background: #111; color: #fff; }
    h1 { text-align: center; }
    .track { margin: 15px 0; padding: 10px; background: #222; border-radius: 8px; }
    audio { width: 100%; }
  </style>
</head>
<body>
  <h1>My Songs</h1>
  <div id="playlist"></div>

  <script>
    // List your files here. Add/remove lines as you upload more.
    const songs = [
      "song1.mp3",
      "song2.mp3", 
      "song3.mp3"
    ];

    const playlistDiv = document.getElementById("playlist");

    songs.forEach(file => {
      const name = file.replace(".mp3", "").replace(/[-_]/g, " ");
      
      const trackDiv = document.createElement("div");
      trackDiv.className = "track";
      
      trackDiv.innerHTML = `
        <h3>${name}</h3>
        <audio controls>
          <source src="${file}" type="audio/mpeg">
        </audio>
      `;
      
      playlistDiv.appendChild(trackDiv);
    });
  </script>
</body>
</html>
