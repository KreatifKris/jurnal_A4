

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BERITA TERKINI SMA PETRA 4 SIDOARJO</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <script src="https://cdn.tailwindcss.com"></script>
    
    <script src="https://cdnjs.cloudflare.com/ajax/libs/tsparticles/2.12.0/tsparticles.bundle.min.js"></script>

    <style>
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
            margin: 0;
            overflow-x: hidden;
            background-color: #f3f4f6;
        }

        #tsparticles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
        }

        .news-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(8px);
            border-radius: 1rem;
            overflow: hidden;
        }
        
        .news-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }

        .breaking-news {
            background-color: #ef4444;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.8; }
        }

        .social-btn-gradient {
            background: linear-gradient(135deg, #3b82f6 0%, #ef4444 100%);
            transition: all 0.3s ease;
        }

        section {
            background: transparent !important;
        }

        /* Animasi masuk untuk komentar baru */
        .comment-fade-in {
            animation: slideUp 0.4s ease-out;
        }

        @keyframes slideUp {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>

    <div id="tsparticles"></div>

    <header class="bg-white/90 backdrop-blur-md shadow-md sticky top-0 z-50">
        <div class="container mx-auto px-4 py-4">
            <div class="flex items-center justify-between">
                <div class="flex items-center">
                    <div class="w-10 h-10 bg-purple-600 rounded-lg flex items-center justify-center mr-3">
                        <i class="fas fa-newspaper text-white text-xl"></i>
                    </div>
                    <h1 class="text-2xl font-bold text-gray-800">Petra 4 News</h1>
                </div>

                <div class="flex items-center space-x-4">
                    <div class="hidden md:flex items-center bg-gray-200 rounded-full px-4 py-2">
                        <i class="fas fa-search text-gray-500 mr-2"></i>
                        <input type="text" id="searchInput" placeholder="Cari berita..." class="bg-transparent outline-none text-sm" oninput="filterNews()">
                    </div>
                </div>
            </div>
        </div>
    </header>

    <div class="breaking-news text-white py-2">
        <div class="container mx-auto px-4">
            <marquee behavior="scroll" direction="left" class="text-sm font-bold">
                Jurnalistik digital bersama tim jurnalistik SMA Petra 4 Sidoarjo - Menembus Batas Kreativitas di Era Digital!
            </marquee>
        </div>
    </div>

    <section id="news" class="py-16">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-4xl font-extrabold text-gray-900 mb-2">Berita Terbaru</h2>
                <div class="h-1 w-20 bg-purple-600 mx-auto"></div>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6" id="newsGrid">
                <div class="news-card border border-gray-100 shadow-sm">
                    <img src="berita1.png.png" class="w-full h-40 object-cover" alt="Desain Grafis">
                    <div class="p-5">
                        <span class="text-xs font-bold text-blue-600 uppercase">Desain Grafis</span>
                        <h3 class="font-bold text-lg mt-2 leading-tight">Menembus Batas Kreativitas</h3>
                        <p class="text-gray-600 text-xs mt-3">Eksplorasi desain tanpa batas di SMA Petra 4...</p>
                        <a href="#" class="inline-block mt-4 text-purple-600 font-bold text-sm">Baca Selengkapnya →</a>
                    </div>
                </div>
                <div class="news-card border border-gray-100 shadow-sm">
                    <img src="berita3.png.png" class="w-full h-40 object-cover" alt="Cooking">
                    <div class="p-5">
                        <span class="text-xs font-bold text-orange-500 uppercase">ELS Cooking</span>
                        <h3 class="font-bold text-lg mt-2 leading-tight">Inovasi Mi Ayam Siswa</h3>
                        <p class="text-gray-600 text-xs mt-3">Kreasi kuliner sehat dan lezat karya siswa...</p>
                        <a href="#" class="inline-block mt-4 text-purple-600 font-bold text-sm">Baca Selengkapnya →</a>
                    </div>
                </div>
                <div class="news-card border border-gray-100 shadow-sm">
                    <img src="Makeup.png" class="w-full h-40 object-cover" alt="Makeup">
                    <div class="p-5">
                        <span class="text-xs font-bold text-pink-500 uppercase">ELS Makeup</span>
                        <h3 class="font-bold text-lg mt-2 leading-tight">Seni Rias & Percaya Diri</h3>
                        <p class="text-gray-600 text-xs mt-3">Mengekspresikan diri melalui seni makeup wajah...</p>
                        <a href="#" class="inline-block mt-4 text-purple-600 font-bold text-sm">Baca Selengkapnya →</a>
                    </div>
                </div>
                <div class="news-card border border-gray-100 shadow-sm">
                    <img src="jepang.png" class="w-full h-40 object-cover" alt="Jepang">
                    <div class="p-5">
                        <span class="text-xs font-bold text-red-600 uppercase">Bahasa Jepang</span>
                        <h3 class="font-bold text-lg mt-2 leading-tight">Jembatan Masa Depan</h3>
                        <p class="text-gray-600 text-xs mt-3">Menguasai bahasa asing untuk peluang global...</p>
                        <a href="#" class="inline-block mt-4 text-purple-600 font-bold text-sm">Baca Selengkapnya →</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="comments" class="py-16">
        <div class="container mx-auto px-4">
            <div class="max-w-2xl mx-auto bg-white/90 backdrop-blur-md p-8 rounded-2xl shadow-xl border border-white">
                <h2 class="text-2xl font-bold text-gray-800 mb-6 flex items-center">
                    <i class="fas fa-comments mr-3 text-purple-600"></i> Diskusi Siswa
                </h2>
                
                <form id="commentForm" class="mb-10">
                    <div class="mb-4">
                        <input type="text" id="name" class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:ring-2 focus:ring-purple-500 outline-none transition-all" placeholder="Nama Lengkap" required>
                    </div>
                    <div class="mb-4">
                        <textarea id="comment" rows="3" class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:ring-2 focus:ring-purple-500 outline-none transition-all" placeholder="Tulis komentar Anda..." required></textarea>
                    </div>
                    <button type="submit" id="submitBtn" class="w-full bg-purple-600 text-white font-bold py-3 rounded-xl hover:bg-purple-700 transform transition active:scale-95 shadow-lg">
                        Kirim Komentar
                    </button>
                </form>

                <div id="commentsList" class="space-y-4">
                    <p class="text-center text-gray-400 text-sm">Memuat diskusi...</p>
                </div>
            </div>
        </div>
    </section>

    <footer class="bg-gray-900 text-white py-12">
        <div class="container mx-auto px-4 text-center">
            <div class="flex justify-center space-x-4 mb-6">
                <a href="#" class="social-btn-gradient p-3 rounded-full w-12 h-12 flex items-center justify-center"><i class="fab fa-whatsapp"></i></a>
                <a href="https://www.instagram.com/digicomtrapat/" class="social-btn-gradient p-3 rounded-full w-12 h-12 flex items-center justify-center"><i class="fab fa-instagram"></i></a>
                <a href="#" class="social-btn-gradient p-3 rounded-full w-12 h-12 flex items-center justify-center"><i class="fab fa-tiktok"></i></a>
            </div>
            <p class="text-gray-500 text-sm">&copy; 2025 Tim Jurnalistik SMA Petra 4 Sidoarjo.</p>
        </div>
    </footer>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/10.7.1/firebase-app.js";
        import { getFirestore, collection, addDoc, query, orderBy, onSnapshot, serverTimestamp } from "https://www.gstatic.com/firebasejs/10.7.1/firebase-firestore.js";

        // Konfigurasi Firebase Anda
        const firebaseConfig = {
            apiKey: "AIzaSyD3yFm25HY3GUrdTEBr9d-eLRbOkH8xnxc",
            authDomain: "jurnal-sma-a4.firebaseapp.com",
            databaseURL: "https://jurnal-sma-a4-default-rtdb.firebaseio.com",
            projectId: "jurnal-sma-a4",
            storageBucket: "jurnal-sma-a4.firebasestorage.app",
            messagingSenderId: "701172220342",
            appId: "1:701172220342:web:ff0d35ca893ee93e6e4117",
            measurementId: "G-6VQT5SGFER"
        };

        // Inisialisasi Firebase
        const app = initializeApp(firebaseConfig);
        const db = getFirestore(app);

        // --- 1. INISIALISASI PARTIKEL ---
        tsParticles.load("tsparticles", {
            particles: {
                number: { value: 50, density: { enable: true, value_area: 800 } },
                color: { value: ["#8B5CF6", "#3b82f6", "#EC4899"] },
                shape: { type: "circle" },
                opacity: { value: 0.3 },
                size: { value: { min: 1, max: 3 } },
                links: { enable: true, distance: 150, color: "#8B5CF6", opacity: 0.2, width: 1 },
                move: { enable: true, speed: 1, direction: "none", outModes: "out" }
            },
            interactivity: {
                events: {
                    onHover: { enable: true, mode: "grab" },
                    onClick: { enable: true, mode: "push" }
                }
            }
        });

        // --- 2. LOGIKA FIREBASE KOMENTAR ---
        const form = document.getElementById('commentForm');
        const commentsList = document.getElementById('commentsList');
        const submitBtn = document.getElementById('submitBtn');

        // Fungsi Kirim Data
        form.addEventListener('submit', async (e) => {
            e.preventDefault();
            
            const name = document.getElementById('name').value;
            const text = document.getElementById('comment').value;

            // Mencegah klik ganda
            submitBtn.disabled = true;
            submitBtn.innerText = "Mengirim...";

            try {
                await addDoc(collection(db, "comments"), {
                    name: name,
                    comment: text,
                    timestamp: serverTimestamp()
                });
                
                form.reset();
                alert("Komentar berhasil dipublikasikan!");
            } catch (error) {
                console.error("Error: ", error);
                alert("Gagal kirim. Pastikan Rules Firebase sudah 'allow write: if true'");
            } finally {
                submitBtn.disabled = false;
                submitBtn.innerText = "Kirim Komentar";
            }
        });

        // Ambil Data Real-time
        const q = query(collection(db, "comments"), orderBy("timestamp", "desc"));
        onSnapshot(q, (snapshot) => {
            commentsList.innerHTML = "";
            
            if (snapshot.empty) {
                commentsList.innerHTML = '<p class="text-center text-gray-400 text-sm">Belum ada diskusi. Jadilah yang pertama!</p>';
                return;
            }

            snapshot.forEach((doc) => {
                const data = doc.data();
                const div = document.createElement('div');
                div.className = "bg-white p-4 rounded-xl border border-gray-100 shadow-sm mb-3 comment-fade-in";
                
                // Ambil inisial nama
                const initial = data.name ? data.name.charAt(0).toUpperCase() : "?";

                div.innerHTML = `
                    <div class="flex items-start">
                        <div class="w-10 h-10 bg-purple-600 rounded-full flex items-center justify-center text-white font-bold shrink-0 mr-3">
                            ${initial}
                        </div>
                        <div>
                            <h4 class="font-bold text-gray-800 text-sm">${data.name}</h4>
                            <p class="text-gray-600 text-sm mt-1">${data.comment}</p>
                        </div>
                    </div>
                `;
                commentsList.appendChild(div);
            });
        }, (error) => {
            console.error("Firebase Error:", error);
            commentsList.innerHTML = '<p class="text-red-500 text-center text-xs">Error: Izin database ditolak.</p>';
        });

        // Fungsi Search Berita
        window.filterNews = function() {
            const query = document.getElementById('searchInput').value.toLowerCase();
            const cards = document.querySelectorAll('.news-card');
            
            cards.forEach(card => {
                const title = card.querySelector('h3').innerText.toLowerCase();
                const category = card.querySelector('span').innerText.toLowerCase();
                
                if (title.includes(query) || category.includes(query)) {
                    card.style.display = "block";
                } else {
                    card.style.display = "none";
                }
            });
        };
    </script>
</body>
