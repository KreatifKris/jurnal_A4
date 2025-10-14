
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BERITA TERKINI SMA PETRA 4 SIDOARJO</title>
    <!-- <link rel="stylesheet" href="bg.css"> -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 50%, #F97316 100%);
        }
        
        .news-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .news-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
        }
        
        .category-badge {
            transition: background-color 0.3s ease;
        }
        
        .category-badge:hover {
            background-color: #3b82f6;
        }
        
        .breaking-news {
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { background-color: #ef4444; }
            50% { background-color: #dc2626; }
            100% { background-color: #ef4444; }
        }

        /* Tambahan untuk logo sekolah di sebelah atas laman (top right) */
        .school-logo {
            height: 40px;
            width: auto;
        }

        .social-btn-gradient {
            background: linear-gradient(135deg, #3b82f6 0%, #ef4444 100%);
            border: none;
        }
        .social-btn-gradient:hover {
            background: linear-gradient(135deg, #2563eb 0%, #dc2626 100%);
        }
    </style>
</head>
<body class="bg-gray-100">
    <!-- Header -->
    <header class="bg-white shadow-md sticky top-0 z-50">
        <div class="container mx-auto px-4 py-4">
            <div class="flex items-center justify-between">
                <!-- Logo Kiri (Icon + Judul + Logo Sekolah) -->
                <div class="flex items-center">
                    <div class="w-10 h-10 bg-purple-600 rounded-lg flex items-center justify-center mr-3">
                        <i class="fas fa-newspaper text-white text-xl"></i>
                    </div>
                    <!-- Tambahan: Logo Sekolah di sebelah kiri atas (bisa diganti dengan path gambar asli) -->
                    <img src="logo.png" alt="Logo SMA Petra 4 Sidoarjo" class="school-logo mr-3">
                    <h1 class="text-2xl font-bold text-gray-800">Berita Terkini</h1>
                </div>

                <!-- Search, Mobile Menu, dan Logo Listing di Sebelah Atas Kanan -->
                <div class="flex items-center space-x-4">
                    <!-- Search -->
                    <div class="hidden md:flex items-center bg-gray-100 rounded-full px-4 py-2">
                        <i class="fas fa-search text-gray-500 mr-2"></i>
                        <input type="text" placeholder="Cari berita..." class="bg-transparent outline-none text-sm">
                    </div>
                    <!-- Tambahan: Listing Logo di Sebelah Atas Kanan (misalnya list ikon atau logo tambahan; di sini saya buat sebagai logo sekolah alternatif atau ikon list) -->
                    <div class="flex items-center space-x-2">
                        <img src="sekolah.png" alt="Listing Logo" class="school-logo rounded-full">
                        <span class="text-sm text-gray-600 hidden md:block">OUR NEWS IN SMA PETRA 4</span>
                    </div>
                    <button class="md:hidden text-gray-700">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
    </header>

    <!-- Breaking News Banner -->
    <div class="breaking-news bg-red-500 text-white py-2">
        <div class="container mx-auto px-4">
            <div class="flex items-center justify-center">
                <span class="font-bold mr-4 animate-pulse">Berita Panas</span>
                <marquee behavior="scroll" direction="left" class="text-sm">
                    Jurnalistik digital bersama tim jurnalistik SMA Petra 4 Sidoarjo
                </marquee>
            </div>
        </div>
    </div>

    <section id="news" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-gray-800 mb-4">Berita Terbaru</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Update Berita SMA Trafour</p>
            </div>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- News Card 1: ELS Desain Grafis -->
                <div class="news-card bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="relative">
                        <img src="berita1.png.png" alt="Desain grafis kreatif dengan elemen modern" class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-blue-600 text-white px-3 py-1 rounded-full text-xs font-semibold">ELS DESAIN GRAFIS</span>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-lg mb-3 text-gray-800">Menembus Batas Kreativitas</h3>
                        <p class="text-gray-600 mb-4 text-sm">Suasana di kelas ELS Desain Grafis tidak selalu kaku. Ada yang serius mengutak-atik desain, ada pula yang sesekali bermain game. Namun, justru dalam atmosfer santai itulah kreativitas siswa semakin tumbuh. ...</p>
                        <div class="flex items-center justify-between mt-4">
                            <span class="text-sm text-gray-500">23 Sept 2025</span>
                            <a href="https://share.google/5ts2tjQrj9KSaK2fw" class="text-blue-600 hover:text-blue-800 text-sm font-semibold">→</a>
                        </div>
                    </div>
                </div>
                <!-- News Card 2: ELS Cooking -->
                <div class="news-card bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="relative">
                        <img src="berita3.png.png" alt="Ilustrasi kegiatan cooking dengan latar alam" class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-orange-500 text-white px-3 py-1 rounded-full text-xs font-semibold">ELS COOKING</span>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-lg mb-3 text-gray-800">Inovasi Mi Ayam ala Siswa ELS Cooking</h3>
                        <p class="text-gray-600 mb-4 text-sm">Memodifikasi resep secara mandiri untuk menemukan cita rasa yang menurut mereka paling pas di lidah. ...</p>
                        <div class="flex items-center justify-between mt-4">
                            <span class="text-sm text-gray-500">15 Oktober 2025</span>
                            <a href="https://share.google/5ts2tjQrj9KSaK2fw" class="text-blue-600 hover:text-blue-800 text-sm font-semibold">→</a>
                        </div>
                    </div>
                </div>
                <!-- News Card 3: ELS Makeup -->
                <div class="news-card bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="relative">
                        <img src="Makeup.png" alt="Beauty and makeup class with students learning skincare" class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-pink-500 text-white px-3 py-1 rounded-full text-xs font-semibold">ELS MAKEUP</span>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-lg mb-3 text-gray-800">EKSKUL MAKEUP: Sekolah, Skincare, Self-Confidence!</h3>
                        <p class="text-gray-600 mb-4 text-sm">SMA Kristen Petra 4 Sidoarjo punya cara unik mendukung kreativitas siswanya. ...</p>
                        <div class="flex items-center justify-between mt-4">
                            <span class="text-sm text-gray-500">9 September 2025</span>
                            <a href="https://share.google/5ts2tjQrj9KSaK2fw" class="text-blue-600 hover:text-blue-800 text-sm font-semibold">→</a>
                        </div>
                    </div>
                </div>
                <!-- News Card 4: ELS Bahasa Jepang -->
                <div class="news-card bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="relative">
                        <img src="jepang.png" alt="Japanese language class" class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-red-600 text-white px-3 py-1 rounded-full text-xs font-semibold">ELS BAHASA JEPANG</span>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-lg mb-3 text-gray-800">Bahasa Jepang sebagai Jembatan Masa Depan</h3>
                        <p class="text-gray-600 mb-4 text-sm">Bahasa Jepang merupakan salah satu bahasa asing yang memiliki daya tarik besar bagi generasi muda di berbagai belahan dunia. ...</p>
                        <div class="flex items-center justify-between mt-4">
                            <span class="text-sm text-gray-500">9 September 2025</span>
                            <a href="https://share.google/5ts2tjQrj9KSaK2fw" class="text-blue-600 hover:text-blue-800 text-sm font-semibold">→</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Comment Section Placeholder -->
    <section id="comments" class="py-16 bg-purple-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-8">Tinggalkan Komentar</h2>
            <div class="max-w-2xl mx-auto bg-white p-8 rounded-xl shadow-lg">
                <form>
                    <div class="mb-4">
                        <label for="name" class="block text-gray-700 font-medium mb-2">Nama</label>
                        <input type="text" id="name" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-500" placeholder="Nama Anda">
                    </div>
                    <div class="mb-4">
                        <label for="comment" class="block text-gray-700 font-medium mb-2">Komentar</label>
                        <textarea id="comment" rows="4" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-500" placeholder="Tulis komentar Anda di sini..."></textarea>
                    </div>
                    <button type="submit" class="w-full bg-purple-600 text-white font-semibold py-3 px-4 rounded-lg hover:bg-purple-700 transition duration-300">Kirim Komentar</button>
                </form>
            </div>
        </div>
    </section>
 
    <footer id="contact" class="bg-gray-900 text-white py-12">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-2xl font-bold mb-4">Ikuti Kami</h2>
            <p class="text-gray-400 mb-8">Terhubung dengan kami melalui media sosial.</p>
            <div class="flex justify-center items-center space-x-6">
                <!-- WhatsApp Link -->
                <a href="https://wa.me/yourphonenumber" target="_blank" class="flex items-center text-white transition duration-300 rounded-lg px-4 py-2 social-btn-gradient">
                    <i class="fab fa-whatsapp text-2xl mr-2"></i>
                    <span class="font-medium">WhatsApp</span>
                </a>
                <!-- Instagram Link -->
                <a href="https://www.instagram.com/digicomtrapat/" target="_blank" class="flex items-center text-white transition duration-300 rounded-lg px-4 py-2 social-btn-gradient">
                    <i class="fab fa-instagram text-2xl mr-2"></i>
                    <span class="font-medium">Instagram</span>
                </a>
                <!-- TikTok Link -->
                <a href="https://tiktok.com/@yourprofile" target="_blank" class="flex items-center text-white transition duration-300 rounded-lg px-4 py-2 social-btn-gradient">
                    <i class="fab fa-tiktok text-2xl mr-2"></i>
                    <span class="font-medium">TikTok</span>
                </a>
            </div>
            <div class="border-t border-gray-700 mt-10 pt-6">
                <p class="text-gray-500 text-sm">&copy; 2025 Tim Jurnalistik SMA Petra 4 Sidoarjo. All Rights Reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
