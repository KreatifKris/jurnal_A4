
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BERITA TERKINI SMA PETRA 4 SIDOARJO</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
            animation: fadeInPage 1s ease;  /* Animasi baru: Fade-in untuk seluruh halaman */
        }
        
        @keyframes fadeInPage {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #8B5CF6 0%, #EC4899 50%, #F97316 100%);
        }
        
        .news-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            animation: fadeIn 0.8s ease forwards;  /* Animasi fade-in untuk news cards */
        }
        
        .news-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
        }
        
        .category-badge {
            transition: background-color 0.3s ease, transform 0.3s ease;
        }
        
        .category-badge:hover {
            background-color: #3b82f6;
            transform: scale(1.1);  /* Efek scale hover */
        }
        
        .breaking-news {
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { background-color: #ef4444; }
            50% { background-color: #dc2626; }
            100% { background-color: #ef4444; }
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes slideDown {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .school-logo {
            height: 40px;
            width: auto;
            transition: transform 0.3s ease;
        }
        
        .school-logo:hover {
            transform: scale(1.1);
        }

        .social-btn-gradient {
            background: linear-gradient(135deg, #3b82f6 0%, #ef4444 100%);
            border: none;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .social-btn-gradient:hover {
            background: linear-gradient(135deg, #2563eb 0%, #dc2626 100%);
            transform: scale(1.05);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        #searchInput:focus {
            animation: glow 0.5s ease infinite;  /* Animasi glow saat fokus */
        }

        @keyframes glow {
            0% { box-shadow: 0 0 0 0 rgba(59, 130, 246, 0.5); }
            100% { box-shadow: 0 0 10px 5px rgba(59, 130, 246, 0.5); }
        }

        button {
            transition: transform 0.3s ease;  /* Animasi untuk tombol umum */
        }
        
        button:hover {
            transform: scale(1.05);  /* Efek scale pada tombol */
        }

        #commentsList div {
            animation: slideDown 0.5s ease;  /* Animasi untuk setiap komentar */
        }
    </style>
</head>
<body class="bg-gray-100">
    <!-- Header -->
    <header class="bg-white shadow-md sticky top-0 z-50 animation-fadeInHeader">  <!-- Animasi untuk header -->
        <div class="container mx-auto px-4 py-4">
            <div class="flex items-center justify-between">
                <!-- Logo Kiri -->
                <div class="flex items-center">
                    <div class="w-10 h-10 bg-purple-600 rounded-lg flex items-center justify-center mr-3 animate-fadeIn">
                        <i class="fas fa-newspaper text-white text-xl"></i>
                    </div>
                    <img src="logo.png" class="school-logo">
                    <h1 class="text-3xl font-bold text-black">Berita Terkini</h1>
                </div>

                <!-- Search, Mobile Menu, dan Logo Listing -->
                <div class="flex items-center space-x-4">
                    <!-- Search -->
                    <div class="hidden md:flex items-center bg-gray-100 rounded-full px-4 py-2" id="searchContainer">
                        <i class="fas fa-search text-gray-500 mr-2"></i>
                        <input type="text" id="searchInput" placeholder="Cari berita..." class="bg-transparent outline-none text-sm" oninput="filterNews()">
                    </div>
                    <div class="flex items-center space-x-2">
                        <img src="sekolah.png" class="school-logo rounded-full">
                        <span class="text-sm text-gray-600 hidden md:block">OUR NEWS IN SMA PETRA 4</span>
                    </div>
                    <button class="md:hidden text-gray-700 animate-pulse-slow">
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

    <section id="news" class="py-16 bg-gray-50 animate-fadeInSection">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-gray-800 mb-4">Berita Terbaru</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Update Berita SMA Trafour</p>
            </div>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8" id="newsGrid">
                <!-- News Card 1 (Tidak dihilangkan) -->
                <div class="news-card">
                    <div class="relative">
                        <img src="berita1.png.png" class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-blue-600 text-white px-3 py-1 rounded-full text-xs font-semibold category-badge">ELS DESAIN GRAFIS</span>
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
                <!-- News Card 2 (Tidak dihilangkan) -->
                <div class="news-card">
                    <div class="relative">
                        <img src="berita3.png.png" class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-orange-500 text-white px-3 py-1 rounded-full text-xs font-semibold category-badge">ELS COOKING</span>
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
                <!-- News Card 3 (Tidak dihilangkan) -->
                <div class="news-card">
                    <div class="relative">
                        <img src="Makeup.png" class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-pink-500 text-white px-3 py-1 rounded-full text-xs font-semibold category-badge">ELS MAKEUP</span>
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
                <!-- News Card 4 (Tidak dihilangkan) -->
                <div class="news-card">
                    <div class="relative">
                        <img src="jepang.png" class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-red-600 text-white px-3 py-1 rounded-full text-xs font-semibold category-badge">ELS BAHASA JEPANG</span>
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

    <!-- Comment Section -->
    <section id="comments" class="py-16 bg-purple-50 animate-fadeInSection">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-8">Tinggalkan Komentar</h2>
            <div class="max-w-2xl mx-auto bg-white p-8 rounded-xl shadow-lg">
                <form id="commentForm">
                    <div class="mb-4">
                        <label for="name" class="block text-gray-700 font-medium mb-2">Nama</label>
                        <input type="text" id="name" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-500 animate-underline" placeholder="Nama Anda" required>
                    </div>
                    <div class="mb-4">
                        <label for="comment" class="block text-gray-700 font-medium mb-2">Komentar</label>
                        <textarea id="comment" rows="4" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-500 animate-underline" placeholder="Tulis komentar Anda di sini..." required></textarea>
                    </div>
                    <button type="submit" class="w-full bg-purple-600 text-white font-semibold py-3 px-4 rounded-lg hover:bg-purple-700 transition duration-300 animate-pulse-on-hover">Kirim Komentar</button>
                </form>
                <div id="commentsList" class="mt-8">
                    <h3 class="text-xl font-bold text-gray-800 mb-4">Daftar Komentar</h3>
                </div>
            </div>
        </div>
    </section>

    <footer id="contact" class="bg-gray-900 text-white py-12 animate-fadeInSection">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-2xl font-bold mb-4 animate-fadeIn">Ikuti Kami</h2>
            <p class="text-gray-400 mb-8 animate-fadeIn">Terhubung dengan kami melalui media sosial.</p>
            <div class="flex justify-center items-center space-x-6 animate-fadeIn">
                <a href="https://wa.me/yourphonenumber" target="_blank" class="flex items-center text-white transition duration-300 rounded-lg px-4 py-2 social-btn-gradient">
                    <i class="fab fa-whatsapp text-2xl mr-2"></i>
                    <span class="font-medium">WhatsApp</span>
                </a>
                <a href="https://www.instagram.com/digicomtrapat/" target="_blank" class="flex items-center text-white transition duration-300 rounded-lg px-4 py-2 social-btn-gradient">
                    <i class="fab fa-instagram text-2xl mr-2"></i>
                    <span class="font-medium">Instagram</span>
                </a>
                <a href="https://tiktok.com/@yourprofile" target="_blank" class="flex items-center text-white transition duration-300 rounded-lg px-4 py-2 social-btn-gradient">
                    <i class="fab fa-tiktok text-2xl mr-2"></i>
                    <span class="font-medium">TikTok</span>
                </a>
            </div>
            <div class="border-t border-gray-700 mt-10 pt-6 animate-fadeIn">
                <p class="text-gray-500 text-sm">&copy; 2025 Tim Jurnalistik SMA Petra 4 Sidoarjo. All Rights Reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        const form = document.getElementById('commentForm');
        const commentsList = document.getElementById('commentsList');
        const serverUrl = 'http://localhost:3000';

        form.addEventListener('submit', async (e) => {
            e.preventDefault();
            const name = document.getElementById('name').value;
            const commentText = document.getElementById('comment').value;
            try {
                const response = await fetch(`${serverUrl}/comments`, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify({ name, comment: commentText }),
                });
                if (response.ok) {
                    alert('Komentar berhasil dikirim!');
                    form.reset();
                    fetchComments();
                } else {
                    alert('Gagal mengirim komentar.');
                }
            } catch (error) {
                console.error(error);
                alert('Terjadi kesalahan.');
            }
        });

        async function fetchComments() {
            try {
                const response = await fetch(`${serverUrl}/comments`);
                const comments = await response.json();
                commentsList.innerHTML = '<h3 class="text-xl font-bold text-gray-800 mb-4">Daftar Komentar</h3>';
                comments.forEach((item) => {
                    const commentDiv = document.createElement('div');
                    commentDiv.className = 'bg-gray-100 p-
