<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Undangan Pernikahan - Sundus & Rofiud</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #f5fdf7;
      margin: 0;
      padding: 0;
      color: #2f3e2f;
    }
    header {
      background: linear-gradient(to right, #0b3d0b, #3b8d3b);
      color: white;
      text-align: center;
      padding: 2rem 1rem;
    }
    header h1 {
      font-size: 2.2rem;
      margin: 0;
    }
    header p {
      margin: 0.5rem 0 0;
    }
    section {
      padding: 2rem 1rem;
      text-align: center;
    }
    .names {
      font-size: 1.8rem;
      color: #0b3d0b;
      font-weight: bold;
    }
    .date-time {
      margin: 1rem 0;
      font-size: 1.2rem;
    }
    .location {
      margin: 1rem 0;
    }
    .map a {
      background: #3b8d3b;
      color: white;
      padding: 0.7rem 1.2rem;
      text-decoration: none;
      border-radius: 8px;
    }
    .countdown {
      margin: 2rem 0;
      font-size: 1.5rem;
      font-weight: bold;
    }
    footer {
      background-color: #0b3d0b;
      color: white;
      text-align: center;
      padding: 1rem;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>Undangan Pernikahan</h1>
    <p>Dengan penuh rasa syukur, kami mengundang Anda</p>
  </header>

  <section>
    <p class="names">Sundus Istiqomah <br>&amp;<br> M. Rofiud Darojat</p>

    <div class="date-time">
      <p><strong>Tanggal:</strong> 28 November 2025</p>
      <p><strong>Akad:</strong> 08.00 WIB</p>
      <p><strong>Resepsi:</strong> Waktu Bebas</p>
    </div>

    <div class="location">
      <p><strong>Tempat:</strong><br>
      Jl. STM Trisakti RT/RW:14/06, Dusun Talangan, Desa Gajahbendo, Beji Pasuruan</p>
    </div>

    <div class="map">
      <a href="https://maps.app.goo.gl/oF9b7N1xwugSq1VJ8" target="_blank">📍 Lihat di Google Maps</a>
    </div>

    <div class="countdown" id="countdown"></div>

    <p>Merupakan kehormatan dan kebahagiaan bagi kami apabila Bapak/Ibu/Saudara/i berkenan hadir untuk memberikan doa restu kepada kedua mempelai.</p>
  </section>

  <footer>
    <p>"Dan di antara tanda-tanda (kebesaran)-Nya ialah Dia menciptakan untukmu pasangan-pasangan dari jenismu sendiri, agar kamu merasa tenteram kepadanya, dan Dia menjadikan di antaramu rasa kasih dan sayang." (QS. Ar-Rum: 21)</p>
    <p>Hormat kami, <br> Keluarga Besar</p>
  </footer>

  <script>
    // Countdown Timer
    const countdown = document.getElementById("countdown");
    const weddingDate = new Date("Nov 28, 2025 08:00:00").getTime();

    const timer = setInterval(function() {
      const now = new Date().getTime();
      const distance = weddingDate - now;

      if (distance < 0) {
        clearInterval(timer);
        countdown.innerHTML = "Acara telah dimulai!";
        return;
      }

      const days = Math.floor(distance / (1000 * 60 * 60 * 24));
      const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((distance % (1000 * 60)) / 1000);

      countdown.innerHTML = `${days} Hari ${hours} Jam ${minutes} Menit ${seconds} Detik`;
    }, 1000);
  </script>
</body>
</html>

# Undangan-pernikahan
Undangan pernikahan Sundus dan Ovi
