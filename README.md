<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Donation Gallery</title>

  <!-- Swiper CSS -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />

  <style>
    body {
      margin: 0;
      font-family: sans-serif;
      background-color: #304674;
      color: white;
    }

    .header {
      text-align: center;
      padding: 20px;
      font-size: 1.5rem;
      font-weight: bold;
    }

    .swiper {
      width: 100%;
      height: auto;
      padding-bottom: 30px;
    }

    .swiper-slide {
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #1e2b4a;
      border-radius: 10px;
      margin: 10px;
    }

    .swiper-slide img {
      width: 90%;
      max-height: 300px;
      object-fit: contain;
      border-radius: 10px;
    }

    .swiper-pagination {
      text-align: center;
    }

    @media (max-width: 600px) {
      .header {
        font-size: 1.2rem;
      }
    }
  </style>
</head>
<body>

  <div class="header">Gifts Given in the Past</div>

  <!-- Swiper -->
  <div class="swiper">
    <div class="swiper-wrapper">
      <div class="swiper-slide">
        <img src="https://drive.google.com/uc?export=view&id=13aCX9wuir9R2uLr4CIbY6tNuRvsJ1_hG" alt="Image 1" />
      </div>
      <div class="swiper-slide">
        <img src="https://drive.google.com/uc?export=view&id=1aZfVBZGUHpPlSSabichf_6VlYp0QWWsn" alt="Image 2" />
      </div>
      <div class="swiper-slide">
        <img src="https://drive.google.com/uc?export=view&id=15D2HE7S6-znCSK3z9UMZM_12HViCriYn" alt="Image 3" />
      </div>
    </div>
    <!-- Add Pagination -->
    <div class="swiper-pagination"></div>
  </div>

  <!-- Swiper JS -->
  <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>

  <script>
    const swiper = new Swiper('.swiper', {
      loop: true,
      pagination: {
        el: '.swiper-pagination',
        clickable: true,
      },
    });
  </script>
</body>
</html>
