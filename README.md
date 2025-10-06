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

        /* Styling tambahan untuk live streaming */
        .live-stream-container {
            position: relative;
            overflow: hidden;
            border-radius: 12px;
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
        }
        .live-stream-container iframe {
            width: 100%;
            height: 400px; /* Tinggi default, bisa disesuaikan */
            border: none;
        }
        .live-indicator {
            position: absolute;
            top: 10px;
            right: 10px;
            background: #ef4444;
            color: white;
            padding: 4px 8px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: bold;
            z-index: 10;
            animation: pulse 2s infinite;
        }
        @media (max-width: 768px) {
            .live-stream-container iframe {
                height: 250px;
            }
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

    <!-- Hero Section -->
    <section id="home" class="gradient-bg text-white py-16">
        <div class="container mx-auto px-4">
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <span class="bg-white text-purple-600 px-4 py-1 rounded-full text-sm font-semibold mb-4 inline-block">FEATURED STORY</span>
                    <h2 class="text-4xl md:text-5xl font-bold mb-6 leading-tight">
                        Wired for Innovation Throught Electro
                    </h2>
                    <p class="text-purple-100 mb-8 text-lg">
                        Di balik ruang fisika yang penuh dengan untaian kabel, transistor, dan resistor sekelompok siswa sibuk merakit alat alat rusak. 

                        Mereka adalah bagian dari ELS Elektro, sebuah kelas yang bukan hanya mengajarkan sebuah teori tetapi juga keterampilan hidup yang berguna. Menurut mereka, yang merupakan bagian dari ELS Elektro merasa bahwa elektro bukanlah sesuatu hal yang cukup mudah untuk dilakukan.

                        Retha, salah satu siswa ELS Elektro berkata, "Di elektro saat kerjain tugas harus bisa fokus, presisi sama sabar."
                    </p>
                    <div class="flex items-center space-x-4 mb-6">
                        <div class="flex items-center">
                            <i class="far fa-calendar-alt mr-2"></i>
                            <span>26 Agustus 2025</span>
                        </div>
                        <div class="flex items-center">
                            <i class="far fa-clock mr-2"></i>
                            <span>info terkini</span>
                        </div>
                    </div>
                    <a href="https://share.google/5ts2tjQrj9KSaK2fw" class="bg-white text-purple-600 px-8 py-3 rounded-lg font-semibold hover:bg-gray-100 transition duration-300">
                        Baca Selengkapnya
                    </a>
                </div>
                <div class="relative">
                    <img src="Berita2.png.png" alt="Modern digital transformation concept with futuristic technology elements and data visualization on dark background" class="rounded-xl shadow-2xl">
                    <div class="absolute -bottom-4 -left-4 bg-white text-gray-800 p-4 rounded-lg shadow-lg">
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-gray-200 rounded-full mr-3">
                                <img src="logo.png" alt="Professional portrait of senior technology journalist with glasses and formal attire" class="rounded-full">
                            </div>
                            <div>
                                <p class="font-semibold"></p>
                                <p class="text-sm text-gray-600">Senior Tech Journalist</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- New Live Streaming Section (Ditambahkan di atas section berita) -->
    <section id="live" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-gray-800 mb-4">Live Streaming</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Tonton siaran langsung acara sekolah dan kegiatan terkini dari SMA Petra 4 Sidoarjo.</p>
            </div>
            <div class="max-w-4xl mx-auto">
                <div class="live-stream-container relative">
                    <!-- Indikator Live -->
                    <div class="live-indicator">
                        <i class="fas fa-circle mr-1"></i>LIVE
                    </div>
                    <!-- Embed YouTube Live Stream (Ganti dengan URL live stream Anda, misalnya dari YouTube) -->
                    <!-- Contoh: Jika menggunakan YouTube, gunakan format embed seperti ini. Pastikan video adalah live stream. -->
                    <iframe 
                        src="https://www.youtube.com/embed/LIVE_STREAM_ID?autoplay=1&mute=0" 
                        allowfullscreen 
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        title="Live Streaming SMA Petra 4 Sidoarjo">
                    </iframe>
                    <!-- Alternatif jika menggunakan Twitch: -->
                    <!-- <iframe src="https://player.twitch.tv/?channel=YOUR_CHANNEL&parent=yourdomain.com" frameborder="0" allowfullscreen="true" scrolling="no" height="400"></iframe> -->
                    <!-- Catatan: Ganti LIVE_STREAM_ID dengan ID video live YouTube Anda (dari URL seperti https://www.youtube.com/watch?v=LIVE_STREAM_ID). Untuk live stream, gunakan fitur embed YouTube Live. -->
                </div>
                <div class="mt-6 text-center">
                    <p class="text-gray-600 text-sm">Tidak ada siaran saat ini? Cek jadwal acara di Instagram kami!</p>
                    <a href="https://www.instagram.com/digicomtrapat/" class="inline-block mt-4 bg-purple-600 text-white px-6 py-2 rounded-lg font-semibold hover:bg-purple-700 transition duration-300">
                        <i class="fab fa-instagram mr-2"></i>Lihat Jadwal
                    </a>
                </div>
            </div>
        </div>
    </section>

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
                        <img src="berita1.png.png" alt="Economic growth chart with upward trend and financial district skyline in background" class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-blue-600 text-white px-3 py-1 rounded-full text-xs font-semibold">ELS DESAIN GRAFIS</span>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-lg mb-3 text-gray-800">Menembus Batas Kreativitas</h3>
                        <p class="text-gray-600 mb-4 text-sm">Suasana di kelas ELS Desain Grafis tidak selalu kaku. Ada yang serius mengutak-atik desain, ada pula yang sesekali bermain game. Namun, justru dalam atmosfer santai itulah kreativitas siswa semakin tumbuh.

                        Kathleen adalah salah satunya. Ia senang bisa merancang CV dengan gaya abstrak yang berbeda dari kebanyakan. “CV saya memang tidak terlalu terstruktur, tapi itu justru ciri khas saya,” katanya. Baginya, materi logo menjadi yang paling berkesan karena sudah terbiasa membuat sketsa sejak awal. Lebih dari sekadar tugas, ia bermimpi menjadikan karya-karyanya sebagai pintu menuju dunia wirausaha.

                        Abby juga punya cerita seru. Bersama timnya, ia melahirkan sebuah brand bernama Maison Étoile—yang berarti toko di galaksi, bagaikan berlian di antara bintang. “Membuat logo itu menyenangkan, karena di situ kami bisa benar-benar menyalurkan kreativitas dan membangun identitas brand sendiri,” jelasnya. Rencananya, produk perdana mereka berupa merchandise akan diluncurkan pada bulan bahasa.

                        Sementara itu, Davin menilai pengalaman ini lebih dari sekadar belajar teknik. “Kami diajarkan untuk berani keluar dari pola yang biasa, jadi karya seperti logo atau CV bisa bermanfaat, bahkan dijual,” ujarnya.

                        Dari CV hingga logo, dari ide hingga brand, para siswa membuktikan bahwa ruang kelas bisa menjadi laboratorium kreativitas. Di sinilah mereka tidak hanya belajar desain, tetapi juga belajar bermimpi lebih besar: menyiapkan masa depan dengan karya.
                        </p>
                        <div class="flex items-center justify-between mt-4">
                            <span class="text-sm text-gray-500">23 Sept 2025</span>
                            <a href="https://share.google/5ts2tjQrj9KSaK2fw" class="text-blue-600 hover:text-blue-800 text-sm font-semibold">
                                →
                            </a>
                        </div>
                    </div>
                </div>

                <!-- News Card 2: ELS Cooking (Diperbaiki struktur) -->
                <div class="news-card bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="relative">
                        <img src="berita3.png.png" alt="Green energy solar panels installation in tropical landscape with clear blue sky" class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-orange-500 text-white px-3 py-1 rounded-full text-xs font-semibold">ELS COOKING</span>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-lg mb-3 text-gray-800">Inovasi Mi Ayam ala Siswa ELS Cooking</h3>
                        <p class="text-gray-600 mb-4 text-sm">Memodifikasi resep secara mandiri untuk menemukan cita rasa yang menurut mereka paling pas di lidah. Inovasi ini membuat sajian mereka terasa unik dibandingkan kuliner sejenis. Bahan utama diperoleh dari persediaan rumah dan pasar tradisional. Meski belum ada cerita khusus di balik sumber lokalnya, mereka tetap menjaga kualitas agar rasa tetap konsisten.

                        Menurut mereka, mi ayam sendiri sudah lama menjadi kuliner khas Indonesia. Perubahan zaman terutama terlihat pada teknik memasak. Dengan hadirnya teknologi baru, proses penyajian kini bisa lebih cepat dan efisien tanpa mengurangi cita rasa.

                        Ketika ditanya siapa yang berperan menjaga keaslian rasa, mereka menegaskan bahwa sosok pewaris resep adalah kunci utama. Warisan inilah yang membuat hidangan tetap otentik. Lebih dari sekadar makanan, mi ayam dianggap penting karena menjadi simbol keanekaragaman rempah di Indonesia. Dari satu mangkuk sederhana, tersimpan identitas budaya dan sejarah panjang kuliner Nusantara.

                        Menariknya, kelompok Jifon juga berusaha menyesuaikan diri dengan tren modern, seperti makanan sehat, vegetarian, hingga digitalisasi pemasaran. Caranya bukan dengan mengubah rasa secara total, melainkan meleburkan tren baru ke dalam resep tanpa menghilangkan ciri khas aslinya.

                        Sungguh, seporsi mi ayam ala Jifon bukan hanya soal rasa, tetapi juga kisah tentang tradisi, inovasi, dan identitas budaya Indonesia.
                        </p>
                        <div class="flex items-center justify-between mt-4">
                            <span class="text-sm text-gray-500">15 Oktober 2025</span>
                            <a href="https://share.google/5ts2tjQrj9KSaK2fw" class="text-blue-600 hover:text-blue-800 text-sm font-semibold">
                                →
                            </a>
                        </div>
                    </div>
                </div>

                <!-- News Card 3: ELS Makeup (Diperbaiki struktur) -->
                <div class="news-card bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="relative">
                        <img src="Makeup.png" alt="Beauty and makeup class with students learning skincare" class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-pink-500 text-white px-3 py-1 rounded-full text-xs font-semibold">ELS MAKEUP</span>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-lg mb-3 text-gray-800">EKSKUL MAKEUP: Sekolah, Skincare, Self-Confidence!</h3>
                        <p class="text-gray-600 mb-4 text-sm">SMA Kristen Petra 4 Sidoarjo punya cara unik mendukung kreativitas siswanya. Tahun ajaran 2025 ini, sekolah membuka ekskul Make-Up yang diikuti
