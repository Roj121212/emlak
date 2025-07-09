<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Premium Immobilien | Professionelle Immobilienlösungen</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #005f73;
            --secondary: #0a9396;
            --accent: #94d2bd;
            --light: #e9d8a6;
            --dark: #001219;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
        }
        
        .property-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
        }
        
        .property-card {
            transition: all 0.3s ease;
        }
        
        .payment-method:hover {
            border-color: var(--secondary);
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .fade-in {
            animation: fadeIn 0.5s ease-in;
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="gradient-bg text-white shadow-lg">
        <div class="container mx-auto px-4 py-3">
            <div class="flex justify-between items-center">
                <div class="flex items-center space-x-4">
                    <i class="fas fa-home text-2xl"></i>
                    <h1 class="text-2xl font-bold">Premium Immobilien</h1>
                </div>
                <div class="hidden md:flex space-x-6">
                    <a href="#" class="hover:text-gray-200">Startseite</a>
                    <a href="#ilanlar" class="hover:text-gray-200">Immobilien</a>
                    <a href="#ekle" class="hover:text-gray-200">Anzeige aufgeben</a>
                    <a href="#iletisim" class="hover:text-gray-200">Kontakt</a>
                </div>
                <div class="flex items-center space-x-2 ml-6">
                    <select class="bg-transparent text-white border border-white rounded px-2 py-1">
                        <option value="de">DE</option>
                        <option value="en">EN</option>
                        <option value="fr">FR</option>
                        <option value="it">IT</option>
                    </select>
                </div>
                <button class="md:hidden text-2xl" id="mobile-menu-button">
                    <i class="fas fa-bars"></i>
                </button>
            </div>
        </div>
        <div class="md:hidden hidden px-4 py-2" id="mobile-menu">
            <a href="#" class="block py-2 hover:text-gray-200">Startseite</a>
            <a href="#ilanlar" class="block py-2 hover:text-gray-200">Immobilien</a>
            <a href="#ekle" class="block py-2 hover:text-gray-200">Inserat aufgeben</a>
            <a href="#iletisim" class="block py-2 hover:text-gray-200">Kontakt</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="gradient-bg text-white py-20">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-4xl font-bold mb-6">Finden Sie Ihr Traumhaus in der Schweiz</h2>
            <p class="text-xl mb-8 max-w-2xl mx-auto">Mit Premium Immobilien finden Sie einfach Miet- und Kaufobjekte in der ganzen Schweiz.</p>
            <div class="flex flex-wrap justify-center gap-4">
                <a href="#ilanlar" class="bg-white text-gray-800 font-bold py-3 px-6 rounded-full hover:bg-gray-100 transition duration-300">Immobilien ansehen</a>
                <a href="#ekle" class="border-2 border-white text-white font-bold py-3 px-6 rounded-full hover:bg-white hover:text-gray-800 transition duration-300">Anzeige aufgeben</a>
            </div>
        </div>
    </section>

    <!-- Search Section -->
    <section class="bg-gray-100 py-12">
        <div class="container mx-auto px-4">
            <div class="bg-white p-6 rounded-lg shadow-lg max-w-6xl mx-auto -mt-12">
                <form class="grid md:grid-cols-4 gap-4">
                    <div>
                        <label class="block text-gray-700 mb-2">Standort</label>
                        <input type="text" placeholder="Kanton, Stadt oder Ort" class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                    </div>
                    <div>
                        <label class="block text-gray-700 mb-2">Immobilientyp</label>
                        <select class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                            <option>Alle</option>
                            <option>Wohnung</option>
                            <option>Geschäft</option>
                            <option>Grundstück</option>
                            <option>Villa</option>
                        </select>
                    </div>
                    <div>
                        <label class="block text-gray-700 mb-2">Kategorie</label>
                        <select class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                            <option>Zu verkaufen</option>
                            <option>Zu mieten</option>
                        </select>
                    </div>
                    <div class="flex items-end">
                        <button class="gradient-bg text-white py-3 px-6 rounded-lg w-full hover:opacity-90 transition duration-300">
                            <i class="fas fa-search mr-2"></i> Ara
                        </button>
                    </div>
                </form>
            </div>
        </div>
    </section>

    <!-- Property Listing Section -->
    <section id="ilanlar" class="py-16">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Aktuelle Inserate</h2>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Property 1 -->
                <div class="property-card bg-white rounded-lg overflow-hidden shadow-lg fade-in">
                    <div class="relative">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/15b49325-134b-4e31-b758-4c63292f4a23.png" alt="Modern beyaz bina önünde yemyeşil çimler ve ağaçlar ile lüks apartman dairesi, İstanbul" class="w-full h-48 object-cover">
                        <div class="absolute top-2 left-2 bg-red-600 text-white px-3 py-1 rounded-full text-sm font-bold">ZU VERKAUFEN</div>
                    </div>
                    <div class="p-4">
                        <h3 class="text-xl font-bold mb-2">Luxuswohnung in Zürich</h3>
                        <p class="text-gray-600 mb-4"><i class="fas fa-map-marker-alt text-blue-500 mr-2"></i> Zürich, Schweiz</p>
                        <div class="flex justify-between text-gray-700 mb-4">
                            <span><i class="fas fa-bed text-blue-500 mr-1"></i> 3+1</span>
                            <span><i class="fas fa-ruler-combined text-blue-500 mr-1"></i> 140 m²</span>
                            <span><i class="fas fa-building text-blue-500 mr-1"></i> 2015</span>
                        </div>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-blue-800">CHF 2.500.000</span>
                            <button class="bg-blue-500 text-white px-4 py-2 rounded-lg hover:bg-blue-600 transition duration-300">Details</button>
                        </div>
                    </div>
                </div>

                <!-- Property 2 -->
                <div class="property-card bg-white rounded-lg overflow-hidden shadow-lg fade-in">
                    <div class="relative">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/beb3b21e-e695-44ce-9494-cc9f281f34b9.png" alt="Geniş yeşillikler içinde yer alan modern villa havuz manzaralı, Bodrum" class="w-full h-48 object-cover">
                        <div class="absolute top-2 left-2 bg-green-600 text-white px-3 py-1 rounded-full text-sm font-bold">ZU MIETEN</div>
                    </div>
                    <div class="p-4">
                        <h3 class="text-xl font-bold mb-2">Bodrum Deniz Manzaralı Villa</h3>
                        <p class="text-gray-600 mb-4"><i class="fas fa-map-marker-alt text-blue-500 mr-2"></i> Bodrum, Muğla</p>
                        <div class="flex justify-between text-gray-700 mb-4">
                            <span><i class="fas fa-bed text-blue-500 mr-1"></i> 5+2</span>
                            <span><i class="fas fa-ruler-combined text-blue-500 mr-1"></i> 320 m²</span>
                            <span><i class="fas fa-building text-blue-500 mr-1"></i> 2020</span>
                        </div>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-blue-800">15.000 TL/Ay</span>
                            <button class="bg-blue-500 text-white px-4 py-2 rounded-lg hover:bg-blue-600 transition duration-300">Detaylar</button>
                        </div>
                    </div>
                </div>

                <!-- Property 3 -->
                <div class="property-card bg-white rounded-lg overflow-hidden shadow-lg fade-in">
                    <div class="relative">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/c6093f1c-fe2c-4c38-9afe-37e21acca2b9.png" alt="Şehir merkezinde modern ofis binası geniş cam cepheli, Ankara" class="w-full h-48 object-cover">
                        <div class="absolute top-2 left-2 bg-red-600 text-white px-3 py-1 rounded-full text-sm font-bold">ZU VERKAUFEN</div>
                    </div>
                    <div class="p-4">
                        <h3 class="text-xl font-bold mb-2">Ankara Merkez Ofis Katı</h3>
                        <p class="text-gray-600 mb-4"><i class="fas fa-map-marker-alt text-blue-500 mr-2"></i> Çankaya, Ankara</p>
                        <div class="flex justify-between text-gray-700 mb-4">
                            <span><i class="fas fa-door-open text-blue-500 mr-1"></i> 6 Oda</span>
                            <span><i class="fas fa-ruler-combined text-blue-500 mr-1"></i> 180 m²</span>
                            <span><i class="fas fa-building text-blue-500 mr-1"></i> 2018</span>
                        </div>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-blue-800">4.200.000 TL</span>
                            <button class="bg-blue-500 text-white px-4 py-2 rounded-lg hover:bg-blue-600 transition duration-300">Detaylar</button>
                        </div>
                    </div>
                </div>
            </div>
            <div class="text-center mt-10">
                <button class="gradient-bg text-white px-6 py-3 rounded-lg hover:opacity-90 transition duration-300">
                    Alle Inserate anzeigen <i class="fas fa-arrow-right ml-2"></i>
                </button>
            </div>
        </div>
    </section>

    <!-- Add Listing Section -->
    <section id="ekle" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Inserat aufgeben</h2>
            <div class="max-w-4xl mx-auto bg-white rounded-lg shadow-lg overflow-hidden">
                <div class="grid md:grid-cols-2">
                    <div class="p-8 gradient-bg text-white flex flex-col justify-center">
                        <h3 class="text-2xl font-bold mb-4">Premium Inserat-Vorteile</h3>
                        <ul class="space-y-3">
                            <li class="flex items-center"><i class="fas fa-check-circle mr-2"></i> 500.000+ potenzielle Käufer</li>
                            <li class="flex items-center"><i class="fas fa-check-circle mr-2"></i> Hervorgehobene Platzierung</li>
                            <li class="flex items-center"><i class="fas fa-check-circle mr-2"></i> Professionelle Fotografie</li>
                            <li class="flex items-center"><i class="fas fa-check-circle mr-2"></i> Social-Media-Werbung</li>
                        </ul>
                        <div class="mt-8 bg-white text-gray-800 p-4 rounded-lg">
                            <h4 class="font-bold mb-2">İlan Ücretleri</h4>
                            <p class="text-sm">Standard-Inserat: <span class="font-bold">99 CHF</span></p>
                            <p class="text-sm">Premium-Inserat: <span class="font-bold">199 CHF</span> (30 Tage)</p>
                            <p class="text-sm">VIP-Inserat: <span class="font-bold">299 CHF</span> (60 Tage + Aktionen)</p>
                        </div>
                    </div>
                    <div class="p-8">
                        <h3 class="text-xl font-bold mb-6">Inserat Informationen</h3>
                        <form id="listing-form">
                            <div class="mb-4">
                                <label class="block text-gray-700 mb-2">Inserat Titel*</label>
                                <input type="text" class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                            </div>
                            <div class="mb-4">
                                <label class="block text-gray-700 mb-2">Immobilientyp*</label>
                                <select class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                                    <option value="">Seçiniz</option>
                                    <option>Konut</option>
                                    <option>Villa</option>
                                    <option>İşyeri</option>
                                    <option>Arsa</option>
                                    <option>Turizm Tesisi</option>
                                </select>
                            </div>
                            <div class="mb-4">
                                <label class="block text-gray-700 mb-2">Kategorie*</label>
                                <select class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                                    <option value="">Seçiniz</option>
                                    <option>Satılık</option>
                                    <option>Kiralık</option>
                                    <option>Günlük Kiralık</option>
                                </select>
                            </div>
                            <div class="mb-4">
                                <label class="block text-gray-700 mb-2">Fotoğraf Yükle (Max 10 MB)</label>
                                <div class="border-2 border-dashed border-gray-300 rounded-lg p-4 text-center">
                                    <input type="file" class="hidden" id="photo-upload" multiple>
                                    <label for="photo-upload" class="cursor-pointer">
                                        <i class="fas fa-cloud-upload-alt text-4xl text-gray-400 mb-2"></i>
                                        <p class="text-gray-500">Fotos ziehen und ablegen oder hier klicken</p>
                                    </label>
                                </div>
                            </div>
                            <button type="button" id="next-btn" class="gradient-bg text-white w-full py-3 rounded-lg hover:opacity-90 transition duration-300 mt-4">Weiter</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Payment Modal -->
    <div id="payment-modal" class="hidden fixed inset-0 bg-black bg-opacity-50 z-50 flex items-center justify-center p-4">
        <div class="bg-white rounded-lg max-w-2xl w-full overflow-hidden">
            <div class="flex justify-between items-center p-4 border-b">
                <h3 class="text-xl font-bold">Zahlungsvorgang</h3>
                <button id="close-modal" class="text-gray-500 hover:text-gray-700">
                    <i class="fas fa-times"></i>
                </button>
            </div>
            <div class="p-6">
                <div class="grid md:grid-cols-2 gap-8">
                    <div>
                        <h4 class="font-bold mb-4">Sipariş Özeti</h4>
                        <div class="bg-gray-50 p-4 rounded-lg mb-6">
                            <div class="flex justify-between mb-2">
                                <span>İlan Paketi:</span>
                                <span class="font-bold" id="package-name">Premium İlan</span>
                            </div>
                            <div class="flex justify-between mb-2">
                                <span>Dauer:</span>
                                <span class="font-bold">30 Tage</span>
                            </div>
                            <div class="flex justify-between border-t pt-2 mt-2">
                                <span>Toplam:</span>
                                <span class="font-bold text-lg" id="total-amount">199 TL</span>
                            </div>
                        </div>
                        <div class="mb-6">
                            <h4 class="font-bold mb-3">Ödeme Yöntemi</h4>
                            <div class="space-y-3">
                                <label class="payment-method flex items-center p-3 border rounded-lg cursor-pointer">
                                    <input type="radio" name="payment" checked class="mr-3">
                                    <div>
                                        <span class="font-bold">Kredit-/Bankkarte</span>
                                        <div class="flex mt-2">
                                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/dd4485dd-2a15-4a53-a032-0094b826d847.png" alt="Visa kart logosu" class="mr-2">
                                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/ea53bf37-295c-4625-8525-8ebc112e0241.png" alt="Mastercard logosu" class="mr-2">
                                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/c972fa89-2a3d-488a-92d7-764279961f37.png" alt="Troy kart logosu">
                                        </div>
                                    </div>
                                </label>
                                <label class="payment-method flex items-center p-3 border rounded-lg cursor-pointer">
                                    <input type="radio" name="payment" class="mr-3">
                                    <div>
                                        <span class="font-bold">PayPal</span>
                                    </div>
                                </label>
                                <label class="payment-method flex items-center p-3 border rounded-lg cursor-pointer">
                                    <input type="radio" name="payment" class="mr-3">
                                    <div>
                                        <span class="font-bold">Überweisung</span>
                                    </div>
                                </label>
                            </div>
                        </div>
                    </div>
                    <div>
                        <h4 class="font-bold mb-4">Kart Bilgileri</h4>
                        <form id="payment-form">
                            <div class="mb-4">
                                <label class="block text-gray-700 mb-2">Kart Sahibi</label>
                                <input type="text" placeholder="Kart üzerindeki isim" class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                            </div>
                            <div class="mb-4">
                                <label class="block text-gray-700 mb-2">Kart Numarası</label>
                                <input type="text" placeholder="1234 5678 9012 3456" class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                            </div>
                            <div class="grid grid-cols-2 gap-4 mb-4">
                                <div>
                                    <label class="block text-gray-700 mb-2">Son Kullanma Tarihi</label>
                                    <input type="text" placeholder="MM/YY" class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                                </div>
                                <div>
                                    <label class="block text-gray-700 mb-2">CVV</label>
                                    <input type="text" placeholder="123" class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                                </div>
                            </div>
                            <button type="submit" class="gradient-bg text-white w-full py-3 rounded-lg hover:opacity-90 transition duration-300">
                                Zahlung abschließen <i class="fas fa-lock ml-2"></i>
                            </button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>

    <!-- Contact Section -->
    <section id="iletisim" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Kontakt</h2>
            <div class="max-w-4xl mx-auto grid md:grid-cols-2 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">Bize Ulaşın</h3>
                    <form>
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">Vorname und Name</label>
                            <input type="text" class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                        </div>
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">E-posta Adresiniz</label>
                            <input type="email" class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                        </div>
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">Mesajınız</label>
                            <textarea rows="5" class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" required></textarea>
                        </div>
                        <button type="submit" class="gradient-bg text-white px-6 py-3 rounded-lg hover:opacity-90 transition duration-300">Senden</button>
                    </form>
                </div>
                <div>
                    <h3 class="text-xl font-bold mb-4">İletişim Bilgileri</h3>
                    <div class="bg-gray-50 p-6 rounded-lg">
                        <div class="flex items-start mb-4">
                            <i class="fas fa-map-marker-alt text-blue-500 mt-1 mr-3"></i>
                            <div>
                                <h4 class="font-bold">Adres</h4>
                                <p class="text-gray-600">Bahnhofstrasse 123<br>8001 Zürich, Schweiz</p>
                            </div>
                        </div>
                        <div class="flex items-start mb-4">
                            <i class="fas fa-phone-alt text-blue-500 mt-1 mr-3"></i>
                            <div>
                                <h4 class="font-bold">Telefon</h4>
                                <p class="text-gray-600">+90 212 123 45 67</p>
                            </div>
                        </div>
                        <div class="flex items-start mb-4">
                            <i class="fas fa-envelope text-blue-500 mt-1 mr-3"></i>
                            <div>
                                <h4 class="font-bold">E-posta</h4>
                                <p class="text-gray-600">info@premiumemlak.com</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <i class="fas fa-clock text-blue-500 mt-1 mr-3"></i>
                            <div>
                                <h4 class="font-bold">Çalışma Saatleri</h4>
                                <p class="text-gray-600">Pazartesi-Cuma: 09:00-18:00</p>
                            </div>
                        </div>
                    </div>
                    <div class="mt-6">
                        <h4 class="font-bold mb-3">Sosyal Medya</h4>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-blue-600 text-white p-3 rounded-full hover:bg-blue-700 transition duration-300"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="bg-blue-400 text-white p-3 rounded-full hover:bg-blue-500 transition duration-300"><i class="fab fa-twitter"></i></a>
                            <a href="#" class="bg-pink-600 text-white p-3 rounded-full hover:bg-pink-700 transition duration-300"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="bg-blue-800 text-white p-3 rounded-full hover:bg-blue-900 transition duration-300"><i class="fab fa-linkedin-in"></i></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">Premium Immobilien</h3>
                    <p>Wir sind eines der führenden Immobilienportale der Schweiz. Wir helfen Ihnen, Ihr Traumhaus zu finden.</p>
                </div>
                <div>
                    <h4 class="font-bold mb-4">Hızlı Linkler</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="hover:text-blue-400 transition duration-300">Startseite</a></li>
                        <li><a href="#ilanlar" class="hover:text-blue-400 transition duration-300">Immobilien</a></li>
                        <li><a href="#ekle" class="hover:text-blue-400 transition duration-300">Inserat</a></li>
                        <li><a href="#iletisim" class="hover:text-blue-400 transition duration-300">Kontakt</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-4">Emlak Hizmetleri</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="hover:text-blue-400 transition duration-300">Emlak Danışmanlığı</a></li>
                        <li><a href="#" class="hover:text-blue-400 transition duration-300">Proje Danışmanlığı</a></li>
                        <li><a href="#" class="hover:text-blue-400 transition duration-300">Hukuki Danışmanlık</a></li>
                        <li><a href="#" class="hover:text-blue-400 transition duration-300">Kredi Danışmanlığı</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-4">E-Bülten</h4>
                    <p>Yeni ilanlardan haberdar olmak için e-posta listemize kaydolun.</p>
                    <form class="mt-4">
                        <div class="flex">
                            <input type="email" placeholder="E-posta adresiniz" class="p-2 rounded-l-lg w-full focus:outline-none text-gray-800">
                            <button class="gradient-bg px-4 rounded-r-lg hover:opacity-90 transition duration-300">
                                <i class="fas fa-paper-plane"></i>
                            </button>
                        </div>
                    </form>
                </div>
            </div>
            <div class="border-t border-gray-800 mt-10 pt-6 text-center text-gray-400">
                <p>© 2023 Premium Immobilien Schweiz. Alle Rechte vorbehalten.</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });

        // Listing Form Next Button
        document.getElementById('next-btn').addEventListener('click', function() {
            const form = document.getElementById('listing-form');
            const isValid = form.checkValidity();
            
            if (isValid) {
                document.getElementById('payment-modal').classList.remove('hidden');
            } else {
                form.reportValidity();
            }
        });

        // Close Modal
        document.getElementById('close-modal').addEventListener('click', function() {
            document.getElementById('payment-modal').classList.add('hidden');
        });

        // Payment Form Submission
        document.getElementById('payment-form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Simulate payment processing
            setTimeout(function() {
                alert('Ihre Zahlung wurde erfolgreich erhalten! Ihre Anzeige wird veröffentlicht.');
                document.getElementById('payment-modal').classList.add('hidden');
                document.getElementById('listing-form').reset();
            }, 1500);
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Animation on scroll
        function fadeInOnScroll() {
            const elements = document.querySelectorAll('.fade-in');
            
            elements.forEach(element => {
                const elementTop = element.getBoundingClientRect().top;
                const windowHeight = window.innerHeight;
                
                if (elementTop < windowHeight - 100) {
                    element.style.opacity = '1';
                }
            });
        }

        window.addEventListener('scroll', fadeInOnScroll);
        window.addEventListener('load', fadeInOnScroll);
    </script>
</body>
</html>

