<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wasal - UAE's Unified Delivery Platform</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }
        .gradient-bg {
            background: linear-gradient(135deg, #4776E6 0%, #8E54E9 100%);
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        .feature-icon {
            background: linear-gradient(135deg, #4776E6 0%, #8E54E9 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .nav-link {
            position: relative;
        }
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -2px;
            left: 0;
            background-color: #8E54E9;
            transition: width 0.3s ease;
        }
        .nav-link:hover::after {
            width: 100%;
        }
        .btn-primary {
            background: linear-gradient(135deg, #4776E6 0%, #8E54E9 100%);
            transition: all 0.3s ease;
        }
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(142, 84, 233, 0.4);
        }
        .btn-outline {
            border: 2px solid #8E54E9;
            color: #8E54E9;
            transition: all 0.3s ease;
        }
        .btn-outline:hover {
            background: linear-gradient(135deg, #4776E6 0%, #8E54E9 100%);
            color: white;
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Navigation -->
    <nav class="bg-white shadow-sm fixed w-full z-10">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center">
                <div class="text-2xl font-bold gradient-bg text-transparent bg-clip-text">Wasal</div>
            </div>
            <div class="hidden md:flex space-x-8">
                <a href="#home" class="nav-link font-medium text-gray-700 hover:text-purple-600">Home</a>
                <a href="#personal" class="nav-link font-medium text-gray-700 hover:text-purple-600">Personal</a>
                <a href="#business" class="nav-link font-medium text-gray-700 hover:text-purple-600">Business</a>
                <a href="#contact" class="nav-link font-medium text-gray-700 hover:text-purple-600">Contact</a>
            </div>
            <div class="flex items-center space-x-4">
                <button class="hidden md:block px-4 py-2 rounded-full btn-outline">Login</button>
                <button class="px-4 py-2 rounded-full text-white btn-primary">Get Started</button>
            </div>
            <div class="md:hidden flex items-center">
                <button id="mobile-menu-button" class="text-gray-500 hover:text-gray-700 focus:outline-none">
                    <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
        </div>
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t">
            <div class="container mx-auto px-4 py-2 space-y-2">
                <a href="#home" class="block py-2 text-gray-700 hover:text-purple-600">Home</a>
                <a href="#personal" class="block py-2 text-gray-700 hover:text-purple-600">Personal</a>
                <a href="#business" class="block py-2 text-gray-700 hover:text-purple-600">Business</a>
                <a href="#contact" class="block py-2 text-gray-700 hover:text-purple-600">Contact</a>
                <button class="block w-full text-left py-2 text-gray-700 hover:text-purple-600">Login</button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="pt-24 pb-16 md:pt-32 md:pb-24 gradient-bg">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 text-center md:text-left text-white mb-8 md:mb-0">
                    <h1 class="text-3xl md:text-5xl font-bold mb-6">The UAE's Unified Delivery Platform</h1>
                    <p class="text-lg md:text-xl mb-8 opacity-90">Bringing together all major delivery services under one app. Find the most suitable delivery provider based on location, item size, transport type, and cost.</p>
                    <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4 justify-center md:justify-start">
                        <button class="px-8 py-3 bg-white text-purple-600 font-semibold rounded-full hover:bg-gray-100 transition duration-300 shadow-lg">Get Started</button>
                        <button class="px-8 py-3 border-2 border-white text-white font-semibold rounded-full hover:bg-white hover:bg-opacity-10 transition duration-300">Learn More</button>
                    </div>
                </div>
                <div class="md:w-1/2">
                    <div class="relative">
                        <!-- Hero SVG Illustration -->
                        <svg class="w-full h-auto" viewBox="0 0 600 400" xmlns="http://www.w3.org/2000/svg">
                            <defs>
                                <linearGradient id="phoneGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                                    <stop offset="0%" stop-color="#ffffff" stop-opacity="0.9"/>
                                    <stop offset="100%" stop-color="#f0f0f0" stop-opacity="0.9"/>
                                </linearGradient>
                            </defs>
                            <!-- Background elements -->
                            <circle cx="150" cy="150" r="80" fill="#ffffff" fill-opacity="0.1"/>
                            <circle cx="450" cy="250" r="60" fill="#ffffff" fill-opacity="0.1"/>
                            <circle cx="300" cy="100" r="40" fill="#ffffff" fill-opacity="0.1"/>
                            
                            <!-- Phone -->
                            <rect x="200" y="50" width="200" height="350" rx="20" fill="url(#phoneGrad)" stroke="#ffffff" stroke-width="2"/>
                            <rect x="220" y="80" width="160" height="280" rx="5" fill="#4776E6" fill-opacity="0.9"/>
                            
                            <!-- Phone elements -->
                            <circle cx="300" cy="65" r="5" fill="#ffffff"/>
                            <rect x="240" y="100" width="120" height="40" rx="5" fill="#ffffff" fill-opacity="0.9"/>
                            <rect x="240" y="150" width="120" height="30" rx="5" fill="#ffffff" fill-opacity="0.7"/>
                            <rect x="240" y="190" width="120" height="30" rx="5" fill="#ffffff" fill-opacity="0.7"/>
                            <rect x="240" y="230" width="120" height="30" rx="5" fill="#ffffff" fill-opacity="0.7"/>
                            <rect x="240" y="270" width="120" height="40" rx="5" fill="#ffffff" fill-opacity="0.9"/>
                            <circle cx="300" cy="340" r="15" fill="#ffffff" stroke="#4776E6" stroke-width="2"/>
                            
                            <!-- Delivery elements -->
                            <circle cx="450" cy="150" r="30" fill="#ffffff" fill-opacity="0.9"/>
                            <path d="M435,150 L465,150 M450,135 L450,165" stroke="#4776E6" stroke-width="4" stroke-linecap="round"/>
                            
                            <circle cx="150" cy="250" r="30" fill="#ffffff" fill-opacity="0.9"/>
                            <path d="M135,250 L165,250 M150,235 L150,265" stroke="#4776E6" stroke-width="4" stroke-linecap="round"/>
                            
                            <!-- Connection lines -->
                            <path d="M300,150 C350,150 400,150 450,150" stroke="#ffffff" stroke-width="2" stroke-dasharray="5,5"/>
                            <path d="M300,250 C250,250 200,250 150,250" stroke="#ffffff" stroke-width="2" stroke-dasharray="5,5"/>
                        </svg>
                    </div>
                </div>
            </div>
        </div>
        <div class="absolute bottom-0 left-0 right-0">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 120">
                <path fill="#ffffff" fill-opacity="1" d="M0,64L80,69.3C160,75,320,85,480,80C640,75,800,53,960,48C1120,43,1280,53,1360,58.7L1440,64L1440,120L1360,120C1280,120,1120,120,960,120C800,120,640,120,480,120C320,120,160,120,80,120L0,120Z"></path>
            </svg>
        </div>
    </section>

    <!-- Personal Section -->
    <section id="personal" class="py-16 md:py-24 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Wasal – For Everyone</h2>
                <p class="text-xl text-gray-600 font-medium">Fast. Easy. Smart.</p>
                <div class="w-20 h-1 bg-purple-600 mx-auto mt-6"></div>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-white rounded-xl shadow-lg p-6 transition-all duration-300 card-hover">
                    <div class="text-4xl mb-4 feature-icon">📍</div>
                    <h3 class="text-xl font-semibold mb-3">Instant Delivery Matching</h3>
                    <p class="text-gray-600">Set the pickup and drop-off locations, choose the item size, and get a list of available delivery services based on price and ETA.</p>
                </div>
                
                <div class="bg-white rounded-xl shadow-lg p-6 transition-all duration-300 card-hover">
                    <div class="text-4xl mb-4 feature-icon">🚚</div>
                    <h3 class="text-xl font-semibold mb-3">Diverse Transport Options</h3>
                    <p class="text-gray-600">From motorcycles to refrigerated vans and floral transports, we have the right vehicle for your delivery needs.</p>
                </div>
                
                <div class="bg-white rounded-xl shadow-lg p-6 transition-all duration-300 card-hover">
                    <div class="text-4xl mb-4 feature-icon">💸</div>
                    <h3 class="text-xl font-semibold mb-3">Smart Pricing Suggestions</h3>
                    <p class="text-gray-600">Let Wasal recommend the best value options from trusted providers based on your specific needs.</p>
                </div>
                
                <div class="bg-white rounded-xl shadow-lg p-6 transition-all duration-300 card-hover">
                    <div class="text-4xl mb-4 feature-icon">⭐</div>
                    <h3 class="text-xl font-semibold mb-3">Review & Track</h3>
                    <p class="text-gray-600">Follow your order in real-time and leave feedback for your delivery experience to help improve the service.</p>
                </div>
                
                <div class="bg-white rounded-xl shadow-lg p-6 transition-all duration-300 card-hover">
                    <div class="text-4xl mb-4 feature-icon">🔒</div>
                    <h3 class="text-xl font-semibold mb-3">No Drivers Needed</h3>
                    <p class="text-gray-600">You focus on sending, we handle the logistics. Let us take care of finding the right delivery partner.</p>
                </div>
                
                <div class="bg-gradient-to-br from-purple-600 to-blue-500 rounded-xl shadow-lg p-6 text-white flex flex-col justify-between">
                    <div>
                        <h3 class="text-xl font-semibold mb-3">Ready to send something?</h3>
                        <p class="mb-6">Whether it's a forgotten wallet, birthday cake, or flower bouquet, Wasal makes sure it gets there fast, affordably, and securely.</p>
                    </div>
                    <button class="bg-white text-purple-600 font-semibold py-3 px-6 rounded-full hover:bg-gray-100 transition duration-300 shadow-lg">Get Started Now</button>
                </div>
            </div>
            
            <div class="mt-16 bg-gray-50 rounded-2xl p-8 shadow-inner">
                <div class="flex flex-col md:flex-row items-center">
                    <div class="md:w-1/2 mb-8 md:mb-0">
                        <!-- App showcase SVG -->
                        <svg class="w-full max-w-md mx-auto" viewBox="0 0 400 300" xmlns="http://www.w3.org/2000/svg">
                            <!-- Phone outline -->
                            <rect x="125" y="20" width="150" height="260" rx="15" fill="#f8f9fa" stroke="#4776E6" stroke-width="2"/>
                            <rect x="135" y="40" width="130" height="220" rx="5" fill="#ffffff"/>
                            
                            <!-- App header -->
                            <rect x="135" y="40" width="130" height="40" rx="5" fill="#4776E6"/>
                            <text x="200" y="65" font-family="Arial" font-size="14" fill="white" text-anchor="middle">Wasal</text>
                            
                            <!-- Map view -->
                            <rect x="145" y="90" width="110" height="80" rx="5" fill="#e9ecef"/>
                            <circle cx="180" cy="120" r="5" fill="#4776E6"/>
                            <circle cx="220" cy="140" r="5" fill="#8E54E9"/>
                            <path d="M180,120 Q200,110 220,140" stroke="#4776E6" stroke-width="2" fill="none"/>
                            
                            <!-- Delivery options -->
                            <rect x="145" y="180" width="110" height="25" rx="5" fill="#f8f9fa" stroke="#e9ecef" stroke-width="1"/>
                            <text x="165" y="197" font-family="Arial" font-size="10" fill="#495057">Motorcycle</text>
                            <text x="235" y="197" font-family="Arial" font-size="10" fill="#4776E6" text-anchor="end">15 AED</text>
                            
                            <rect x="145" y="210" width="110" height="25" rx="5" fill="#f8f9fa" stroke="#e9ecef" stroke-width="1"/>
                            <text x="165" y="227" font-family="Arial" font-size="10" fill="#495057">Car</text>
                            <text x="235" y="227" font-family="Arial" font-size="10" fill="#4776E6" text-anchor="end">25 AED</text>
                            
                            <!-- Button -->
                            <rect x="155" y="245" width="90" height="30" rx="15" fill="#4776E6"/>
                            <text x="200" y="265" font-family="Arial" font-size="12" fill="white" text-anchor="middle">Book Now</text>
                            
                            <!-- Phone elements -->
                            <circle cx="200" y="30" r="3" fill="#e9ecef"/>
                            <rect x="175" y="275" width="50" height="5" rx="2.5" fill="#e9ecef"/>
                        </svg>
                    </div>
                    <div class="md:w-1/2 md:pl-8">
                        <h3 class="text-2xl font-bold mb-4">Download the Wasal App</h3>
                        <p class="text-gray-600 mb-6">Experience the convenience of Wasal on your smartphone. Track deliveries, compare prices, and manage your shipments on the go.</p>
                        <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
                            <button class="flex items-center justify-center bg-black text-white py-3 px-6 rounded-lg">
                                <svg class="w-6 h-6 mr-2" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M17.5,2H8.5C6.6,2,5,3.6,5,5.5v13C5,20.4,6.6,22,8.5,22h9c1.9,0,3.5-1.6,3.5-3.5v-13C21,3.6,19.4,2,17.5,2z M13,20h-2v-1h2V20z M18,16H8V5h10V16z"/>
                                </svg>
                                App Store
                            </button>
                            <button class="flex items-center justify-center bg-black text-white py-3 px-6 rounded-lg">
                                <svg class="w-6 h-6 mr-2" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M3.9,12c0-3.1,2.5-5.6,5.6-5.6h5c3.1,0,5.6,2.5,5.6,5.6v0c0,3.1-2.5,5.6-5.6,5.6h-5C6.4,17.6,3.9,15.1,3.9,12L3.9,12z M12,8.4c-2,0-3.6,1.6-3.6,3.6s1.6,3.6,3.6,3.6s3.6-1.6,3.6-3.6S14,8.4,12,8.4z"/>
                                </svg>
                                Google Play
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Business Section -->
    <section id="business" class="py-16 md:py-24 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Wasal Business – Delivery, Optimized</h2>
                <p class="text-xl text-gray-600 font-medium">Built for Small Businesses, Delivery Companies & Drivers</p>
                <div class="w-20 h-1 bg-purple-600 mx-auto mt-6"></div>
            </div>
            
            <div class="flex flex-col md:flex-row space-y-8 md:space-y-0 md:space-x-8">
                <div class="md:w-1/3 bg-white rounded-xl shadow-lg overflow-hidden">
                    <div class="h-2 bg-blue-500"></div>
                    <div class="p-6">
                        <div class="text-2xl font-bold text-blue-500 mb-4">For Small Businesses</div>
                        <ul class="space-y-4">
                            <li class="flex items-start">
                                <div class="text-blue-500 mr-3">📦</div>
                                <div>
                                    <span class="font-semibold">Integrated Order Management</span>
                                    <p class="text-gray-600 text-sm mt-1">Schedule, assign, and track orders easily.</p>
                                </div>
                            </li>
                            <li class="flex items-start">
                                <div class="text-blue-500 mr-3">🖨️</div>
                                <div>
                                    <span class="font-semibold">QR Sticker Machines</span>
                                    <p class="text-gray-600 text-sm mt-1">Rent or buy our smart sticker machines to label and monitor every delivery.</p>
                                </div>
                            </li>
                            <li class="flex items-start">
                                <div class="text-blue-500 mr-3">📊</div>
                                <div>
                                    <span class="font-semibold">Analytics & Feedback Dashboard</span>
                                    <p class="text-gray-600 text-sm mt-1">View top-performing delivery partners and customer satisfaction ratings.</p>
                                </div>
                            </li>
                            <li class="flex items-start">
                                <div class="text-blue-500 mr-3">🔄</div>
                                <div>
                                    <span class="font-semibold">Flexible Service Selection</span>
                                    <p class="text-gray-600 text-sm mt-1">Choose refrigerated, floral, or general transport as needed.</p>
                                </div>
                            </li>
                        </ul>
                        <button class="w-full mt-6 py-3 bg-blue-500 text-white font-semibold rounded-lg hover:bg-blue-600 transition duration-300">Learn More</button>
                    </div>
                </div>
                
                <div class="md:w-1/3 bg-white rounded-xl shadow-lg overflow-hidden">
                    <div class="h-2 bg-purple-600"></div>
                    <div class="p-6">
                        <div class="text-2xl font-bold text-purple-600 mb-4">For Delivery Companies</div>
                        <ul class="space-y-4">
                            <li class="flex items-start">
                                <div class="text-purple-600 mr-3">📈</div>
                                <div>
                                    <span class="font-semibold">Business Growth</span>
                                    <p class="text-gray-600 text-sm mt-1">Get listed and gain access to a broader customer base through our platform.</p>
                                </div>
                            </li>
                            <li class="flex items-start">
                                <div class="text-purple-600 mr-3">🧾</div>
                                <div>
                                    <span class="font-semibold">Live Order Tracking</span>
                                    <p class="text-gray-600 text-sm mt-1">Assign orders to drivers, track status, and view historical performance.</p>
                                </div>
                            </li>
                            <li class="flex items-start">
                                <div class="text-purple-600 mr-3">🌟</div>
                                <div>
                                    <span class="font-semibold">Customer Ratings & Insights</span>
                                    <p class="text-gray-600 text-sm mt-1">Access reviews and data to improve your services.</p>
                                </div>
                            </li>
                        </ul>
                        <button class="w-full mt-6 py-3 bg-purple-600 text-white font-semibold rounded-lg hover:bg-purple-700 transition duration-300">Partner With Us</button>
                    </div>
                </div>
                
                <div class="md:w-1/3 bg-white rounded-xl shadow-lg overflow-hidden">
                    <div class="h-2 bg-green-500"></div>
                    <div class="p-6">
                        <div class="text-2xl font-bold text-green-500 mb-4">For Drivers</div>
                        <ul class="space-y-4">
                            <li class="flex items-start">
                                <div class="text-green-500 mr-3">🚴</div>
                                <div>
                                    <span class="font-semibold">Driver Portal</span>
                                    <p class="text-gray-600 text-sm mt-1">View assigned deliveries, earnings, performance metrics, and customer feedback.</p>
                                </div>
                            </li>
                            <li class="flex items-start">
                                <div class="text-green-500 mr-3">🧑‍💼</div>
                                <div>
                                    <span class="font-semibold">Company Integration</span>
                                    <p class="text-gray-600 text-sm mt-1">Drivers operate under their assigned companies, ensuring efficiency and accountability.</p>
                                </div>
                            </li>
                        </ul>
                        <button class="w-full mt-6 py-3 bg-green-500 text-white font-semibold rounded-lg hover:bg-green-600 transition duration-300">Join As Driver</button>
                    </div>
                </div>
            </div>
            
            <div class="mt-16">
                <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
                    <div class="flex flex-col md:flex-row">
                        <div class="md:w-1/2 p-8 md:p-12">
                            <h3 class="text-2xl font-bold mb-4">Wasal Business Dashboard</h3>
                            <p class="text-gray-600 mb-6">Our intuitive dashboard gives you complete control over your delivery operations. Monitor performance, manage orders, and grow your business with powerful analytics.</p>
                            <ul class="space-y-3 mb-8">
                                <li class="flex items-center">
                                    <svg class="w-5 h-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                                    </svg>
                                    Real-time order tracking
                                </li>
                                <li class="flex items-center">
                                    <svg class="w-5 h-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                                    </svg>
                                    Comprehensive analytics
                                </li>
                                <li class="flex items-center">
                                    <svg class="w-5 h-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                                    </svg>
                                    Customer feedback management
                                </li>
                                <li class="flex items-center">
                                    <svg class="w-5 h-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                                    </svg>
                                    Automated reporting
                                </li>
                            </ul>
                            <button class="px-8 py-3 bg-gradient-to-r from-purple-600 to-blue-500 text-white font-semibold rounded-lg hover:from-purple-700 hover:to-blue-600 transition duration-300 shadow-md">Join Wasal Business Today</button>
                        </div>
                        <div class="md:w-1/2 bg-gray-50 p-8 flex items-center justify-center">
                            <!-- Dashboard SVG -->
                            <svg class="w-full max-w-md" viewBox="0 0 500 300" xmlns="http://www.w3.org/2000/svg">
                                <!-- Dashboard background -->
                                <rect x="50" y="20" width="400" height="260" rx="10" fill="#ffffff" stroke="#e0e0e0" stroke-width="2"/>
                                
                                <!-- Sidebar -->
                                <rect x="50" y="20" width="80" height="260" fill="#4776E6"/>
                                <circle cx="90" cy="50" r="15" fill="#ffffff" fill-opacity="0.2"/>
                                <rect x="70" y="80" width="40" height="5" rx="2" fill="#ffffff" fill-opacity="0.6"/>
                                <rect x="70" y="100" width="40" height="5" rx="2" fill="#ffffff" fill-opacity="0.6"/>
                                <rect x="70" y="120" width="40" height="5" rx="2" fill="#ffffff" fill-opacity="0.6"/>
                                <rect x="70" y="140" width="40" height="5" rx="2" fill="#ffffff" fill-opacity="0.6"/>
                                <rect x="70" y="160" width="40" height="5" rx="2" fill="#ffffff" fill-opacity="0.6"/>
                                
                                <!-- Header -->
                                <rect x="130" y="20" width="320" height="50" fill="#f8f9fa"/>
                                <rect x="150" y="42.5" width="120" height="5" rx="2" fill="#495057"/>
                                <circle cx="430" cy="45" r="15" fill="#e9ecef"/>
                                
                                <!-- Main content -->
                                <rect x="150" y="90" width="120" height="80" rx="5" fill="#e9ecef"/>
                                <rect x="160" y="100" width="100" height="10" rx="2" fill="#adb5bd"/>
                                <rect x="160" y="120" width="60" height="40" rx="2" fill="#4776E6"/>
                                
                                <rect x="290" y="90" width="120" height="80" rx="5" fill="#e9ecef"/>
                                <rect x="300" y="100" width="100" height="10" rx="2" fill="#adb5bd"/>
                                <rect x="300" y="120" width="40" height="40" rx="2" fill="#8E54E9"/>
                                <rect x="350" y="120" width="50" height="40" rx="2" fill="#8E54E9" fill-opacity="0.6"/>
                                
                                <rect x="150" y="190" width="260" height="70" rx="5" fill="#e9ecef"/>
                                <rect x="160" y="200" width="240" height="10" rx="2" fill="#adb5bd"/>
                                <rect x="160" y="220" width="240" height="5" rx="2" fill="#ced4da"/>
                                <rect x="160" y="235" width="240" height="5" rx="2" fill="#ced4da"/>
                                <rect x="160" y="250" width="240" height="5" rx="2" fill="#ced4da"/>
                            </svg>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="py-16 md:py-24 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">What Our Users Say</h2>
                <p class="text-xl text-gray-600">Join thousands of satisfied users across the UAE</p>
                <div class="w-20 h-1 bg-purple-600 mx-auto mt-6"></div>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-gray-50 rounded-xl p-6 shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gradient-to-br from-blue-500 to-purple-600 flex items-center justify-center text-white font-bold text-xl">S</div>
                        <div class="ml-4">
                            <div class="font-semibold">Sarah A.</div>
                            <div class="text-sm text-gray-500">Dubai</div>
                        </div>
                    </div>
                    <div class="mb-4">
                        <div class="flex text-yellow-400">
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                        </div>
                    </div>
                    <p class="text-gray-600">"Wasal saved me when I needed to send an important document across town urgently. The app found me the fastest courier at the best price. Will definitely use again!"</p>
                </div>
                
                <div class="bg-gray-50 rounded-xl p-6 shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gradient-to-br from-blue-500 to-purple-600 flex items-center justify-center text-white font-bold text-xl">M</div>
                        <div class="ml-4">
                            <div class="font-semibold">Mohammed K.</div>
                            <div class="text-sm text-gray-500">Abu Dhabi</div>
                        </div>
                    </div>
                    <div class="mb-4">
                        <div class="flex text-yellow-400">
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                        </div>
                    </div>
                    <p class="text-gray-600">"As a small business owner, Wasal Business has transformed how we handle deliveries. The dashboard is intuitive and the analytics help us make better decisions. Highly recommended!"</p>
                </div>
                
                <div class="bg-gray-50 rounded-xl p-6 shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gradient-to-br from-blue-500 to-purple-600 flex items-center justify-center text-white font-bold text-xl">L</div>
                        <div class="ml-4">
                            <div class="font-semibold">Layla R.</div>
                            <div class="text-sm text-gray-500">Sharjah</div>
                        </div>
                    </div>
                    <div class="mb-4">
                        <div class="flex text-yellow-400">
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                        </div>
                    </div>
                    <p class="text-gray-600">"I needed to send a refrigerated cake for my sister's birthday. Wasal found me a specialized transport option I didn't even know existed! The cake arrived perfect and on time."</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 md:py-24 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
                    <h2 class="text-3xl font-bold mb-6">Get in Touch</h2>
                    <p class="text-gray-600 mb-8">Have questions about Wasal? Want to partner with us? Our team is ready to help you with any inquiries.</p>
                    
                    <div class="space-y-6">
                        <div class="flex items-start">
                            <div class="w-12 h-12 rounded-full bg-purple-100 flex items-center justify-center text-purple-600 mr-4">
                                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path>
                                </svg>
                            </div>
                            <div>
                                <h3 class="font-semibold text-lg">Phone</h3>
                                <p class="text-gray-600">+971 4 123 4567</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="w-12 h-12 rounded-full bg-purple-100 flex items-center justify-center text-purple-600 mr-4">
                                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
                                </svg>
                            </div>
                            <div>
                                <h3 class="font-semibold text-lg">Email</h3>
                                <p class="text-gray-600">info@wasal.ae</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="w-12 h-12 rounded-full bg-purple-100 flex items-center justify-center text-purple-600 mr-4">
                                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"></path>
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path>
                                </svg>
                            </div>
                            <div>
                                <h3 class="font-semibold text-lg">Address</h3>
                                <p class="text-gray-600">Downtown Dubai<br>Dubai, United Arab Emirates</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="mt-8">
                        <h3 class="font-semibold text-lg mb-4">Follow Us</h3>
                        <div class="flex space-x-4">
                            <a href="#" class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white hover:bg-blue-700 transition duration-300">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M18.77,7.46H14.5v-1.9c0-.9.6-1.1,1-1.1h3V.5L14.84.5C10.41.5,9.4,3.3,9.4,5.3V7.46H6.21v4H9.4V22h5.1V11.46h3.77Z"></path>
                                </svg>
                            </a>
                            <a href="#" class="w-10 h-10 rounded-full bg-blue-400 flex items-center justify-center text-white hover:bg-blue-500 transition duration-300">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M22.46,6c-.77.35-1.6.58-2.46.69.88-.53,1.56-1.37,1.88-2.38-.83.5-1.75.85-2.72,1.05C18.37,4.5,17.26,4,16,4c-2.35,0-4.27,1.92-4.27,4.29,0,.34.04.67.11.98C8.28,9.09,5.11,7.38,3,4.79c-.37.63-.58,1.37-.58,2.15,0,1.49.75,2.81,1.91,3.56-.71,0-1.37-.2-1.95-.5v.03c0,2.08,1.48,3.82,3.44,4.21a4.22,4.22,0,0,1-1.93.07,4.28,4.28,0,0,0,4,2.98,8.521,8.521,0,0,1-5.33,1.84c-.34,0-.68-.02-1.02-.06C3.44,20.29,5.7,21,8.12,21,16,21,20.33,14.46,20.33,8.79c0-.19,0-.37-.01-.56.84-.6,1.56-1.36,2.14-2.23Z"></path>
                                </svg>
                            </a>
                            <a href="#" class="w-10 h-10 rounded-full bg-pink-600 flex items-center justify-center text-white hover:bg-pink-700 transition duration-300">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M12,2.2c3.2,0,3.6,0,4.9.1,3.3.1,4.8,1.7,4.9,4.9.1,1.3.1,1.6.1,4.8s0,3.6-.1,4.9c-.1,3.2-1.7,4.8-4.9,4.9-1.3.1-1.6.1-4.9.1s-3.6,0-4.9-.1c-3.3-.1-4.8-1.7-4.9-4.9-.1-1.3-.1-1.6-.1-4.9s0-3.6.1-4.8c.1-3.2,1.7-4.8,4.9-4.9,1.3-.1,1.6-.1,4.9-.1ZM12,0C8.7,0,8.3,0,7.1.1,2.7.3.3,2.7.1,7.1,0,8.3,0,8.7,0,12s0,3.7.1,4.9c.2,4.4,2.6,6.8,7,7,1.2.1,1.6.1,4.9.1s3.7,0,4.9-.1c4.4-.2,6.8-2.6,7-7,.1-1.2.1-1.6.1-4.9s0-3.7-.1-4.9c-.2-4.4-2.6-6.8-7-7C15.7,0,15.3,0,12,0Zm0,5.8A6.2,6.2,0,1,0,18.2,12,6.2,6.2,0,0,0,12,5.8Zm0,10.2A4,4,0,1,1,16,12,4,4,0,0,1,12,16ZM18.4,4.2A1.4,1.4,0,1,0,19.8,5.6,1.4,1.4,0,0,0,18.4,4.2Z"></path>
                                </svg>
                            </a>
                            <a href="#" class="w-10 h-10 rounded-full bg-blue-700 flex items-center justify-center text-white hover:bg-blue-800 transition duration-300">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M19,3H5C3.9,3,3,3.9,3,5v14c0,1.1,0.9,2,2,2h14c1.1,0,2-0.9,2-2V5C21,3.9,20.1,3,19,3z M9,17H6.5v-7H9V17z M7.7,8.7c-0.8,0-1.4-0.7-1.4-1.4c0-0.8,0.6-1.4,1.4-1.4c0.8,0,1.4,0.6,1.4,1.4C9.1,8.1,8.5,8.7,7.7,8.7z M18,17h-2.4v-3.8c0-1.5-0.5-1.7-1.2-1.7c-1.2,0-1.4,0.7-1.4,2v3.5h-2.5v-7h2.5v1c0.2-0.6,1-1.2,2-1.2c1.1,0,2.5,0.6,2.5,3.2V17z"></path>
                                </svg>
                            </a>
                        </div>
                    </div>
                </div>
                
                <div class="md:w-1/2">
                    <div class="bg-white rounded-xl shadow-lg p-8">
                        <h3 class="text-2xl font-bold mb-6">Send Us a Message</h3>
                        <form class="space-y-6">
                            <div>
                                <label class="block text-gray-700 mb-2" for="name">Full Name</label>
                                <input type="text" id="name" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-purple-600 focus:border-transparent" placeholder="Your name">
                            </div>
                            
                            <div>
                                <label class="block text-gray-700 mb-2" for="email">Email Address</label>
                                <input type="email" id="email" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-purple-600 focus:border-transparent" placeholder="Your email">
                            </div>
                            
                            <div>
                                <label class="block text-gray-700 mb-2" for="subject">Subject</label>
                                <input type="text" id="subject" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-purple-600 focus:border-transparent" placeholder="Subject">
                            </div>
                            
                            <div>
                                <label class="block text-gray-700 mb-2" for="message">Message</label>
                                <textarea id="message" rows="4" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-purple-600 focus:border-transparent" placeholder="Your message"></textarea>
                            </div>
                            
                            <button type="submit" class="w-full py-3 bg-gradient-to-r from-purple-600 to-blue-500 text-white font-semibold rounded-lg hover:from-purple-700 hover:to-blue-600 transition duration-300 shadow-md">Send Message</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-2xl font-bold mb-4 gradient-bg text-transparent bg-clip-text">Wasal</h3>
                    <p class="text-gray-400 mb-4">The UAE's Unified Delivery Platform bringing together all major delivery services under one app.</p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M18.77,7.46H14.5v-1.9c0-.9.6-1.1,1-1.1h3V.5L14.84.5C10.41.5,9.4,3.3,9.4,5.3V7.46H6.21v4H9.4V22h5.1V11.46h3.77Z"></path></svg>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M22.46,6c-.77.35-1.6.58-2.46.69.88-.53,1.56-1.37,1.88-2.38-.83.5-1.75.85-2.72,1.05C18.37,4.5,17.26,4,16,4c-2.35,0-4.27,1.92-4.27,4.29,0,.34.04.67.11.98C8.28,9.09,5.11,7.38,3,4.79c-.37.63-.58,1.37-.58,2.15,0,1.49.75,2.81,1.91,3.56-.71,0-1.37-.2-1.95-.5v.03c0,2.08,1.48,3.82,3.44,4.21a4.22,4.22,0,0,1-1.93.07,4.28,4.28,0,0,0,4,2.98,8.521,8.521,0,0,1-5.33,1.84c-.34,0-.68-.02-1.02-.06C3.44,20.29,5.7,21,8.12,21,16,21,20.33,14.46,20.33,8.79c0-.19,0-.37-.01-.56.84-.6,1.56-1.36,2.14-2.23Z"></path></svg>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M12,2.2c3.2,0,3.6,0,4.9.1,3.3.1,4.8,1.7,4.9,4.9.1,1.3.1,1.6.1,4.8s0,3.6-.1,4.9c-.1,3.2-1.7,4.8-4.9,4.9-1.3.1-1.6.1-4.9.1s-3.6,0-4.9-.1c-3.3-.1-4.8-1.7-4.9-4.9-.1-1.3-.1-1.6-.1-4.9s0-3.6.1-4.8c.1-3.2,1.7-4.8,4.9-4.9,1.3-.1,1.6-.1,4.9-.1ZM12,0C8.7,0,8.3,0,7.1.1,2.7.3.3,2.7.1,7.1,0,8.3,0,8.7,0,12s0,3.7.1,4.9c.2,4.4,2.6,6.8,7,7,1.2.1,1.6.1,4.9.1s3.7,0,4.9-.1c4.4-.2,6.8-2.6,7-7,.1-1.2.1-1.6.1-4.9s0-3.7-.1-4.9c-.2-4.4-2.6-6.8-7-7C15.7,0,15.3,0,12,0Zm0,5.8A6.2,6.2,0,1,0,18.2,12,6.2,6.2,0,0,0,12,5.8Zm0,10.2A4,4,0,1,1,16,12,4,4,0,0,1,12,16ZM18.4,4.2A1.4,1.4,0,1,0,19.8,5.6,1.4,1.4,0,0,0,18.4,4.2Z"></path></svg>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M19,3H5C3.9,3,3,3.9,3,5v14c0,1.1,0.9,2,2,2h14c1.1,0,2-0.9,2-2V5C21,3.9,20.1,3,19,3z M9,17H6.5v-7H9V17z M7.7,8.7c-0.8,0-1.4-0.7-1.4-1.4c0-0.8,0.6-1.4,1.4-1.4c0.8,0,1.4,0.6,1.4,1.4C9.1,8.1,8.5,8.7,7.7,8.7z M18,17h-2.4v-3.8c0-1.5-0.5-1.7-1.2-1.7c-1.2,0-1.4,0.7-1.4,2v3.5h-2.5v-7h2.5v1c0.2-0.6,1-1.2,2-1.2c1.1,0,2.5,0.6,2.5,3.2V17z"></path></svg>
                        </a>
                    </div>
                </div>
                
                <div>
                    <h4 class="text-lg font-semibold mb-4">Quick Links</h4>
                    <ul class="space-y-2">
                        <li><a href="#home" class="text-gray-400 hover:text-white transition duration-300">Home</a></li>
                        <li><a href="#personal" class="text-gray-400 hover:text-white transition duration-300">Personal</a></li>
                        <li><a href="#business" class="text-gray-400 hover:text-white transition duration-300">Business</a></li>
                        <li><a href="#contact" class="text-gray-400 hover:text-white transition duration-300">Contact</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-semibold mb-4">Services</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Personal Delivery</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Business Solutions</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Delivery Companies</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Driver Portal</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-semibold mb-4">Legal</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Cookie Policy</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">FAQ</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-8 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 text-sm mb```
<!-- ...existing code... -->
            <div class="border-t border-gray-800 mt-8 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 text-sm mb-4 md:mb-0">&copy; 2025 Wasal. All rights reserved.</p>
                <div class="flex space-x-4">
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">Terms</a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">Privacy</a>
                </div>
            </div>
        </div>
    </footer>
</body>
</html>
