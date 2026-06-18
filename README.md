<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RADEA ARCANA | Ruang Spiritual & Energi</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Inter', sans-serif; background-color: #0f1021; color: #f3f4f6; }
        h1, h2, h3, .font-cinzel { font-family: 'Cinzel', serif; }
        
        /* Glassmorphism Effect */
        .glass {
            background: rgba(30, 27, 75, 0.4);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 215, 0, 0.1);
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
        }

        /* Gold Gradient Text */
        .text-gold {
            background: linear-gradient(to right, #bf953f, #fcf6ba, #b38728, #fbf5b7, #aa771c);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        /* Scroll Reveal Animation */
        .reveal { opacity: 0; transform: translateY(30px); transition: all 0.8s ease-out; }
        .reveal.active { opacity: 1; transform: translateY(0); }

        /* Loader Animation */
        .loader {
            border: 3px solid rgba(255, 215, 0, 0.3);
            border-top: 3px solid #fcf6ba;
            border-radius: 50%;
            width: 24px;
            height: 24px;
            animation: spin 1s linear infinite;
            display: inline-block;
        }
        @keyframes spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
    </style>
</head>
<body class="relative overflow-x-hidden antialiased">

    <!-- Starfield Background -->
    <canvas id="starfield" class="fixed top-0 left-0 w-full h-full -z-10"></canvas>

    <!-- Header Section -->
    <header class="min-h-screen flex flex-col items-center justify-center text-center px-6 reveal pt-20">
        <h1 class="text-5xl md:text-7xl font-bold font-cinzel text-gold mb-4 tracking-widest">RADEA ARCANA</h1>
        <p class="text-sm md:text-base tracking-[0.3em] text-gray-400 mb-8 uppercase">Raihan • Dewi Ratna • Renanda</p>
        <div class="max-w-2xl glass p-8 rounded-2xl">
            <p class="text-lg md:text-xl leading-relaxed font-light">
                Selamat datang di <span class="text-yellow-200">RADEA ARCANA</span>, ruang spiritual dan konsultasi energi yang hadir untuk membantu Anda memahami perjalanan hidup, energi diri, dan pesan-pesan yang ingin disampaikan semesta.
            </p>
        </div>
    </header>

    <!-- Services Section -->
    <section class="py-20 px-6 max-w-6xl mx-auto">
        <h2 class="text-3xl md:text-4xl text-center font-cinzel text-gold mb-12 reveal">Layanan Kami</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Service 1 -->
            <div class="glass p-8 rounded-2xl reveal hover:-translate-y-2 transition-transform duration-300">
                <div class="text-4xl mb-4">🔮</div>
                <h3 class="text-xl font-cinzel text-yellow-200 mb-3">Reading Tarot</h3>
                <p class="text-sm text-gray-300 leading-relaxed">Pembacaan kartu tarot untuk membantu Anda mendapatkan sudut pandang, refleksi diri, serta memahami situasi yang sedang dihadapi.</p>
            </div>
            <!-- Service 2 -->
            <div class="glass p-8 rounded-2xl reveal hover:-translate-y-2 transition-transform duration-300 delay-100">
                <div class="text-4xl mb-4">✨</div>
                <h3 class="text-xl font-cinzel text-yellow-200 mb-3">Pembersihan Energi</h3>
                <p class="text-sm text-gray-300 leading-relaxed">Layanan spiritual untuk membantu membersihkan energi negatif dan menciptakan suasana yang lebih nyaman, tenang, dan positif.</p>
            </div>
            <!-- Service 3 -->
            <div class="glass p-8 rounded-2xl reveal hover:-translate-y-2 transition-transform duration-300 delay-200">
                <div class="text-4xl mb-4">👁️</div>
                <h3 class="text-xl font-cinzel text-yellow-200 mb-3">Gambar Sosok Pendamping</h3>
                <p class="text-sm text-gray-300 leading-relaxed">Visualisasi artistik berdasarkan deskripsi dan interpretasi spiritual yang diberikan selama sesi konsultasi.</p>
            </div>
        </div>
    </section>

    <!-- Operational & Contact Section -->
    <section class="py-20 px-6 max-w-4xl mx-auto text-center reveal">
        <div class="glass p-10 rounded-3xl">
            <h2 class="text-2xl font-cinzel text-gold mb-6">Jam Operasional</h2>
            <p class="text-lg text-gray-300 mb-2">📅 Senin – Jumat</p>
            <p class="text-lg text-gray-300 mb-10">⏰ Buka Setiap Hari</p>
            
            <h2 class="text-2xl font-cinzel text-gold mb-6">Cara Pemesanan</h2>
            <p class="text-gray-300 mb-6">Melayani konsultasi dan pemesanan melalui DM TikTok. Silakan hubungi kami untuk informasi layanan, jadwal, dan konsultasi lebih lanjut.</p>
            
            <a href="https://tiktok.com/@RADEAARCANA" target="_blank" class="inline-block px-8 py-3 bg-gradient-to-r from-purple-800 to-indigo-900 text-white rounded-full font-semibold tracking-wider hover:from-indigo-700 hover:to-purple-600 transition-all shadow-[0_0_15px_rgba(139,92,246,0.5)] border border-purple-400/30">
                Hubungi @RADEA ARCANA
            </a>
        </div>
    </section>

    <!-- Footer Section -->
    <footer class="py-12 text-center px-6 border-t border-white/5 mt-10">
        <h2 class="text-2xl font-cinzel text-gold mb-4 tracking-widest">RADEA ARCANA</h2>
        <p class="text-sm md:text-base text-gray-400 italic max-w-2xl mx-auto font-light">
            "Membantu Anda mengenal diri, memahami energi, dan menemukan makna di setiap perjalanan kehidupan."
        </p>
    </footer>

    <!-- Scripts -->
    <script>
        // 1. Starfield Background Animation
        const canvas = document.getElementById('starfield');
        const ctx = canvas.getContext('2d');
        let width, height, stars = [];

        function initCanvas() {
            width = canvas.width = window.innerWidth;
            height = canvas.height = window.innerHeight;
            stars = [];
            for (let i = 0; i < 200; i++) {
                stars.push({
                    x: Math.random() * width,
                    y: Math.random() * height,
                    radius: Math.random() * 1.5,
                    vx: Math.floor(Math.random() * 50) - 25,
                    vy: Math.floor(Math.random() * 50) - 25
                });
            }
        }

        function drawStars() {
            ctx.clearRect(0, 0, width, height);
            ctx.fillStyle = 'white';
            ctx.beginPath();
            stars.forEach(star => {
                star.x += star.vx / 100;
                star.y += star.vy / 100;
                if (star.x < 0 || star.x > width) star.vx = -star.vx;
                if (star.y < 0 || star.y > height) star.vy = -star.vy;
                ctx.moveTo(star.x, star.y);
                ctx.arc(star.x, star.y, star.radius, 0, Math.PI * 2, true);
            });
            ctx.fill();
            requestAnimationFrame(drawStars);
        }

        window.addEventListener('resize', initCanvas);
        initCanvas();
        drawStars();

        // 2. Scroll Reveal Animation
        function reveal() {
            var reveals = document.querySelectorAll(".reveal");
            for (var i = 0; i < reveals.length; i++) {
                var windowHeight = window.innerHeight;
                var elementTop = reveals[i].getBoundingClientRect().top;
                var elementVisible = 100;
                if (elementTop < windowHeight - elementVisible) {
                    reveals[i].classList.add("active");
                }
            }
        }
        window.addEventListener("scroll", reveal);
        reveal(); // Trigger on load
    </script>
</body>
</html>
