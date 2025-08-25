# PHANTOM-COIN
Visualisasi teknologi berbasis blockchain di era baru cryptocurrency
`phantom-coin.html`
```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Phantom Coin - Cryptocurrency Masa Depan</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, #0f0f23 0%, #1a1a2e 50%, #16213e 100%);
            color: #ffffff;
            min-height: 100vh;
        }
        .gradient-bg {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        .coin-glow {
            box-shadow: 0 0 50px rgba(118, 75, 162, 0.5);
        }
        .feature-card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
        }
        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(118, 75, 162, 0.3);
        }
        .price-ticker {
            background: linear-gradient(45deg, #667eea, #764ba2);
            animation: pulse 2s infinite;
        }
        @keyframes pulse {
            0% { opacity: 1; }
            50% { opacity: 0.8; }
            100% { opacity: 1; }
        }
    </style>
</head>
<body class="min-h-screen">
    <!-- Header -->
    <header class="fixed w-full bg-black/80 backdrop-blur-md z-50">
        <nav class="container mx-auto px-6 py-4">
            <div class="flex items-center justify-between">
                <div class="flex items-center space-x-3">
                    <div class="w-10 h-10 bg-purple-600 rounded-full flex items-center justify-center">
                        <span class="text-white font-bold text-xl">P</span>
                    </div>
                    <span class="text-xl font-bold bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent">
                        PHANTOM COIN
                    </span>
                </div>
                
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#about" class="hover:text-purple-300 transition-colors">Tentang</a>
                    <a href="#features" class="hover:text-purple-300 transition-colors">Fitur</a>
                    <a href="#technology" class="hover:text-purple-300 transition-colors">Teknologi</a>
                    <a href="#get-started" class="hover:text-purple-300 transition-colors">Mulai</a>
                </div>

                <button class="bg-gradient-to-r from-purple-600 to-pink-600 text-white px-6 py-2 rounded-full hover:from-purple-700 hover:to-pink-700 transition-all">
                    Beli Sekarang
                </button>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="pt-32 pb-20 px-6">
        <div class="container mx-auto text-center">
            <div class="max-w-4xl mx-auto">
                <h1 class="text-5xl md:text-7xl font-bold mb-6">
                    <span class="bg-gradient-to-r from-purple-400 via-pink-400 to-blue-400 bg-clip-text text-transparent">
                        Phantom Coin
                    </span>
                </h1>
                <p class="text-xl md:text-2xl text-gray-300 mb-8">
                    Cryptocurrency revolusioner dengan teknologi blockchain generasi berikutnya. 
                    Cepat, aman, dan terdesentralisasi untuk masa depan digital.
                </p>
                
                <div class="flex flex-col sm:flex-row gap-4 justify-center items-center mb-12">
                    <button class="gradient-bg text-white px-8 py-4 rounded-full text-lg font-semibold hover:shadow-2xl transition-all">
                        Mulai Berinvestasi
                    </button>
                    <button class="border border-purple-400 text-purple-300 px-8 py-4 rounded-full text-lg font-semibold hover:bg-purple-400/10 transition-all">
                        Pelajari Lebih Lanjut
                    </button>
                </div>

                <!-- Live Price Ticker -->
                <div class="price-ticker inline-flex items-center px-6 py-3 rounded-full mb-12">
                    <div class="w-3 h-3 bg-green-400 rounded-full mr-3 animate-pulse"></div>
                    <span class="font-mono text-lg">PHM: $</span>
                    <span id="live-price" class="font-mono text-lg font-bold">42.69</span>
                    <span class="ml-2 text-green-300">+2.34%</span>
                </div>
            </div>

            <!-- Coin Visualization -->
            <div class="relative max-w-2xl mx-auto mt-16">
                <div class="coin-glow w-64 h-64 mx-auto bg-gradient-to-br from-purple-600 via-blue-600 to-pink-600 rounded-full flex items-center justify-center relative">
                    <div class="w-48 h-48 bg-black/20 rounded-full flex items-center justify-center">
                        <div class="w-32 h-32 bg-gradient-to-tr from-purple-400 to-blue-400 rounded-full flex items-center justify-center">
                            <span class="text-4xl font-bold text-white">P</span>
                        </div>
                    </div>
                </div>
                <div class="absolute -inset-4 bg-gradient-to-r from-purple-600 to-pink-600 rounded-full opacity-20 blur-3xl"></div>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="py-16 px-6 bg-black/30">
        <div class="container mx-auto">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8 text-center">
                <div class="p-6">
                    <div class="text-3xl font-bold text-purple-400 mb-2">$4.2B</div>
                    <div class="text-gray-400">Market Cap</div>
                </div>
                <div class="p-6">
                    <div class="text-3xl font-bold text-purple-400 mb-2">21M</div>
                    <div class="text-gray-400">Total Supply</div>
                </div>
                <div class="p-6">
                    <div class="text-3xl font-bold text-purple-400 mb-2">1.2M</div>
                    <div class="text-gray-400">Active Users</div>
                </div>
                <div class="p-6">
                    <div class="text-3xl font-bold text-purple-400 mb-2">0.001s</div>
                    <div class="text-gray-400">Transaction Time</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section id="features" class="py-20 px-6">
        <div class="container mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold mb-4">Fitur Unggulan</h2>
                <p class="text-xl text-gray-300 max-w-2xl mx-auto">
                    Phantom Coin menawarkan teknologi terdepan dengan fitur-fitur yang membuatnya unggul di pasar cryptocurrency.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="feature-card p-8 rounded-2xl">
                    <div class="w-16 h-16 gradient-bg rounded-2xl flex items-center justify-center mb-6">
                        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path>
                        </svg>
                    </div>
                    <h3 class="text-xl font-semibold mb-4">Kecepatan Tinggi</h3>
                    <p class="text-gray-300">
                        Transaksi diproses dalam hitungan detik dengan teknologi blockchain generasi ke-3.
                    </p>
                </div>

                <div class="feature-card p-8 rounded-2xl">
                    <div class="w-16 h-16 gradient-bg rounded-2xl flex items-center justify-center mb-6">
                        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z"></path>
                        </svg>
                    </div>
                    <h3 class="text-xl font-semibold mb-4">Keamanan Maximum</h3>
                    <p class="text-gray-300">
                        Dilindungi oleh algoritma enkripsi quantum-resistant dan smart contract audit.
                    </p>
                </div>

                <div class="feature-card p-8 rounded-2xl">
                    <div class="w-16 h-16 gradient-bg rounded-2xl flex items-center justify-center mb-6">
                        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 4v5h.582m15.356 2A8.001 8.001 0 004.582 9m0 0H9m11 11v-5h-.581m0 0a8.003 8.003 0 01-15.357-2m15.357 2H15"></path>
                        </svg>
                    </div>
                    <h3 class="text-xl font-semibold mb-4">Energi Efisien</h3>
                    <p class="text-gray-300">
                        Menggunakan proof-of-stake yang ramah lingkungan dengan konsumsi energi 99% lebih rendah.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Technology Section -->
    <section id="technology" class="py-20 px-6 bg-black/30">
        <div class="container mx-auto">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <div>
                    <h2 class="text-4xl font-bold mb-6">Teknologi Blockchain Masa Depan</h2>
                    <p class="text-lg text-gray-300 mb-6">
                        Phantom Coin dibangun di atas Phantom Chain, blockchain proprietary yang menggabungkan teknologi sharding, zero-knowledge proofs, dan consensus mechanism terbaru.
                    </p>
                    <ul class="space-y-3">
                        <li class="flex items-center">
                            <div class="w-6 h-6 gradient-bg rounded-full mr-3 flex items-center justify-center">
                                <svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                                </svg>
                            </div>
                            <span>10,000+ TPS (Transactions Per Second)</span>
                        </li>
                        <li class="flex items-center">
                            <div class="w-6 h-6 gradient-bg rounded-full mr-3 flex items-center justify-center">
                                <svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                                </svg>
                            </div>
                            <span>Gas fees hampir nol ($0.0001 per transaksi)</span>
                        </li>
                        <li class="flex items-center">
                            <div class="w-6 h-6 gradient-bg rounded-full mr-3 flex items-center justify-center">
                                <svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                                </svg>
                            </div>
                            <span>Interoperabilitas dengan blockchain lainnya</span>
                        </li>
                    </ul>
                </div>
                <div class="relative">
                    <img src="https://placehold.co/600x400" alt="Visualisasi teknologi blockchain Phantom Coin menunjukkan node yang saling terhubung dengan garis-garis cahaya ungu dan biru pada latar belakang gelap" class="rounded-2xl w-full" />
                    <div class="absolute -inset-4 bg-gradient-to-r from-purple-600 to-blue-600 rounded-2xl opacity-20 blur-3xl -z-10"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- Get Started Section -->
    <section id="get-started" class="py-20 px-6">
        <div class="container mx-auto text-center">
            <h2 class="text-4xl font-bold mb-6">Mulai dengan Phantom Coin</h2>
            <p class="text-xl text-gray-300 mb-12 max-w-2xl mx-auto">
                Bergabunglah dengan revolusi cryptocurrency. Beli, simpan, dan gunakan Phantom Coin dengan mudah.
