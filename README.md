# Welcome
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <title>Toko Minuman Coklat</title>
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background: #fdf6f0;
      color: #333;
    }
    header {
      background: #4E342E;
      color: white;
      padding: 20px 10px;
      text-align: center;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
    }
    nav {
      background: #6D4C41;
      padding: 12px 0;
      text-align: center;
    }
    nav a {
      margin: 0 20px;
      color: white;
      text-decoration: none;
      font-weight: bold;
      font-size: 16px;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #FFD180;
    }
    section {
      padding: 30px 20px;
      max-width: 800px;
      margin: auto;
      display: none;
      animation: fadeIn 0.5s ease-in;
    }
    section.active {
      display: block;
    }
    .product {
      background: #fff;
      border: 1px solid #ddd;
      padding: 15px;
      margin-bottom: 15px;
      cursor: pointer;
      border-radius: 8px;
      transition: background 0.3s;
    }
    .product:hover {
      background: #f1e1d0;
    }
    .product-detail {
      background: #fff9f5;
      border-left: 5px solid #A1887F;
      padding: 15px;
      margin-bottom: 20px;
      border-radius: 5px;
      display: none;
    }
    .product-detail img {
      max-width: 100%;
      height: auto;
      margin-top: 10px;
      border-radius: 6px;
      box-shadow: 0 2px 6px rgba(0, 0, 0, 0.15);
    }
    .whatsapp-button {
      color: white;
      background-color: #43A047;
      padding: 8px 16px;
      border-radius: 5px;
      text-decoration: none;
      display: inline-block;
      margin-top: 10px;
    }
    .whatsapp-button:hover {
      background-color: #388E3C;
    }
    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(10px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
  </style>
  <script>
    function showPage(pageId) {
      const sections = document.querySelectorAll("section");
      sections.forEach((sec) => sec.classList.remove("active"));
      document.getElementById(pageId).classList.add("active");
      if (pageId === "produk") {
        const details = document.querySelectorAll(".product-detail");
        details.forEach((d) => (d.style.display = "none"));
      }
    }

    function showProductInfo(productId) {
      const allProducts = document.querySelectorAll(".product-detail");
      allProducts.forEach((p) => (p.style.display = "none"));
      document.getElementById(productId).style.display = "block";
    }

    window.onload = () => showPage("profil");
  </script>
</head>
<body>
  <header>
    <h1>Toko Minuman Coklat Puname</h1>
    <p>Nikmati sensasi coklat premium dalam setiap tegukan!</p>
  </header>

  <nav>
    <a href="#" onclick="showPage('profil'); return false;">Profil</a>
    <a href="#" onclick="showPage('produk'); return false;">Produk</a>
    <a href="#" onclick="showPage('cara'); return false;">Cara Pemesanan</a>
    <a href="#" onclick="showPage('kontak'); return false;">Kontak</a>
  </nav>

  <section id="profil" style="max-width:900px; margin:auto; padding:30px 20px; background:#FFF8F0; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.1);">

  <h2 style="text-align:center; color:#4E342E; margin-bottom:30px; font-size:2rem;">Tentang Kami</h2>

  <div style="display:flex; flex-wrap:wrap; gap:30px; align-items:center; justify-content:center;">
    <img src="https://www.waralabaku.com/logo/logo_franchise_peluang_usaha_minuman_coklat_serius.jpg" 
         alt="Minuman Coklat" 
         style="flex:1 1 320px; max-width:320px; border-radius:16px; box-shadow: 0 8px 20px rgba(0,0,0,0.15);" />

    <div style="flex:2 1 400px; color:#5D4037; font-size:1.1rem; line-height:1.6;">
      <p><strong>Toko Minuman Coklat</strong> berdiri sejak 2023, menghadirkan minuman coklat berkualitas dengan resep rahasia dan bahan premium.</p>
      <p>Kami berkomitmen memberikan pengalaman minuman yang tak hanya lezat, tapi juga sehat dan segar untuk semua kalangan.</p>

      <div style="display:grid; grid-template-columns: repeat(auto-fit,minmax(140px,1fr)); gap:15px; margin-top:20px;">
        <div style="background:#6D4C41; color:#FFF3E0; padding:15px; border-radius:12px; text-align:center; box-shadow: 0 4px 10px rgba(109,76,65,0.4);">
            <div style="font-size:2rem;">💸</div>
            <p>Murah di Kantong</p>
          </div>
        <div style="background:#6D4C41; color:#FFF3E0; padding:15px; border-radius:12px; text-align:center; box-shadow: 0 4px 10px rgba(109,76,65,0.4);">
          <div style="font-size:2rem;">⚡</div>
          <p>Pengiriman Cepat</p>
        </div>
        <div style="background:#6D4C41; color:#FFF3E0; padding:15px; border-radius:12px; text-align:center; box-shadow: 0 4px 10px rgba(109,76,65,0.4);">
          <div style="font-size:2rem;">💯</div>
          <p>100% Kepuasan</p>
        </div>
        <div style="background:#6D4C41; color:#FFF3E0; padding:15px; border-radius:12px; text-align:center; box-shadow: 0 4px 10px rgba(109,76,65,0.4);">
          <div style="font-size:2rem;">🏆</div>
          <p>Produk Terpercaya</p>
        </div>
      </div>

      <blockquote style="margin-top:25px; font-style:italic; border-left: 4px solid #A1887F; padding-left:15px; color:#6D4C41;">
        "Minuman coklat yang sangat enak dan membuat hari saya jadi lebih cerah! Pelayanan juga cepat dan ramah." <br><strong>- Rani, Pelanggan Setia</strong>
      </blockquote>
    </div>
  </div>
</section>


  <section id="produk">
    <h2 style="text-align:center;">🍹 Pilih Minuman Coklat Favoritmu!</h2>
    <p style="text-align:center; font-size:16px; color:#6D4C41;">Rasa coklat yang lumer di mulut, segar dinikmati kapan saja! Klik untuk melihat detailnya.</p>

    <div class="product" onclick="showProductInfo('coklatOriginal')">🍫 <strong>Es Coklat Original</strong><br><small>Rasa klasik yang tak pernah salah!</small></div>
    <div class="product" onclick="showProductInfo('coklatOreo')">🍪 <strong>Es Coklat Oreo</strong><br><small>Dengan biskuit renyah di dalamnya!</small></div>
    <div class="product" onclick="showProductInfo('coklatKeju')">🧀 <strong>Es Coklat Keju</strong><br><small>Paduan manis & gurih yang unik!</small></div>

    <div id="coklatOriginal" class="product-detail">
      <h3>🍫 Es Coklat Original</h3>
      <p>Minuman coklat klasik dengan rasa autentik dan kesegaran alami, cocok untuk semua kalangan.</p>
      <p style="color:#D84315;"><strong>Harga: Rp 15.000</strong></p>
      <img src="https://static.promediateknologi.id/crop/0x0:0x0/0x0/webp/photo/p2/81/2024/09/10/WhatsApp-Image-2024-09-10-at-165729_d20ecc5b-3061382257.jpg" alt="Es Coklat Original" />
      <p><a href="https://wa.me/6285179764812?text=Halo%2C%20saya%20ingin%20pesan%20Es%20Coklat%20Original" target="_blank" class="whatsapp-button">Pesan Sekarang via WhatsApp</a></p>
    </div>

    <div id="coklatOreo" class="product-detail">
      <h3>🍪 Es Coklat Oreo</h3>
      <p>Perpaduan coklat creamy dengan potongan biskuit Oreo yang crunchy dan nikmat.</p>
      <p style="color:#D84315;"><strong>Harga: Rp 18.000</strong></p>
      <img src="https://www.dapurkintamani.com/wp-content/uploads/2021/06/oreo-milkshake.webp" alt="Es Coklat Oreo" />
      <p><a href="https://wa.me/6285179764812?text=Halo%2C%20saya%20ingin%20pesan%20Es%20Coklat%20Original" target="_blank" class="whatsapp-button">Pesan Sekarang via WhatsApp</a></p>
    </div>

    <div id="coklatKeju" class="product-detail">
      <h3>🧀 Es Coklat Keju</h3>
      <p>Coklat lembut dengan topping keju premium yang lumer di mulut, favorit pelanggan kami!</p>
      <p style="color:#D84315;"><strong>Harga: Rp 10.000</strong></p>
      <img src="https://i0.wp.com/i.gojekapi.com/darkroom/gofood-indonesia/v2/images/uploads/7d77ad0f-4762-407d-9f73-ed8d9d39873f_Go-Biz_20230218_125110.jpeg" alt="Es Coklat Keju" />
      <p><a href="https://wa.me/6285179764812?text=Halo%2C%20saya%20ingin%20pesan%20Es%20Coklat%20Original" target="_blank" class="whatsapp-button">Pesan Sekarang via WhatsApp</a></p>
    </div>
  </section>

  <section id="cara">
    <h2>🛒 Cara Pemesanan</h2>
    <ol>
      <li>
        <strong>Pilih minuman favoritmu</strong> dari daftar varian yang tersedia di halaman <em>Produk</em>.
      </li>
      <li>
        <strong>Hubungi kami via WhatsApp</strong> melalui tombol kontak yang tersedia.
        Sampaikan varian dan jumlah pesanan kamu.
      </li>
      <li>
        Tim kami akan mengkonfirmasi <strong>total pembayaran</strong> sesuai pesananmu (termasuk ongkir jika ada).
      </li>
      <li>
        Lakukan pembayaran melalui <strong>transfer bank</strong> yang akan kami informasikan.
      </li>
      <li>
        Setelah pembayaran diterima, pesananmu akan segera kami proses dan kirim ke alamat tujuan. 🚚✨
      </li>
    </ol>
    <p style="margin-top: 20px; background: #fff0e6; padding: 15px; border-left: 4px solid #FF8A65; border-radius: 5px;">
      💡 <strong>Catatan:</strong> Setelah melakukan pemesanan, kamu akan menerima rincian <strong>total pembayaran</strong> melalui chat WhatsApp. Pastikan untuk memeriksa kembali agar tidak ada yang terlewat, ya!
    </p>
  </section>

 <section id="kontak" style="max-width:600px; margin:auto; padding:30px 20px; background:#FFF3E0; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.1);">
  <h2 style="text-align:center; color:#4E342E; margin-bottom:25px;">📞 Hubungi Kami</h2>

  <div style="display:flex; flex-direction: column; gap:20px; font-size:18px; color:#5D4037;">

    <a href="https://wa.me/6285179764812?text=Halo%2C%20saya%20ingin%20pesan%20Es%20Coklat%20Original" target="_blank" rel="noopener noreferrer" 
       style="display:flex; align-items:center; gap:12px; background:#25D366; color:white; text-decoration:none; padding:12px 20px; border-radius:8px; font-weight:bold; box-shadow: 0 3px 8px rgba(37, 211, 102, 0.6); transition: background 0.3s;">
      <img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" alt="WhatsApp" style="width:28px; height:28px;" />
      WhatsApp: 0812-3456-7890
    </a>

    <a href="https://instagram.com/tokocoklatkita" target="_blank" rel="noopener noreferrer" 
       style="display:flex; align-items:center; gap:12px; background:#C13584; color:white; text-decoration:none; padding:12px 20px; border-radius:8px; font-weight:bold; box-shadow: 0 3px 8px rgba(193, 53, 132, 0.6); transition: background 0.3s;">
      <img src="https://cdn-icons-png.flaticon.com/512/174/174855.png" alt="Instagram" style="width:28px; height:28px;" />
      Instagram: @tokocoklatkita
    </a>

    <a href="mailto:tokocoklatkita@gmail.com" 
       style="display:flex; align-items:center; gap:12px; background:#6D4C41; color:white; text-decoration:none; padding:12px 20px; border-radius:8px; font-weight:bold; box-shadow: 0 3px 8px rgba(109, 76, 65, 0.6); transition: background 0.3s;">
      <img src="https://cdn-icons-png.flaticon.com/512/732/732200.png" alt="Email" style="width:28px; height:28px;" />
      Email: tokocoklatkita@gmail.com
    </a>

  </div>
</section>

</body>
</html>
