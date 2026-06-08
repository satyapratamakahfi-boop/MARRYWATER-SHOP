<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>Vito Haru | Jual Beli Jas Hitam Premium</title>
  <!-- Font Awesome 6 (Ikon keren) -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <!-- Google Fonts: Poppins & Inter -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,600;14..32,700&family=Poppins:wght@500;600;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: #f4f6fa;
      color: #1e1e2f;
      line-height: 1.5;
      scroll-behavior: smooth;
    }

    .container {
      max-width: 1280px;
      margin: 0 auto;
      padding: 0 24px;
    }

    /* Header & Brand */
    .navbar {
      background: #0a0c15;
      color: white;
      padding: 20px 0;
      border-bottom: 3px solid #d4af37;
      box-shadow: 0 8px 20px rgba(0,0,0,0.05);
    }

    .nav-flex {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      flex-wrap: wrap;
      gap: 16px;
    }

    .logo-area h1 {
      font-family: 'Poppins', sans-serif;
      font-size: 1.8rem;
      letter-spacing: -0.5px;
    }

    .logo-area p {
      font-size: 0.85rem;
      color: #b9c3d9;
      margin-top: 5px;
    }

    .vito-click {
      background: #252a3a;
      padding: 10px 20px;
      border-radius: 60px;
      cursor: pointer;
      transition: all 0.25s ease;
      display: inline-flex;
      align-items: center;
      gap: 12px;
      font-weight: 600;
      border: 1px solid #d4af37;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
    }

    .vito-click i {
      font-size: 1.2rem;
      color: #ffd966;
    }

    .vito-click:hover {
      background: #d4af37;
      color: #0a0c15;
      transform: scale(1.02);
      border-color: white;
    }

    .vito-click:hover i {
      color: #0a0c15;
    }

    /* headline */
    .hero {
      background: linear-gradient(135deg, #e9eef3 0%, #ffffff 100%);
      padding: 40px 0 30px;
      border-bottom: 1px solid #e2e8f0;
      text-align: center;
    }

    .hero h2 {
      font-size: 2rem;
      font-weight: 700;
      color: #111;
    }

    .hero span {
      background: #0a0c15;
      color: #d4af37;
      padding: 4px 12px;
      border-radius: 40px;
      font-size: 0.9rem;
      display: inline-block;
      margin-top: 12px;
    }

    /* Grid produk */
    .section-title {
      font-size: 1.8rem;
      font-weight: 700;
      margin: 40px 0 20px 0;
      position: relative;
      display: inline-block;
    }
    .section-title:after {
      content: '';
      position: absolute;
      bottom: -10px;
      left: 0;
      width: 60px;
      height: 4px;
      background: #d4af37;
      border-radius: 4px;
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
      gap: 30px;
      margin: 30px 0 40px;
    }

    .product-card {
      background: white;
      border-radius: 28px;
      overflow: hidden;
      transition: all 0.3s ease;
      box-shadow: 0 12px 24px -12px rgba(0,0,0,0.1);
      border: 1px solid #edf2f7;
    }

    .product-card:hover {
      transform: translateY(-6px);
      box-shadow: 0 24px 36px -16px rgba(0,0,0,0.2);
      border-color: #d4af37;
    }

    .product-img {
      background: #11131f;
      height: 200px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #e2c168;
    }

    .product-img i {
      font-size: 5rem;
      filter: drop-shadow(2px 4px 8px rgba(0,0,0,0.3));
    }

    .product-info {
      padding: 20px 18px 24px;
    }

    .product-title {
      font-size: 1.35rem;
      font-weight: 700;
      margin-bottom: 8px;
      color: #0a0c15;
    }

    .product-desc {
      font-size: 0.85rem;
      color: #4a5568;
      margin: 12px 0;
      line-height: 1.4;
    }

    .product-price {
      font-size: 1.6rem;
      font-weight: 800;
      color: #c49a2b;
      margin: 12px 0;
    }

    .product-price small {
      font-size: 0.8rem;
      font-weight: 500;
      color: #64748b;
    }

    .btn-buy {
      background: #0a0c15;
      color: white;
      border: none;
      width: 100%;
      padding: 12px 0;
      font-weight: 700;
      font-size: 1rem;
      border-radius: 40px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      cursor: pointer;
      transition: all 0.2s;
      margin-top: 8px;
      font-family: 'Inter', sans-serif;
    }

    .btn-buy i {
      font-size: 1rem;
    }

    .btn-buy:hover {
      background: #d4af37;
      color: #0a0c15;
      transform: scale(0.98);
    }

    /* JUAL FORM SECTION */
    .sell-section {
      background: #ffffffdd;
      backdrop-filter: blur(2px);
      background: linear-gradient(120deg, #f8fafc, #ffffff);
      border-radius: 40px;
      padding: 30px 28px;
      margin: 40px 0 60px;
      box-shadow: 0 8px 28px rgba(0,0,0,0.05);
      border: 1px solid #e9edf2;
    }

    .sell-title {
      font-size: 1.7rem;
      font-weight: 700;
      margin-bottom: 6px;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .sell-title i {
      color: #c49a2b;
    }

    .form-group {
      margin-bottom: 20px;
    }

    .form-group label {
      display: block;
      font-weight: 600;
      margin-bottom: 6px;
      color: #1e293b;
    }

    .form-group input, .form-group textarea {
      width: 100%;
      padding: 12px 16px;
      border-radius: 28px;
      border: 1.5px solid #e2e8f0;
      font-family: 'Inter', sans-serif;
      transition: 0.2s;
      background: white;
    }

    .form-group input:focus, .form-group textarea:focus {
      outline: none;
      border-color: #d4af37;
      box-shadow: 0 0 0 3px rgba(212,175,55,0.2);
    }

    .btn-sell {
      background: #1e293b;
      color: white;
      padding: 12px 32px;
      border: none;
      border-radius: 40px;
      font-weight: 700;
      font-size: 1rem;
      display: inline-flex;
      align-items: center;
      gap: 12px;
      cursor: pointer;
      transition: 0.2s;
    }

    .btn-sell:hover {
      background: #d4af37;
      color: #0f172a;
      transform: scale(1.02);
    }

    /* footer */
    .footer {
      background: #0a0c15;
      color: #94a3b8;
      text-align: center;
      padding: 28px 0;
      margin-top: 20px;
      border-top: 1px solid #2d3748;
    }

    .footer a {
      color: #d4af37;
      text-decoration: none;
    }

    .empty-msg {
      text-align: center;
      grid-column: 1/-1;
      padding: 40px;
      background: #f1f5f9;
      border-radius: 40px;
    }

    @media (max-width: 640px) {
      .nav-flex {
        flex-direction: column;
        align-items: flex-start;
      }
      .product-grid {
        gap: 20px;
      }
      .hero h2 {
        font-size: 1.6rem;
      }
    }
  </style>
</head>
<body>

<div class="navbar">
  <div class="container nav-flex">
    <div class="logo-area">
      <h1>🕴️ JAS HITAM <span style="color:#d4af37;">MARKET</span></h1>
      <p>Pusat Jual Beli Jas Hitam Premium & Eksklusif</p>
    </div>
    <div class="vito-click" id="vitoClickBtn">
      <i class="fas fa-crown"></i>
      <span>✨ VITO HARU ✨</span>
      <i class="fas fa-hand-pointer"></i>
    </div>
  </div>
</div>

<div class="hero">
  <div class="container">
    <h2>⚡ Jual & Beli Jas Hitam ⚡</h2>
    <p style="margin-top: 12px; max-width: 600px; margin-left: auto; margin-right: auto;">Koleksi terbaik dari berbagai model, mulai dari slim fit hingga double breasted. Transaksi mudah & terpercaya.</p>
    <span><i class="fas fa-tshirt"></i> 100% Original | Garansi Style</span>
  </div>
</div>

<div class="container">
  <!-- Produk Terdaftar -->
  <div>
    <div class="section-title">🔥 Daftar Jas Hitam</div>
    <div id="productContainer" class="product-grid">
      <!-- product cards akan di-render via JS -->
      <div class="empty-msg">Memuat koleksi terbaik...</div>
    </div>
  </div>

  <!-- Form JUAL Jas Hitam -->
  <div class="sell-section">
    <div class="sell-title">
      <i class="fas fa-store"></i>
      <h3>Jual Jas Hitam Anda</h3>
    </div>
    <p style="margin-bottom: 20px; color: #334155;">Ingin menjual jas hitam? Isi form di bawah, maka produk akan langsung tampil di daftar. Gratis!</p>
    <form id="sellForm">
      <div class="form-group">
        <label><i class="fas fa-tag"></i> Nama Jas *</label>
        <input type="text" id="productName" placeholder="cth: Jas Hitam Tuxedo Premium" required>
      </div>
      <div class="form-group">
        <label><i class="fas fa-money-bill-wave"></i> Harga (Rp) *</label>
        <input type="number" id="productPrice" placeholder="Harga dalam Rupiah" required>
      </div>
      <div class="form-group">
        <label><i class="fas fa-align-left"></i> Deskripsi Singkat</label>
        <textarea id="productDesc" rows="2" placeholder="Kondisi, ukuran, bahan, dll..."></textarea>
      </div>
      <button type="submit" class="btn-sell"><i class="fas fa-plus-circle"></i> Tawarkan Jual Sekarang</button>
    </form>
    <p style="margin-top: 18px; font-size: 0.75rem; color: #5b6e8c;"><i class="fas fa-info-circle"></i> Setelah ditambahkan, pembeli bisa langsung klik tombol "Beli" untuk menghubungi Vito Haru.</p>
  </div>
</div>

<div class="footer">
  <div class="container">
    <p>© 2025 <span style="color:#d4af37; font-weight:600;">Vito Haru's Black Suit Exchange</span> — Jual beli jas hitam terpercaya | <i class="fas fa-mobile-alt"></i> Hubungi via WhatsApp +62 812 3456 7890</p>
    <p style="margin-top: 8px; font-size: 0.75rem;">✨ Klik nama <strong>"Vito Haru"</strong> di atas untuk info kontak & layanan eksklusif ✨</p>
  </div>
</div>

<script>
  // Data awal produk jas hitam (list jual)
  let products = [
    {
      id: 1,
      name: "Jas Hitam Exclusive Wool",
      price: 1200000,
      description: "Bahan wool premium import, lining sutra, cocok untuk acara formal & gala dinner.",
    },
    {
      id: 2,
      name: "Jas Hitam Slim Fit Modern",
      price: 950000,
      description: "Model slim fit kekinian, ringan dan nyaman dipakai sehari-hari, tampil elegan.",
    },
    {
      id: 3,
      name: "Jas Hitam Double Breasted",
      price: 1500000,
      description: "Kesan klasik + maskulin, kancing ganda emas, bahan wol blend.",
    },
    {
      id: 4,
      name: "Jas Hitam Casual Linen",
      price: 800000,
      description: "Bahan linen adem, casual elegan untuk acara semi formal atau kondangan.",
    },
    {
      id: 5,
      name: "Jas Hitam Velvet Malam",
      price: 2100000,
      description: "Jas velvet hitam mewah, kilau elegan, cocok pesta malam & anniversary.",
    }
  ];

  // Helper: format Rupiah
  function formatRupiah(angka) {
    return new Intl.NumberFormat('id-ID', { style: 'currency', currency: 'IDR', minimumFractionDigits: 0 }).format(angka);
  }

  // Render semua produk ke dalam grid
  function renderProducts() {
    const container = document.getElementById('productContainer');
    if (!container) return;
    
    if (products.length === 0) {
      container.innerHTML = `<div class="empty-msg"><i class="fas fa-box-open"></i> Belum ada jas hitam yang dijual. jadi yang pertama jual jas mu! ✨</div>`;
      return;
    }
    
    let cardsHTML = '';
    products.forEach(product => {
      cardsHTML += `
        <div class="product-card" data-id="${product.id}">
          <div class="product-img">
            <i class="fas fa-user-tie"></i>
          </div>
          <div class="product-info">
            <div class="product-title">${escapeHtml(product.name)}</div>
            <div class="product-desc">${escapeHtml(product.description) || "Jas hitam kualitas terbaik, siap mempercantik penampilanmu."}</div>
            <div class="product-price">${formatRupiah(product.price)} <small> / unit</small></div>
            <button class="btn-buy buy-btn" data-name="${escapeHtml(product.name)}" data-price="${product.price}" data-id="${product.id}">
              <i class="fas fa-shopping-cart"></i> Beli Sekarang
            </button>
          </div>
        </div>
      `;
    });
    container.innerHTML = cardsHTML;
  }

  // fungsi sederhana untuk menghindari XSS
  function escapeHtml(str) {
    if (!str) return '';
    return str.replace(/[&<>]/g, function(m) {
      if (m === '&') return '&amp;';
      if (m === '<') return '&lt;';
      if (m === '>') return '&gt;';
      return m;
    }).replace(/[\uD800-\uDBFF][\uDC00-\uDFFF]/g, function(c) {
      return c;
    });
  }

  // Fungsi menambah produk baru (jual)
  function addNewProduct(name, price, description) {
    // validasi sederhana
    if (!name || name.trim() === "") {
      alert("❌ Nama jas tidak boleh kosong!");
      return false;
    }
    if (!price || isNaN(price) || Number(price) <= 0) {
      alert("❌ Harga harus diisi dengan angka positif!");
      return false;
    }
    const priceNum = Number(price);
    const newId = Date.now(); // ID unik berdasarkan timestamp
    const newProduct = {
      id: newId,
      name: name.trim(),
      price: priceNum,
      description: description && description.trim() !== "" ? description.trim() : "Jas hitam keren, siap dikirim ke seluruh Indonesia.",
    };
    products.unshift(newProduct); // tambahkan di awal biar langsung terlihat
    renderProducts();
    return true;
  }

  // EVENT DELEGATION: untuk tombol beli (produk statis / dinamis)
  function setupBuyEvent() {
    const container = document.getElementById('productContainer');
    if (!container) return;
    container.addEventListener('click', (e) => {
      const buyButton = e.target.closest('.buy-btn');
      if (!buyButton) return;
      
      // ambil data dari attribute button
      const productName = buyButton.getAttribute('data-name') || "Jas Hitam";
      const productPriceRaw = buyButton.getAttribute('data-price');
      let priceFormatted = "";
      if (productPriceRaw) {
        priceFormatted = formatRupiah(Number(productPriceRaw));
      }
      
      // Tampilkan pesan minat beli + mengarahkan ke Vito Haru (karena jual beli dikelola Vito)
      alert(`🕴️ MINAT BELI JAS HITAM 🕴️\n\nProduk: ${productName}\nHarga: ${priceFormatted}\n\n✅ Silakan lanjutkan transaksi dengan mengklik nama "VITO HARU" di pojok kanan atas untuk mendapatkan kontak resmi (WA/Telegram).\n\nAtau hubungi langsung Vito Haru via WhatsApp : +62 812 3456 7890\nTerima kasih telah berbelanja di Vito's Market!`);
    });
  }

  // Fungsi handle form jual jas
  function initSellForm() {
    const form = document.getElementById('sellForm');
    if (!form) return;
    form.addEventListener('submit', (e) => {
      e.preventDefault();
      const nameInput = document.getElementById('productName');
      const priceInput = document.getElementById('productPrice');
      const descInput = document.getElementById('productDesc');
      
      let name = nameInput.value;
      let price = priceInput.value;
      let desc = descInput.value;
      
      const success = addNewProduct(name, price, desc);
      if (success) {
        // reset form setelah berhasil
        nameInput.value = '';
        priceInput.value = '';
        descInput.value = '';
        // scroll sedikit ke daftar produk agar seller lihat hasilnya
        document.querySelector('.section-title')?.scrollIntoView({ behavior: 'smooth', block: 'start' });
        alert("✨ Jas hitam berhasil ditambahkan ke daftar jualan! Sekarang pembeli bisa lihat dan klik tombol beli ✨");
      }
    });
  }

  // FUNGSI KLIK NAMA VITO HARU (clickable)
  function initVitoClickable() {
    const vitoElement = document.getElementById('vitoClickBtn');
    if (vitoElement) {
      vitoElement.addEventListener('click', (e) => {
        e.preventDefault();
        // Menampilkan informasi kontak Vito Haru & layanan jual beli
        alert("👔 VITO HARU - Owner & Founder Black Suit Exchange 👔\n\n📞 Kontak Resmi:\n📱 WhatsApp: +62 812 3456 7890\n📧 Email: vito.haru@jashitam.id\n\n💼 Layanan: Jual Beli Jas Hitam (Baru/Second)\n📍 Fast response & negotiable.\n\n✨ Klik 'OK' untuk langsung chat via WhatsApp? (Simpan kontak)");
        // Bisa juga tambahan konfirmasi untuk membuka link WA (optional, lebih friendly)
        const userConfirm = confirm("Buka WhatsApp untuk terhubung dengan Vito Haru?");
        if (userConfirm) {
          window.open("https://wa.me/6281234567890?text=Halo%20Vito%20Haru,%20saya%20tertarik%20dengan%20jas%20hitam%20di%20marketplace%20Anda.", "_blank");
        }
      });
    }
  }

  // Tombol-tombol tambahan interaksi (syarat ada tombolnya sudah terpenuhi: tombol beli di setiap card, tombol jual, dan tombol virtual pada Vito)
  // Selain itu kita juga bisa menambahkan tombol sampel lain? Sudah cukup.
  
  // Inisialisasi halaman
  function init() {
    renderProducts();
    setupBuyEvent();     // event delegation untuk tombol beli
    initSellForm();      // form jual jas hitam
    initVitoClickable(); // nama vito haru bisa di pencet
    
    // Tambahan: Pesan sambutan bahwa tombol sudah tersedia (bonus)
    console.log("✅ Vito Haru's Market ready | Tombol Beli & Jual Aktif");
  }
  
  // jalankan saat DOM siap
  if (document.readyState === 'loading') {
    document.addEventListener('DOMContentLoaded', init);
  } else {
    init();
  }
</script>
</body>
</html>
