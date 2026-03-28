<!doctype html>
<html lang="id"> 
 <head> 
  <meta charset="UTF-8"> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <title>Jasa @KenzXiterz - Order Sekarang</title> 
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"> 
  <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial Black', Gadget, sans-serif;
        }

        body {
            min-height: 100vh;
            padding: 20px;
            color: white;
            /* Background Killua Zoldyck dengan efek 3D dan warna biru */
            background: linear-gradient(45deg, rgba(0, 40, 120, 0.9), rgba(0, 80, 180, 0.85)), 
                        url('https://images6.alphacoders.com/968/968385.jpg') no-repeat center center fixed;
            background-size: cover;
            /* Efek 3D pada background */
            perspective: 1200px;
            transform-style: preserve-3d;
            animation: bg3DMove 18s ease-in-out infinite alternate;
        }

        /* Animasi gerakan 3D background */
        @keyframes bg3DMove {
            0% {
                background-position: 0% 10%;
                transform: rotateY(-6deg) translateZ(5px);
            }
            33% {
                background-position: 25% 35%;
                transform: rotateY(-2deg) translateZ(15px);
            }
            66% {
                background-position: 75% 65%;
                transform: rotateY(2deg) translateZ(15px);
            }
            100% {
                background-position: 100% 90%;
                transform: rotateY(6deg) translateZ(5px);
            }
        }

        /* Lapisan overlay untuk memperkuat warna biru dan efek kedalaman */
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 70% 30%, rgba(0, 120, 255, 0.3), rgba(0, 20, 80, 0.9));
            z-index: -1;
        }

        .container {
            max-width: 600px;
            margin: 0 auto;
            transform-style: preserve-3d;
            transform: translateZ(35px);
            transition: all 0.7s ease;
            opacity: 1;
        }

        .container:hover {
            transform: translateZ(50px);
        }

        /* Header Section */
        .header {
            text-align: center;
            margin-bottom: 30px;
            padding: 20px;
            background: rgba(0, 0, 0, 0.7);
            border-radius: 20px;
            border: 3px solid rgba(0, 180, 255, 0.8);
            box-shadow: 0 0 30px rgba(0, 150, 255, 0.6);
            transform-style: preserve-3d;
            transform: translateZ(20px);
        }

        .profile-img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border: 3px solid #00e5ff;
            margin-bottom: 15px;
            object-fit: cover;
            box-shadow: 0 0 20px rgba(0, 220, 255, 0.9);
            /* Ganti gambar profil dengan foto Killua juga */
            content: url('https://cdn-icons-png.flaticon.com/512/965/965928.png');
        }

        .username {
            font-size: 24px;
            margin-bottom: 10px;
            color: #00e5ff;
            text-shadow: 0 0 10px rgba(0, 220, 255, 0.9);
        }

        .promo-text {
            background-color: rgba(0, 20, 60, 0.9);
            padding: 12px;
            border-radius: 10px;
            font-size: 16px;
            margin-bottom: 20px;
            line-height: 1.5;
            border: 2px solid #00e5ff;
            box-shadow: 0 0 15px rgba(0, 220, 255, 0.6);
            color: white;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 25px;
            margin-bottom: 25px;
        }

        .social-btn {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: rgba(0, 80, 180, 0.9);
            color: white;
            border: 2px solid #00e5ff;
            font-size: 22px;
            cursor: pointer;
            transition: all 0.4s ease;
            box-shadow: 0 0 12px rgba(0, 220, 255, 0.7);
            transform-style: preserve-3d;
        }

        .social-btn:hover {
            transform: scale(1.15) translateZ(10px);
            background-color: #00e5ff;
            color: #002a5a;
            box-shadow: 0 0 25px rgba(0, 220, 255, 1);
        }

        /* Product Grid */
        .product-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            margin-bottom: 35px;
        }

        .product-item {
            background-color: rgba(0, 0, 0, 0.75);
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            cursor: pointer;
            border: 2px solid transparent;
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.6);
            transform-style: preserve-3d;
        }

        .product-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, rgba(0, 220, 255, 0.2), transparent);
            z-index: 0;
        }

        .product-item.active {
            border-color: #00e5ff;
            background-color: rgba(0, 30, 90, 0.95);
            box-shadow: 0 0 20px rgba(0, 220, 255, 0.9);
            transform: translateY(-6px) translateZ(15px);
        }

        .product-item * {
            position: relative;
            z-index: 1;
        }

        .product-name {
            font-size: 16px;
            margin-bottom: 8px;
            text-transform: uppercase;
            color: #ffffff;
            text-shadow: 0 0 8px rgba(0, 220, 255, 0.7);
        }

        .product-price {
            font-size: 14px;
            color: #00ffd6;
            font-weight: bold;
            text-shadow: 0 0 8px rgba(0, 255, 210, 0.9);
        }

        /* Order Form */
        .order-form {
            background-color: rgba(0, 0, 0, 0.75);
            padding: 25px;
            border-radius: 15px;
            margin-bottom: 30px;
            border: 3px solid rgba(0, 180, 255, 0.8);
            box-shadow: 0 0 30px rgba(0, 150, 255, 0.6);
            transform-style: preserve-3d;
            transform: translateZ(25px);
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-size: 16px;
            color: #00e5ff;
            text-shadow: 0 0 8px rgba(0, 220, 255, 0.7);
        }

        .form-control {
            width: 100%;
            padding: 12px;
            border-radius: 8px;
            border: 2px solid #00e5ff;
            font-size: 16px;
            background-color: rgba(0, 20, 60, 0.9);
            color: white;
            box-shadow: inset 0 0 8px rgba(0, 220, 255, 0.6);
            transition: all 0.3s ease;
        }

        .form-control::placeholder {
            color: rgba(200, 240, 255, 0.8);
        }

        .form-control:focus {
            outline: none;
            background-color: rgba(0, 30, 90, 0.9);
            box-shadow: inset 0 0 10px rgba(0, 220, 255, 0.8), 0 0 10px rgba(0, 220, 255, 0.5);
        }

        .submit-btn {
            width: 100%;
            padding: 15px;
            border-radius: 10px;
            border: none;
            background: linear-gradient(45deg, #0088ff, #00e5ff);
            color: #002a5a;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.4s ease;
            text-transform: uppercase;
            box-shadow: 0 0 18px rgba(0, 220, 255, 0.9);
            transform-style: preserve-3d;
        }

        .submit-btn:hover {
            background: linear-gradient(45deg, #00e5ff, #00ffff);
            transform: translateY(-3px) translateZ(10px);
            box-shadow: 0 0 30px rgba(0, 220, 255, 1);
        }

        /* Alert */
        .alert {
            padding: 12px;
            border-radius: 8px;
            margin-bottom: 20px;
            text-align: center;
            display: none;
            border: 2px solid;
            text-shadow: 0 0 8px rgba(0, 0, 0, 0.8);
            transform-style: preserve-3d;
            transform: translateZ(10px);
        }

        .alert.show {
            display: block;
        }

        .alert.success {
            background-color: rgba(0, 200, 120, 0.7);
            color: white;
            border-color: #00ff9d;
            box-shadow: 0 0 15px rgba(0, 255, 150, 0.7);
        }

        .alert.error {
            background-color: rgba(200, 60, 60, 0.7);
            color: white;
            border-color: #ff4444;
            box-shadow: 0 0 15px rgba(255, 100, 100, 0.7);
        }

        /* Footer */
        .footer {
            text-align: center;
            font-size: 14px;
            opacity: 0.9;
            margin-top: 20px;
            padding: 15px;
            background: rgba(0, 0, 0, 0.7);
            border-radius: 10px;
            border: 2px solid #00e5ff;
            color: #00e5ff;
            text-shadow: 0 0 8px rgba(0, 220, 255, 0.7);
            transform-style: preserve-3d;
            transform: translateZ(15px);
        }

        /* Animasi masuk halaman */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateZ(35px) translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateZ(35px) translateY(0);
            }
        }

        /* Responsif */
        @media (max-width: 400px) {
            .product-grid {
                grid-template-columns: 1fr;
            }

            body {
                animation: bg3DMove 25s ease-in-out infinite alternate;
            }
        }
    </style> 
 </head> 
 <body> 
  <div class="container"> <!-- Header --> 
   <div class="header"> 
    <img src="https://via.placeholder.com/100" alt="Profile @KenzXiterz" class="profile-img"> 
    <div class="username">
     @KenzXiterz
    </div> 
    <div class="promo-text"> 
    </div> 
    <div class="social-links"> <button class="social-btn"><i class="fab fa-youtube"></i></button> <button class="social-btn" onclick="openWhatsAppDirect()"><i class="fab fa-whatsapp"></i></button> <button class="social-btn"><i class="fab fa-tiktok"></i></button> 
    </div> 
   </div> <!-- Alert --> 
   <div id="alertBox" class="alert"></div> <!-- Product Grid --> 
   <div class="product-grid" id="productGrid"> 
    <div class="product-item" data-name="ETD Fanatical V1 " data-price="10000"> 
     <div class="product-name">
      ETD Fanatical V1
     </div> 
     <div class="product-price">
      IDR 10,000
     </div> 
    </div> 
    <div class="product-item" data-name="ETD Fanatical V2" data-price="20000"> 
     <div class="product-name">
      ETD Fanatical V2
     </div> 
     <div class="product-price">
      IDR 15,000
     </div> 
    </div> 
    <div class="product-item" data-name="ETD FanaticalV3 data-price=" 40000"> 
     <div class="product-name">
      ETD Fanatical V3
     </div> 
     <div class="product-price">
      IDR 25,000
     </div> 
    </div> 
    <div class="product-item" data-name="ETD Fanatical V4" data-price="50000"> 
     <div class="product-name">
      ETD Fanatical V4
     </div> 
     <div class="product-price">
      IDR 35,000
     </div> 
    </div> 
    <div class="product-item" data-name="ETD Fanatical V5" data-price="700
                        </div>
            <div class=" product-item"> 
     <div class="product-name">
      ETD Fanatical V5
     </div> 
     <div class="product-price">
      IDR 45,000
     </div> 
    </div> 
    <div class="product-item" data-name="HEADLOCK 30%" data-price="20000"> 
     <div class="product-name">
      HEADLOCK 30%
     </div> 
     <div class="product-price">
      IDR 20,000
     </div> 
    </div> 
    <div class="product-item" data-name="HEADLOCK 40%" data-price="30000"> 
     <div class="product-name" headlock 40%>
      HEADLOCK 40%
     </div> 
     <div class="product-price">
      IDR 30,000
     </div> 
    </div> 
    <div class="product-item" data-name="HEADLOCK 50%" data-price="40000"> 
     <div class="product-name">
      HEADLOCK 50%
     </div> 
     <div class="product-price">
      IDR 40,000
     </div> 
    </div> 
    <div class="product-item" data-name="HEADLOCK 65%" data-price="50000"> 
     <div class="product-name">
      HEADLOCK 65%
     </div> 
     <div class="product-price">
      IDR 45,000
     </div> 
    </div> 
    <div class="product-item" data-name="HEADLOCK 80%" data-price="5000"> 
     <div class="product-name">
      HEADLOCK 80%
     </div> 
     <div class="product-price">
      IDR 50,000
     </div> 
    </div> 
    <div class="product-item" data-name="INJEC PANEL TOXIC V10" data-price="15000"> 
     <div class="product-name">
      INJEC PANEL TOXIC V10
     </div> 
     <div class="product-price">
      IDR 50,000
     </div> 
    </div> 
    <div class="product-item" data-name="FFX TOOLS + MOD MENU" data-price="25000"> 
     <div class="product-name">
      FFX TOOLS + MOD MENU
     </div> 
     <div class="product-price">
      IDR 55,000
     </div> 
    </div> 
   </div> <!-- Order Form --> 
   <form id="orderForm" class="order-form"> 
    <div class="form-group"> <label for="namaPembeli">NAMA KAMU</label> 
     <input type="text" id="namaPembeli" class="form-control" placeholder="Contoh: kenz" required> 
    </div> 
    <div class="form-group"> <label for="noHpPembeli">NOMOR HP KAMU</label> 
     <input type="tel" id="noHpPembeli" class="form-control" placeholder="Contoh: 081234567890" required> 
    </div> 
    <div class="form-group"> <label for="jumlahProduk">JUMLAH PESANAN</label> 
     <input type="number" id="jumlahProduk" class="form-control" min="1" value="1" required> 
    </div> 
    <div class="form-group"> <label for="pesanTambahan">PESAN / CATATAN (Opsional)</label> <textarea id="pesanTambahan" class="form-control" placeholder="Contoh: halo bang Kenz aku mau beli"></textarea> 
    </div> <button type="submit" class="submit-btn"> <i class="fab fa-whatsapp"></i> ORDER SEKARANG </button> 
   </form> <!-- Footer --> 
   <div class="footer">
     made with KENZ | © 2026 @KenzXiterz | THEME KILLUA ZOLDYCK 3D 
   </div> 
  </div> 
  <script>
        // Nomor WhatsApp tujuan (diformat sesuai standar)
        const nomorWA = "6281234567890";
        
        // Ambil elemen
        const productGrid = document.getElementById('productGrid');
        const orderForm = document.getElementById('orderForm');
        const alertBox = document.getElementById('alertBox');
        let selectedProduct = null;

        // Fungsi tampilkan alert
        function showAlert(message, isSuccess) {
            alertBox.textContent = message;
            alertBox.className = `alert ${isSuccess ? 'success' : 'error'} show`;
            setTimeout(() => {
                alertBox.className = 'alert';
            }, 5000);
        }

        // Fungsi pilih produk
        productGrid.addEventListener('click', (e) => {
            const item = e.target.closest('.product-item');
            if (item) {
                // Hapus status aktif dari produk lain
                document.querySelectorAll('.product-item').forEach(p => p.classList.remove('active'));
                // Tambah status aktif ke produk yang dipilih
                item.classList.add('active');
                selectedProduct = {
                    name: item.dataset.name,
                    price: item.dataset.price
                };
                showAlert(`Produk ${selectedProduct.name} berhasil dipilih!`, true);
            }
        });

        // Fungsi buka WhatsApp langsung
        function openWhatsAppDirect() {
            const pesan = encodeURIComponent("Halo @KenzXiterz, saya mau nanya tentang jasa kamu dong!");
            window.open(`https://wa.me/${nomorWA}?text=${pesan}`, '_blank');
        }

        // Fungsi kirim pesanan ke WhatsApp
        orderForm.addEventListener('submit', (e) => {
            e.preventDefault();
            
            // Cek apakah produk sudah dipilih
            if (!selectedProduct) {
                showAlert("Woi pilih produk dulu dong gan!", false);
                return;
            }

            // Ambil data dari form
            const nama = document.getElementById('namaPembeli').value.trim();
            const noHp = document.getElementById('noHpPembeli').value.trim();
            const jumlah = document.getElementById('jumlahProduk').value;
            const pesan = document.getElementById('pesanTambahan').value.trim();

            // Hitung total harga
            const totalHarga = selectedProduct.price * jumlah;
            const hargaFormat = new Intl.NumberFormat('id-ID', { style: 'currency', currency: 'IDR' }).format(totalHarga);
            const hargaSatuanFormat = new Intl.NumberFormat('id-ID', { style: 'currency', currency: 'IDR' }).format(selectedProduct.price);

            // Susun pesan WhatsApp dengan tema Killua yang seru
            let pesanWA = encodeURIComponent(
                `⚡ HALOOO @KenzXiterz!!! AKU MAU ORDER NIH ⚡\n` +
                `══════════════════════════════════════\n` +
                `👤 DATA PEMBELI:\n` +
                `Nama: ${nama}\n` +
                `No HP: ${noHp}\n` +
                `══════════════════════════════════════\n` +
                `🛒 DETAIL PESANAN:\n` +
                `Produk: ${selectedProduct.name}\n` +
                `Jumlah: ${jumlah} buah\n` +
                `Harga Satuan: ${hargaSatuanFormat}\n` +
                `Total Harga: ${hargaFormat}\n` +
                `══════════════════════════════════════\n` +
                `💬 PESAN TAMBAHAN:\n` +
                `${pesan || 'Ga ada pesan tambahan kenz'}\n` +
                `══════════════════════════════════════\n` +
                `MOHON DI PROSES YA BANGGG! TERIMA KASIHH 🙏`
            );

            // Buka WhatsApp dengan pesan yang sudah jadi
            window.open(`https://wa.me/${nomorWA}?text=${pesanWA}`, '_blank');
            showAlert("Pesanan berhasil dibuat! Cek WA kamu dong kenz!", true);
            
            // Reset form dan pilihan produk
            orderForm.reset();
            document.querySelectorAll('.product-item').forEach(p => p.classList.remove('active'));
            selectedProduct = null;
        });

        // Animasi masuk saat halaman dibuka
        window.addEventListener('load', () => {
            const container = document.querySelector('.container');
            container.style.opacity = '0';
            container.style.transform = 'translateZ(35px) translateY(20px)';
            setTimeout(() => {
                container.style.transition = 'all 1s ease';
                container.style.opacity = '1';
                container.style.transform = 'translateZ(35px) translateY(0)';
            }, 300);
        });
    </script> 
 </body>
</html>
