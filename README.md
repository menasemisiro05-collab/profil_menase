<!DOCTYPE html>
<html lang="id" x-data="{ darkMode: true }" :class="{ 'dark': darkMode }">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menase Misiro | Portofolio & Student Profile</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
    <!-- Google Fonts: Inter & Roboto Slab -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&family=Roboto+Slab:wght@400;700&display=swap" rel="stylesheet">
    <!-- Alpine.js CDN -->
    <script defer src="https://cdn.jsdelivr.net/npm/alpinejs@3.x.x/dist/cdn.min.js"></script>
    <!-- Font Awesome untuk Icon -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
        }
        .btn-font {
            font-family: 'Roboto Slab', serif;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-900 dark:bg-slate-950 dark:text-slate-100 transition-colors duration-300">

    <!-- TOPBAR -->
    <div class="bg-amber-500 text-slate-950 text-xs md:text-sm py-2 px-4 text-center font-semibold tracking-wide border-b border-amber-600">
        🚀 Available for freelance projects & collaboration! <span class="hidden md:inline">| Mahasiswa STMIK Pesat Nabire</span>
    </div>

    <!-- NAVBAR -->
    <nav class="sticky top-0 z-40 backdrop-blur-md bg-white/70 dark:bg-slate-950/70 border-b border-slate-200 dark:border-slate-800 transition-colors duration-300">
        <div class="max-w-6xl mx-auto px-4 h-16 flex items-center justify-between">
            <a href="#" class="text-xl font-bold tracking-wider text-slate-900 dark:text-white">
                Mr.<span class="text-amber-500">Khujo</span>
            </a>

            <!-- Menu Desktop -->
            <div class="hidden md:flex items-center space-x-8 font-medium text-sm">
                <a href="#home" class="hover:text-amber-500 transition-colors">Home</a>
                <a href="#portfolio" class="hover:text-amber-500 transition-colors">Portfolio</a>
                <a href="#tentang" class="hover:text-amber-500 transition-colors">Tentang Saya</a>
                <a href="#kontak" class="hover:text-amber-500 transition-colors">Kontak</a>
            </div>

            <!-- Dark Mode Toggle & Button -->
            <div class="flex items-center space-x-4">
                <button @click="darkMode = !darkMode" class="p-2 rounded-full hover:bg-slate-200 dark:hover:bg-slate-800 text-amber-500 focus:outline-none" title="Ganti Tema">
                    <i class="fa-solid" :class="darkMode ? 'fa-sun' : 'fa-moon'"></i>
                </button>
                <a href="#kontak" class="btn-font hidden sm:inline-block bg-amber-500 hover:bg-amber-600 text-slate-950 font-bold py-2 px-4 rounded-lg transition-all text-sm shadow-lg shadow-amber-500/20">
                    Hire Me
                </a>
            </div>
        </div>
    </nav>

    <!-- BANNER UTAMA (HERO SECTION) -->
    <header id="home" class="relative overflow-hidden min-h-[calc(100vh-64px)] flex items-center justify-center px-4 py-16 bg-gradient-to-br from-amber-500/5 via-transparent to-transparent">
        <div class="max-w-4xl text-center space-y-6 z-10">
            <div class="inline-flex items-center space-x-2 bg-amber-500/10 text-amber-500 px-3 py-1 rounded-full text-xs font-semibold tracking-wide uppercase border border-amber-500/20">
                <span>Web Developer</span>
                <span class="w-1.5 h-1.5 rounded-full bg-amber-500 animate-pulse"></span>
                <span>Mahasiswa</span>
            </div>
            <h1 class="text-4xl md:text-6xl font-extrabold tracking-tight">
                Mr <span class="text-transparent bg-clip-text bg-gradient-to-r from-amber-500 to-amber-600">Menase Misiro</span>
            </h1>
            <p class="text-lg md:text-xl text-slate-600 dark:text-slate-400 max-w-2xl mx-auto leading-relaxed">
                Mahasiswa Semester 2 di STMIK PESAT NABIRE sekaligus Junior Web Developer yang berfokus membangun aplikasi web modern, responsif, dan interaktif.
            </p>
            <div class="flex flex-wrap justify-center gap-4 pt-4">
                <a href="#portfolio" class="btn-font bg-amber-500 hover:bg-amber-600 text-slate-950 font-bold py-3 px-6 rounded-xl transition-all shadow-xl shadow-amber-500/20 flex items-center space-x-2">
                    <span>Lihat Portfolio</span>
                    <i class="fa-solid fa-arrow-right text-xs"></i>
                </a>
                <a href="#tentang" class="btn-font border-2 border-slate-300 dark:border-slate-700 hover:border-amber-500 dark:hover:border-amber-500 font-bold py-3 px-6 rounded-xl transition-all flex items-center space-x-2">
                    <span>Tentang Saya</span>
                </a>
            </div>
        </div>
        <!-- Dekorasi Background -->
        <div class="absolute top-1/4 left-1/4 w-72 h-72 bg-amber-500/10 rounded-full blur-3xl -z-10 animate-pulse"></div>
        <div class="absolute bottom-1/4 right-1/4 w-72 h-72 bg-amber-600/10 rounded-full blur-3xl -z-10 animate-pulse delay-75"></div>
    </header>

    <!-- PORTFOLIO SECTION (HASIL UJIAN) -->
    <section id="portfolio" class="max-w-6xl mx-auto px-4 py-20 border-t border-slate-200 dark:border-slate-900">
        <div class="text-center max-w-2xl mx-auto mb-12">
            <h2 class="text-3xl font-bold tracking-tight">Portfolio & Transkrip</h2>
            <p class="text-slate-600 dark:text-slate-400 mt-2">Bukti pencapaian akademik Semester 1 sebagai komitmen dalam belajar teknologi dan ilmu komputer.</p>
        </div>

        <!-- IPK Highlight Card -->
        <div class="bg-gradient-to-r from-amber-500 to-amber-600 text-slate-950 rounded-2xl p-6 md:p-8 shadow-xl mb-8 flex flex-col md:flex-row items-center justify-between gap-6">
            <div>
                <h3 class="text-xl md:text-2xl font-bold">Indeks Prestasi Kumulatif (IPK)</h3>
                <p class="text-slate-900/80 text-sm mt-1">Hasil evaluasi belajar semester ganjil, STMIK PESAT NABIRE.</p>
            </div>
            <div class="bg-white/20 backdrop-blur-md border border-white/30 px-6 py-4 rounded-xl text-center min-w-[140px]">
                <span class="text-4xl font-extrabold tracking-tight">3.50</span>
            </div>
        </div>

        <!-- Tabel Transkrip Nilai -->
        <div class="bg-white dark:bg-slate-900 rounded-2xl border border-slate-200 dark:border-slate-800 shadow-xl overflow-hidden">
            <div class="p-6 border-b border-slate-200 dark:border-slate-800 flex justify-between items-center">
                <h4 class="font-bold text-lg flex items-center space-x-2">
                    <i class="fa-solid fa-graduation-cap text-amber-500"></i>
                    <span>Rincian Mata Kuliah - Semester 1</span>
                </h4>
                <span class="text-xs bg-slate-100 dark:bg-slate-800 px-3 py-1 rounded-full text-slate-500">Lulus</span>
            </div>
            <div class="overflow-x-auto">
                <table class="w-full text-left border-collapse">
                    <thead>
                        <tr class="bg-slate-50 dark:bg-slate-800/50 text-xs font-bold tracking-wider uppercase text-slate-500 border-b border-slate-200 dark:border-slate-800">
                            <th class="py-4 px-6">Mata Kuliah</th>
                            <th class="py-4 px-6 text-center">Nilai Huruf</th>
                            <th class="py-4 px-6 text-center">Status</th>
                        </tr>
                    </thead>
                    <tbody class="divide-y divide-slate-200 dark:divide-slate-800 text-sm">
                        <tr class="hover:bg-slate-50/50 dark:hover:bg-slate-800/30 transition-colors">
                            <td class="py-4 px-6 font-medium">Agama Kristen Protestan</td>
                            <td class="py-4 px-6 text-center"><span class="bg-emerald-500/10 text-emerald-500 font-bold px-2.5 py-1 rounded">A</span></td>
                            <td class="py-4 px-6 text-center text-slate-500">Selesai</td>
                        </tr>
                        <tr class="hover:bg-slate-50/50 dark:hover:bg-slate-800/30 transition-colors">
                            <td class="py-4 px-6 font-medium">Pancasila</td>
                            <td class="py-4 px-6 text-center"><span class="bg-emerald-500/10 text-emerald-500 font-bold px-2.5 py-1 rounded">A-</span></td>
                            <td class="py-4 px-6 text-center text-slate-500">Selesai</td>
                        </tr>
                        <tr class="hover:bg-slate-50/50 dark:hover:bg-slate-800/30 transition-colors">
                            <td class="py-4 px-6 font-medium">Bahasa Indonesia</td>
                            <td class="py-4 px-6 text-center"><span class="bg-amber-500/10 text-amber-500 font-bold px-2.5 py-1 rounded">B+</span></td>
                            <td class="py-4 px-6 text-center text-slate-500">Selesai</td>
                        </tr>
                        <tr class="hover:bg-slate-50/50 dark:hover:bg-slate-800/30 transition-colors">
                            <td class="py-4 px-6 font-medium">Dasar Teknik Komputer</td>
                            <td class="py-4 px-6 text-center"><span class="bg-amber-500/10 text-amber-500 font-bold px-2.5 py-1 rounded">B+</span></td>
                            <td class="py-4 px-6 text-center text-slate-500">Selesai</td>
                        </tr>
                        <tr class="hover:bg-slate-50/50 dark:hover:bg-slate-800/30 transition-colors">
                            <td class="py-4 px-6 font-medium">Matematika</td>
                            <td class="py-4 px-6 text-center"><span class="bg-amber-500/10 text-amber-500 font-bold px-2.5 py-1 rounded">B</span></td>
                            <td class="py-4 px-6 text-center text-slate-500">Selesai</td>
                        </tr>
                        <tr class="hover:bg-slate-50/50 dark:hover:bg-slate-800/30 transition-colors">
                            <td class="py-4 px-6 font-medium">Pengantar Teknologi Informasi</td>
                            <td class="py-4 px-6 text-center"><span class="bg-amber-500/10 text-amber-500 font-bold px-2.5 py-1 rounded">B+</span></td>
                            <td class="py-4 px-6 text-center text-slate-500">Selesai</td>
                        </tr>
                        <tr class="hover:bg-slate-50/50 dark:hover:bg-slate-800/30 transition-colors">
                            <td class="py-4 px-6 font-medium">Bahasa Inggris</td>
                            <td class="py-4 px-6 text-center"><span class="bg-emerald-500/10 text-emerald-500 font-bold px-2.5 py-1 rounded">A</span></td>
                            <td class="py-4 px-6 text-center text-slate-500">Selesai</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
    </section>

    <!-- TENTANG SAYA SECTION -->
    <section id="tentang" class="max-w-6xl mx-auto px-4 py-20 border-t border-slate-200 dark:border-slate-900 bg-slate-100/50 dark:bg-slate-900/20 rounded-3xl">
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12">
            <!-- Profil Singkat / Kiri -->
            <div class="space-y-4">
                <div class="inline-block bg-amber-500 text-slate-950 text-xs font-bold px-3 py-1 rounded-md uppercase tracking-wider">
                    Biography
                </div>
                <h2 class="text-3xl font-bold tracking-tight">Tentang Saya</h2>
                <p class="text-slate-600 dark:text-slate-400 leading-relaxed text-sm">
                    Nama lengkap saya <strong>Chalvin Menase Otniel Misiro</strong>. Lahir di Makimi, 20 Maret 2005 (Umur 21 Tahun). Saya dibesarkan dalam keluarga besar 7 bersaudara dari pasangan Ayah Matias Misiro (Suku Wate) dan Ibu Helsin Fedrika Rumaseb (Suku Biak).
                </p>
                <div class="p-4 border-l-2 border-amber-500 bg-amber-500/5 rounded-r-xl space-y-2 text-xs">
                    <p><strong>Organisasi Kampus:</strong></p>
                    <ul class="list-disc list-inside space-y-1 text-slate-600 dark:text-slate-400">
                        <li>Ketua Kelas Angkatan 7 Karyawan</li>
                        <li>Anggota BEM (Jabatan Humas)</li>
                    </ul>
                </div>
            </div>

            <!-- Detail Data / Kanan (2 Kolom) -->
            <div class="lg:col-span-2 grid grid-cols-1 md:grid-cols-2 gap-6">
                <!-- Biodata Card -->
                <div class="bg-white dark:bg-slate-900 p-6 rounded-2xl border border-slate-200 dark:border-slate-800 shadow-sm space-y-4">
                    <h3 class="font-bold border-b border-slate-100 dark:border-slate-800 pb-2 flex items-center space-x-2 text-amber-500">
                        <i class="fa-solid fa-user text-sm"></i> <span>Informasi Pribadi</span>
                    </h3>
                    <ul class="space-y-2 text-sm">
                        <li class="flex justify-between"><span class="text-slate-500">Nama Panggilan:</span> <span class="font-medium">Apin</span></li>
                        <li class="flex justify-between"><span class="text-slate-500">NIM           :</span> <span class="font-medium">2501061</span></li>
                        <li class="flex justify-between"><span class="text-slate-500">Kelas         :</span> <span class="font-medium">Karyawan</span></li>
                        <li class="flex justify-between"><span class="text-slate-500">Angkatan      :</span> <span class="font-medium">7</span></li>
                        <li class="flex justify-between"><span class="text-slate-500">Mahasiswa     :</span> <span class="font-medium">STMIK PESAT NABIRE</span></li>
                        <li class="flex justify-between"><span class="text-slate-500">Jumlah Saudara:</span> <span class="font-medium">7 Bersaudara</span></li>
                        <li class="flex justify-between"><span class="text-slate-500">Asal          :</span> <span class="font-medium">Makimi, Nabire, Papua Tengah</span></li>
                        <li class="flex justify-between"><span class="text-slate-500">Tinggal       :</span> <span class="font-medium">Makimi</li>
                    </ul>
                </div>

                <!-- Riwayat Pendidikan Card -->
                <div class="bg-white dark:bg-slate-900 p-6 rounded-2xl border border-slate-200 dark:border-slate-800 shadow-sm space-y-4">
                    <h3 class="font-bold border-b border-slate-100 dark:border-slate-800 pb-2 flex items-center space-x-2 text-amber-500">
                        <i class="fa-solid fa-graduation-cap text-sm"></i> <span>Riwayat Studi</span>
                    </h3>
                    <div class="relative border-l border-slate-200 dark:border-slate-800 pl-4 space-y-4 text-xs">
                        <div class="relative">
                            <span class="absolute -left-[21px] top-0 bg-amber-500 w-2.5 h-2.5 rounded-full"></span>
                            <h4 class="font-bold text-sm">STMIK PESAT NABIRE</h4>
                            <p class="text-slate-500">Mahasiswa Aktif - Semester 2</p>
                        </div>
                        <div class="relative">
                            <span class="absolute -left-[21px] top-0 bg-slate-300 dark:bg-slate-700 w-2.5 h-2.5 rounded-full"></span>
                            <h4 class="font-bold">SMK Negeri 3 Nabire</h4>
                            <p class="text-slate-500">Masa Studi 3 Tahun</p>
                        </div>
                        <div class="relative">
                            <span class="absolute -left-[21px] top-0 bg-slate-300 dark:bg-slate-700 w-2.5 h-2.5 rounded-full"></span>
                            <h4 class="font-bold">SMP Negeri Makimi</h4>
                            <p class="text-slate-500">Masa Studi 3 Tahun</p>
                        </div>
                        <div class="relative">
                            <span class="absolute -left-[21px] top-0 bg-slate-300 dark:bg-slate-700 w-2.5 h-2.5 rounded-full"></span>
                            <h4 class="font-bold">SD Negeri Jayanti</h4>
                            <p class="text-slate-500">Masa Studi 6 Tahun</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- KONTAK SECTION WITH FORM -->
    <section id="kontak" class="max-w-6xl mx-auto px-4 py-20 border-t border-slate-200 dark:border-slate-900">
        <div class="text-center max-w-2xl mx-auto mb-12">
            <h2 class="text-3xl font-bold tracking-tight">Mari Terhubung</h2>
            <p class="text-slate-600 dark:text-slate-400 mt-2 text-sm">Punya proyek website atau ingin berdiskusi seputar organisasi dan perkuliahan? Hubungi saya kapan saja.</p>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-5 gap-8 items-start">
            <!-- Informasi Kontak Kiri (2 Kolom) -->
            <div class="lg:col-span-2 space-y-4">
                <a href="tel:081327928992" class="flex items-center space-x-4 p-4 bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 rounded-xl hover:border-amber-500 dark:hover:border-amber-500 transition-all group">
                    <div class="w-10 h-10 bg-amber-500/10 text-amber-500 rounded-lg flex items-center justify-center group-hover:bg-amber-500 group-hover:text-slate-950 transition-colors">
                        <i class="fa-solid fa-phone"></i>
                    </div>
                    <div class="text-left">
                        <p class="text-xs text-slate-500">Telepon / WA</p>
                        <p class="text-sm font-semibold">081327928992</p>
                    </div>
                </a>
                <a href="mailto:menasemisiro05@gmail.com" class="flex items-center space-x-4 p-4 bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 rounded-xl hover:border-amber-500 dark:hover:border-amber-500 transition-all group">
                    <div class="w-10 h-10 bg-amber-500/10 text-amber-500 rounded-lg flex items-center justify-center group-hover:bg-amber-500 group-hover:text-slate-950 transition-colors">
                        <i class="fa-solid fa-envelope"></i>
                    </div>
                    <div class="text-left">
                        <p class="text-xs text-slate-500">Email Resmi</p>
                        <p class="text-sm font-semibold break-all">menasemisiro05@gmail.com</p>
                    </div>
                </a>
            </div>

            <!-- Form Kirim Pesan Kanan (3 Kolom) -->
            <div class="lg:col-span-3 bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 rounded-2xl p-6 md:p-8 shadow-xl"
                 x-data="{ name: '', email: '', message: '', isSuccess: false, submitForm() { if(this.name && this.email && this.message) { this.isSuccess = true; this.name = ''; this.email = ''; this.message = ''; setTimeout(() => this.isSuccess = false, 5000); } } }">

                <h3 class="text-lg font-bold mb-6 flex items-center space-x-2">
                    <i class="fa-solid fa-paper-plane text-amber-500"></i>
                    <span>Kirim Pesan Langsung</span>
                </h3>

                <!-- Alert Sukses Berhasil Kirim -->
                <div x-show="isSuccess" x-transition class="mb-6 p-4 bg-emerald-500/10 border border-emerald-500/30 text-emerald-500 rounded-xl text-sm flex items-center space-x-2">
                    <i class="fa-solid fa-circle-check"></i>
                    <span>Terima kasih! Pesan Anda berhasil dikirim (simulasi).</span>
                </div>

                <form @submit.prevent="submitForm()" class="space-y-4 text-sm">
                    <div>
                        <label class="block text-xs font-semibold mb-2 text-slate-500 uppercase tracking-wider">Nama Lengkap</label>
                        <input type="text" x-model="name" required placeholder="Masukkan nama Anda"
                               class="w-full px-4 py-3 bg-slate-50 dark:bg-slate-950 border border-slate-200 dark:border-slate-800 rounded-xl focus:outline-none focus:border-amber-500 dark:focus:border-amber-500 transition-all">
                    </div>
                    <div>
                        <label class="block text-xs font-semibold mb-2 text-slate-500 uppercase tracking-wider">Alamat Email</label>
                        <input type="email" x-model="email" required placeholder="nama@email.com"
                               class="w-full px-4 py-3 bg-slate-50 dark:bg-slate-950 border border-slate-200 dark:border-slate-800 rounded-xl focus:outline-none focus:border-amber-500 dark:focus:border-amber-500 transition-all">
                    </div>
                    <div>
                        <label class="block text-xs font-semibold mb-2 text-slate-500 uppercase tracking-wider">Isi Pesan</label>
                        <textarea x-model="message" required rows="4" placeholder="Tuliskan pesan atau penawaran kerja sama di sini..."
                                  class="w-full px-4 py-3 bg-slate-50 dark:bg-slate-950 border border-slate-200 dark:border-slate-800 rounded-xl focus:outline-none focus:border-amber-500 dark:focus:border-amber-500 transition-all"></textarea>
                    </div>

                    <button type="submit" class="btn-font w-full bg-amber-500 hover:bg-amber-600 text-slate-950 font-bold py-3 px-6 rounded-xl transition-all shadow-lg shadow-amber-500/20 flex items-center justify-center space-x-2">
                        <span>Kirim Sekarang</span>
                        <i class="fa-solid fa-paper-plane text-xs"></i>
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="border-t border-slate-200 dark:border-slate-900 py-8 text-center text-xs text-slate-500">
        <p>&copy; 2026 Chalvin Menase Otniel Misiro. Built with Tailwind CSS & Alpine.js.</p>
    </footer>

    <!-- STICKY BOTTOM SOCIAL MEDIA & BACK TO TOP BUTTONS -->
    <div class="fixed bottom-6 right-6 z-50 flex flex-col space-y-3" x-data="{ showTapToTop: false }" @window.scroll.window="showTapToTop = (window.pageYOffset > 300) ? true : false">

        <!-- Instagram Button -->
        <a href="https://instagram.com" target="_blank" class="w-12 h-12 bg-white dark:bg-slate-900 text-slate-700 dark:text-slate-300 rounded-full flex items-center justify-center shadow-lg hover:bg-amber-500 dark:hover:bg-amber-500 hover:text-slate-950 dark:hover:text-slate-950 transition-all transform hover:-translate-y-1" title="Instagram">
            <i class="fa-brands fa-instagram text-lg"></i>
        </a>

        <!-- WhatsApp Button -->
        <a href="https://wa.me/6281327928992" target="_blank" class="w-12 h-12 bg-white dark:bg-slate-900 text-slate-700 dark:text-slate-300 rounded-full flex items-center justify-center shadow-lg hover:bg-amber-500 dark:hover:bg-amber-500 hover:text-slate-950 dark:hover:text-slate-950 transition-all transform hover:-translate-y-1" title="WhatsApp">
            <i class="fa-brands fa-whatsapp text-lg"></i>
        </a>

        <!-- GitHub Button -->
        <a href="https://github.com" target="_blank" class="w-12 h-12 bg-white dark:bg-slate-900 text-slate-700 dark:text-slate-300 rounded-full flex items-center justify-center shadow-lg hover:bg-amber-500 dark:hover:bg-amber-500 hover:text-slate-950 dark:hover:text-slate-950 transition-all transform hover:-translate-y-1" title="GitHub">
            <i class="fa-brands fa-github text-lg"></i>
        </a>

        <!-- Back to Top Button -->
        <button @click="window.scrollTo({top: 0, behavior: 'smooth'})"
                x-show="showTapToTop"
                x-transition:enter="transition ease-out duration-300"
                x-transition:enter-start="opacity-0 translate-y-10"
                x-transition:enter-end="opacity-100 translate-y-0"
                x-transition:leave="transition ease-in duration-300"
                x-transition:leave-start="opacity-100 translate-y-0"
                x-transition:leave-end="opacity-0 translate-y-10"
                class="btn-font w-12 h-12 bg-amber-500 text-slate-950 font-bold rounded-full flex items-center justify-center shadow-2xl hover:bg-amber-600 transition-all transform hover:-translate-y-1"
                title="Back to Top">
            <i class="fa-solid fa-arrow-up"></i>
        </button>
    </div>

</body>
</html>


