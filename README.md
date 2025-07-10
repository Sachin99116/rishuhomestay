<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rishu Homestay - Serene Stay in Chakrata, Uttarakhand</title>
    <meta name="description" content="Experience peaceful mountain living at Rishu Homestay in Chakrata. Comfortable rooms, delicious food, and breathtaking views of the Himalayas.">
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Custom CSS for enhancements */
        .hero {
            background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://images.unsplash.com/photo-1566073771259-6a8506099945?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80');
            background-size: cover;
            background-position: center;
        }
        
        .room-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .gallery-item {
            transition: all 0.3s ease;
        }
        
        .gallery-item:hover {
            transform: scale(1.03);
        }
        
        .active-tab {
            border-bottom: 3px solid #f59e0b;
            color: #f59e0b;
        }
        
        /* Animation for booking form */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .animate-fade-in {
            animation: fadeIn 0.5s ease-out forwards;
        }
    </style>
</head>
<body class="font-sans bg-amber-50">
    <!-- Navigation -->
    <nav class="bg-white shadow-md sticky top-0 z-50">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center">
                <i class="fas fa-mountain text-amber-600 text-2xl mr-2"></i>
                <a href="#" class="text-xl font-bold text-gray-800">Rishu Homestay</a>
            </div>
            
            <div class="hidden md:flex space-x-6">
                <a href="#home" class="text-gray-700 hover:text-amber-600 transition">Home</a>
                <a href="#about" class="text-gray-700 hover:text-amber-600 transition">About</a>
                <a href="#rooms" class="text-gray-700 hover:text-amber-600 transition">Rooms</a>
                <a href="#gallery" class="text-gray-700 hover:text-amber-600 transition">Gallery</a>
                <a href="#reviews" class="text-gray-700 hover:text-amber-600 transition">Reviews</a>
                <a href="#contact" class="text-gray-700 hover:text-amber-600 transition">Contact</a>
            </div>
            
            <button id="mobile-menu-button" class="md:hidden text-gray-700">
                <i class="fas fa-bars text-xl"></i>
            </button>
        </div>
        
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white py-2 px-4 shadow-lg">
            <a href="#home" class="block py-2 text-gray-700 hover:text-amber-600">Home</a>
            <a href="#about" class="block py-2 text-gray-700 hover:text-amber-600">About</a>
            <a href="#rooms" class="block py-2 text-gray-700 hover:text-amber-600">Rooms</a>
            <a href="#gallery" class="block py-2 text-gray-700 hover:text-amber-600">Gallery</a>
            <a href="#reviews" class="block py-2 text-gray-700 hover:text-amber-600">Reviews</a>
            <a href="#contact" class="block py-2 text-gray-700 hover:text-amber-600">Contact</a>
            <a href="#booking" class="block py-2 bg-amber-500 text-white rounded text-center mt-2 hover:bg-amber-600">Book Now</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero min-h-screen flex items-center justify-center text-center text-white">
        <div class="container mx-auto px-4">
            <h1 class="text-4xl md:text-6xl font-bold mb-6">Welcome to Rishu Homestay</h1>
            <p class="text-xl md:text-2xl mb-8">Experience the serenity of Chakrata in the heart of Uttarakhand</p>
            <a href="#booking" class="bg-amber-500 hover:bg-amber-600 text-white font-bold py-3 px-8 rounded-full text-lg transition duration-300 inline-block">Book Your Stay</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">About Our Homestay</h2>
            
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
                    <img src="https://images.unsplash.com/photo-1600585154340-be6161a56a0c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="Rishu Homestay" class="rounded-lg shadow-xl w-full h-auto">
                </div>
                
                <div class="md:w-1/2">
                    <h3 class="text-2xl font-semibold mb-4 text-amber-600">Your Home in the Himalayas</h3>
                    <p class="text-gray-700 mb-4">Nestled in the pristine hills of Chakrata, Rishu Homestay offers a perfect blend of comfort and nature's beauty. Our family-run establishment provides a warm, personalized experience that hotels simply can't match.</p>
                    <p class="text-gray-700 mb-4">Located on Tiger Fall Road, we're surrounded by lush forests and offer breathtaking views of the Himalayan ranges. Wake up to the sound of birds and enjoy fresh mountain air every morning.</p>
                    <p class="text-gray-700 mb-6">We take pride in serving homemade meals prepared with locally sourced ingredients, giving you a true taste of Uttarakhand's culinary heritage.</p>
                    
                    <div class="grid grid-cols-2 gap-4">
                        <div class="flex items-center">
                            <i class="fas fa-mountain text-amber-500 mr-2"></i>
                            <span>Mountain Views</span>
                        </div>
                        <div class="flex items-center">
                            <i class="fas fa-utensils text-amber-500 mr-2"></i>
                            <span>Home-cooked Meals</span>
                        </div>
                        <div class="flex items-center">
                            <i class="fas fa-wifi text-amber-500 mr-2"></i>
                            <span>Free WiFi</span>
                        </div>
                        <div class="flex items-center">
                            <i class="fas fa-parking text-amber-500 mr-2"></i>
                            <span>Parking Available</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Rooms Section -->
    <section id="rooms" class="py-16 bg-amber-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Our Rooms</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Room 1 -->
                <div class="room-card bg-white rounded-lg overflow-hidden shadow-md transition duration-300">
                    <img src="https://images.unsplash.com/photo-1631049307264-da0ec9d70304?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="Deluxe Room" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2 text-gray-800">Deluxe Room</h3>
                        <p class="text-gray-600 mb-4">Spacious room with mountain view, attached bathroom, and comfortable queen-size bed.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-amber-600 font-bold text-lg">₹2,500/night</span>
                            <button class="book-btn bg-amber-500 hover:bg-amber-600 text-white py-2 px-4 rounded transition" data-room="Deluxe Room">Book Now</button>
                        </div>
                    </div>
                </div>
                
                <!-- Room 2 -->
                <div class="room-card bg-white rounded-lg overflow-hidden shadow-md transition duration-300">
                    <img src="https://images.unsplash.com/photo-1582719478250-c89cae4dc85b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="Family Suite" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2 text-gray-800">Family Suite</h3>
                        <p class="text-gray-600 mb-4">Perfect for families with one double bed and two single beds, private balcony.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-amber-600 font-bold text-lg">₹3,500/night</span>
                            <button class="book-btn bg-amber-500 hover:bg-amber-600 text-white py-2 px-4 rounded transition" data-room="Family Suite">Book Now</button>
                        </div>
                    </div>
                </div>
                
                <!-- Room 3 -->
                <div class="room-card bg-white rounded-lg overflow-hidden shadow-md transition duration-300">
                    <img src="https://images.unsplash.com/photo-1566669437685-f6c10b1d6604?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1974&q=80" alt="Premium Cottage" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2 text-gray-800">Premium Cottage</h3>
                        <p class="text-gray-600 mb-4">Private cottage with fireplace, king-size bed, and panoramic mountain views.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-amber-600 font-bold text-lg">₹4,500/night</span>
                            <button class="book-btn bg-amber-500 hover:bg-amber-600 text-white py-2 px-4 rounded transition" data-room="Premium Cottage">Book Now</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Amenities Section -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Our Amenities</h2>
            
            <div class="grid grid-cols-2 md:grid-cols-4 gap-6">
                <div class="text-center p-4">
                    <div class="bg-amber-100 w-16 h-16 mx-auto rounded-full flex items-center justify-center mb-3">
                        <i class="fas fa-utensils text-amber-600 text-2xl"></i>
                    </div>
                    <h3 class="font-semibold">Home-cooked Meals</h3>
                </div>
                
                <div class="text-center p-4">
                    <div class="bg-amber-100 w-16 h-16 mx-auto rounded-full flex items-center justify-center mb-3">
                        <i class="fas fa-wifi text-amber-600 text-2xl"></i>
                    </div>
                    <h3 class="font-semibold">Free WiFi</h3>
                </div>
                
                <div class="text-center p-4">
                    <div class="bg-amber-100 w-16 h-16 mx-auto rounded-full flex items-center justify-center mb-3">
                        <i class="fas fa-parking text-amber-600 text-2xl"></i>
                    </div>
                    <h3 class="font-semibold">Parking</h3>
                </div>
                
                <div class="text-center p-4">
                    <div class="bg-amber-100 w-16 h-16 mx-auto rounded-full flex items-center justify-center mb-3">
                        <i class="fas fa-snowflake text-amber-600 text-2xl"></i>
                    </div>
                    <h3 class="font-semibold">Heating</h3>
                </div>
                
                <div class="text-center p-4">
                    <div class="bg-amber-100 w-16 h-16 mx-auto rounded-full flex items-center justify-center mb-3">
                        <i class="fas fa-tv text-amber-600 text-2xl"></i>
                    </div>
                    <h3 class="font-semibold">TV</h3>
                </div>
                
                <div class="text-center p-4">
                    <div class="bg-amber-100 w-16 h-16 mx-auto rounded-full flex items-center justify-center mb-3">
                        <i class="fas fa-mug-hot text-amber-600 text-2xl"></i>
                    </div>
                    <h3 class="font-semibold">Tea/Coffee</h3>
                </div>
                
                <div class="text-center p-4">
                    <div class="bg-amber-100 w-16 h-16 mx-auto rounded-full flex items-center justify-center mb-3">
                        <i class="fas fa-hiking text-amber-600 text-2xl"></i>
                    </div>
                    <h3 class="font-semibold">Trekking Guides</h3>
                </div>
                
                <div class="text-center p-4">
                    <div class="bg-amber-100 w-16 h-16 mx-auto rounded-full flex items-center justify-center mb-3">
                        <i class="fas fa-first-aid text-amber-600 text-2xl"></i>
                    </div>
                    <h3 class="font-semibold">First Aid</h3>
                </div>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section id="gallery" class="py-16 bg-amber-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Photo Gallery</h2>
            
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
                <div class="gallery-item overflow-hidden rounded-lg shadow-md">
                    <img src="https://images.unsplash.com/photo-1564501049412-61c2a3083791?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1932&q=80" alt="Homestay View" class="w-full h-48 object-cover hover:scale-105 transition duration-300">
                </div>
                <div class="gallery-item overflow-hidden rounded-lg shadow-md">
                    <img src="https://images.unsplash.com/photo-1600566752227-17c6c0e62b2b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="Dining Area" class="w-full h-48 object-cover hover:scale-105 transition duration-300">
                </div>
                <div class="gallery-item overflow-hidden rounded-lg shadow-md">
                    <img src="https://images.unsplash.com/photo-1556911220-bff31c812dba?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1986&q=80" alt="Living Room" class="w-full h-48 object-cover hover:scale-105 transition duration-300">
                </div>
                <div class="gallery-item overflow-hidden rounded-lg shadow-md">
                    <img src="https://images.unsplash.com/photo-1584132967334-10e028bd69f7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="Kitchen" class="w-full h-48 object-cover hover:scale-105 transition duration-300">
                </div>
                <div class="gallery-item overflow-hidden rounded-lg shadow-md">
                    <img src="https://images.unsplash.com/photo-1582719478250-c89cae4dc85b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="Bedroom" class="w-full h-48 object-cover hover:scale-105 transition duration-300">
                </div>
                <div class="gallery-item overflow-hidden rounded-lg shadow-md">
                    <img src="https://images.unsplash.com/photo-1520250497591-112f2f40a3f4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="Bathroom" class="w-full h-48 object-cover hover:scale-105 transition duration-300">
                </div>
                <div class="gallery-item overflow-hidden rounded-lg shadow-md">
                    <img src="https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="Garden" class="w-full h-48 object-cover hover:scale-105 transition duration-300">
                </div>
                <div class="gallery-item overflow-hidden rounded-lg shadow-md">
                    <img src="https://images.unsplash.com/photo-1513519245088-0e12902e5a38?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="Mountain View" class="w-full h-48 object-cover hover:scale-105 transition duration-300">
                </div>
            </div>
        </div>
    </section>

    <!-- Reviews Section -->
    <section id="reviews" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Guest Reviews</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Review 1 -->
                <div class="bg-amber-50 p-6 rounded-lg shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/32.jpg" alt="Guest" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Priya Sharma</h4>
                            <div class="flex text-amber-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-700">"Absolutely loved our stay at Rishu Homestay! The hosts were incredibly warm and welcoming. The food was delicious and the room was cozy with a beautiful mountain view. Will definitely come back!"</p>
                </div>
                
                <!-- Review 2 -->
                <div class="bg-amber-50 p-6 rounded-lg shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/men/45.jpg" alt="Guest" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Rahul Verma</h4>
                            <div class="flex text-amber-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star-half-alt"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-700">"Perfect getaway from city life. The homestay is well-maintained and the location is peaceful. The hosts helped us plan our local sightseeing which was very helpful. Highly recommended!"</p>
                </div>
                
                <!-- Review 3 -->
                <div class="bg-amber-50 p-6 rounded-lg shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Guest" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Neha Patel</h4>
                            <div class="flex text-amber-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-700">"We stayed for 3 nights and wished we could stay longer! The family made us feel at home, the kids loved playing in the garden, and the homemade breakfast was amazing. Truly a memorable experience."</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Booking Section -->
    <section id="booking" class="py-16 bg-amber-600 text-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Book Your Stay</h2>
            
            <div class="max-w-3xl mx-auto bg-white rounded-lg shadow-xl overflow-hidden animate-fade-in">
                <div class="md:flex">
                    <div class="md:w-1/2 bg-amber-700 p-8">
                        <h3 class="text-2xl font-bold mb-4">Reservation Details</h3>
                        <p class="mb-6">Fill out the form to check availability and book your perfect mountain getaway.</p>
                        
                        <div class="mb-6">
                            <h4 class="font-bold mb-2">Why Book With Us?</h4>
                            <ul class="space-y-2">
                                <li class="flex items-start">
                                    <i class="fas fa-check-circle mt-1 mr-2"></i>
                                    <span>Best price guarantee</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check-circle mt-1 mr-2"></i>
                                    <span>No booking fees</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check-circle mt-1 mr-2"></i>
                                    <span>Instant confirmation</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check-circle mt-1 mr-2"></i>
                                    <span>Flexible cancellation</span>
                                </li>
                            </ul>
                        </div>
                        
                        <div>
                            <h4 class="font-bold mb-2">Need Help?</h4>
                            <p>Call us at <a href="tel:+918630395282" class="underline">+91 8630395282</a> or email <a href="mailto:info@rishuhomestay.com" class="underline">info@rishuhomestay.com</a></p>
                        </div>
                    </div>
                    
                    <div class="md:w-1/2 p-8 text-gray-800">
                        <form id="booking-form" class="space-y-4">
                            <div>
                                <label for="room-type" class="block font-medium mb-1">Room Type</label>
                                <select id="room-type" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500" required>
                                    <option value="" disabled selected>Select Room</option>
                                    <option value="Deluxe Room">Deluxe Room - ₹2,500/night</option>
                                    <option value="Family Suite">Family Suite - ₹3,500/night</option>
                                    <option value="Premium Cottage">Premium Cottage - ₹4,500/night</option>
                                </select>
                            </div>
                            
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                <div>
                                    <label for="check-in" class="block font-medium mb-1">Check-in</label>
                                    <input type="date" id="check-in" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500" required>
                                </div>
                                <div>
                                    <label for="check-out" class="block font-medium mb-1">Check-out</label>
                                    <input type="date" id="check-out" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500" required>
                                </div>
                            </div>
                            
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                <div>
                                    <label for="adults" class="block font-medium mb-1">Adults</label>
                                    <select id="adults" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500" required>
                                        <option value="1">1</option>
                                        <option value="2" selected>2</option>
                                        <option value="3">3</option>
                                        <option value="4">4</option>
                                    </select>
                                </div>
                                <div>
                                    <label for="children" class="block font-medium mb-1">Children</label>
                                    <select id="children" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500">
                                        <option value="0" selected>0</option>
                                        <option value="1">1</option>
                                        <option value="2">2</option>
                                        <option value="3">3</option>
                                    </select>
                                </div>
                            </div>
                            
                            <div>
                                <label for="name" class="block font-medium mb-1">Full Name</label>
                                <input type="text" id="name" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500" required>
                            </div>
                            
                            <div>
                                <label for="email" class="block font-medium mb-1">Email</label>
                                <input type="email" id="email" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500" required>
                            </div>
                            
                            <div>
                                <label for="phone" class="block font-medium mb-1">Phone</label>
                                <input type="tel" id="phone" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500" required>
                            </div>
                            
                            <div>
                                <label for="special-requests" class="block font-medium mb-1">Special Requests</label>
                                <textarea id="special-requests" rows="3" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500"></textarea>
                            </div>
                            
                            <button type="submit" class="w-full bg-amber-600 hover:bg-amber-700 text-white font-bold py-3 px-4 rounded transition duration-300">Complete Booking</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Contact Us</h2>
            
            <div class="flex flex-col md:flex-row gap-8">
                <div class="md:w-1/2">
                    <div class="bg-amber-50 p-6 rounded-lg shadow-md h-full">
                        <h3 class="text-xl font-bold mb-4 text-amber-600">Get in Touch</h3>
                        
                        <div class="space-y-4">
                            <div class="flex items-start">
                                <i class="fas fa-map-marker-alt text-amber-600 mt-1 mr-3"></i>
                                <div>
                                    <h4 class="font-semibold">Address</h4>
                                    <p>Chakrata, Tiger Fall Road, Uttarakhand</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <i class="fas fa-phone-alt text-amber-600 mt-1 mr-3"></i>
                                <div>
                                    <h4 class="font-semibold">Phone</h4>
                                    <p><a href="tel:+918630395282" class="hover:text-amber-600">+91 8630395282</a></p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <i class="fas fa-envelope text-amber-600 mt-1 mr-3"></i>
                                <div>
                                    <h4 class="font-semibold">Email</h4>
                                    <p><a href="mailto:info@rishuhomestay.com" class="hover:text-amber-600">info@rishuhomestay.com</a></p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <i class="fas fa-clock text-amber-600 mt-1 mr-3"></i>
                                <div>
                                    <h4 class="font-semibold">Check-in/Check-out</h4>
                                    <p>Check-in: 12:00 PM | Check-out: 10:00 AM</p>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-8">
                            <h4 class="font-semibold mb-3">Follow Us</h4>
                            <div class="flex space-x-4">
                                <a href="#" class="w-10 h-10 rounded-full bg-amber-600 text-white flex items-center justify-center hover:bg-amber-700 transition">
                                    <i class="fab fa-facebook-f"></i>
                                </a>
                                <a href="#" class="w-10 h-10 rounded-full bg-amber-600 text-white flex items-center justify-center hover:bg-amber-700 transition">
                                    <i class="fab fa-instagram"></i>
                                </a>
                                <a href="#" class="w-10 h-10 rounded-full bg-amber-600 text-white flex items-center justify-center hover:bg-amber-700 transition">
                                    <i class="fab fa-twitter"></i>
                                </a>
                                <a href="#" class="w-10 h-10 rounded-full bg-amber-600 text-white flex items-center justify-center hover:bg-amber-700 transition">
                                    <i class="fab fa-tripadvisor"></i>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="md:w-1/2">
                    <div class="h-full rounded-lg overflow-hidden shadow-md">
                        <!-- Map placeholder - in a real implementation you would use Google Maps or similar -->
                        <div class="bg-gray-200 h-full flex items-center justify-center">
                            <div class="text-center p-6">
                                <i class="fas fa-map-marked-alt text-4xl text-amber-600 mb-4"></i>
                                <h3 class="text-xl font-bold mb-2">Our Location</h3>
                                <p class="mb-4">Chakrata, Tiger Fall Road, Uttarakhand</p>
                                <a href="https://maps.google.com/?q=Rishu+Homestay,Chakrata+Tiger+Fall+Road,Uttrakhand" target="_blank" class="inline-block bg-amber-600 hover:bg-amber-700 text-white py-2 px-4 rounded transition">View on Google Maps</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="mt-12 bg-amber-50 p-6 rounded-lg shadow-md">
                <h3 class="text-xl font-bold mb-4 text-amber-600">Send Us a Message</h3>
                <form class="space-y-4">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div>
                            <label for="contact-name" class="block font-medium mb-1">Name</label>
                            <input type="text" id="contact-name" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500" required>
                        </div>
                        <div>
                            <label for="contact-email" class="block font-medium mb-1">Email</label>
                            <input type="email" id="contact-email" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500" required>
                        </div>
                    </div>
                    
                    <div>
                        <label for="contact-subject" class="block font-medium mb-1">Subject</label>
                        <input type="text" id="contact-subject" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500" required>
                    </div>
                    
                    <div>
                        <label for="contact-message" class="block font-medium mb-1">Message</label>
                        <textarea id="contact-message" rows="4" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-amber-500" required></textarea>
                    </div>
                    
                    <button type="submit" class="bg-amber-600 hover:bg-amber-700 text-white font-bold py-2 px-6 rounded transition">Send Message</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">Rishu Homestay</h3>
                    <p class="mb-4">Experience the serenity of the Himalayas with our warm hospitality and comfortable accommodations.</p>
                    <div class="flex space-x-4">
                        <a href="#" class="hover:text-amber-400"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="hover:text-amber-400"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="hover:text-amber-400"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="hover:text-amber-400"><i class="fab fa-tripadvisor"></i></a>
                    </div>
                </div>
                
                <div>
                    <h4 class="font-bold mb-4">Quick Links</h4>
                    <ul class="space-y-2">
                        <li><a href="#home" class="hover:text-amber-400 transition">Home</a></li>
                        <li><a href="#about" class="hover:text-amber-400 transition">About Us</a></li>
                        <li><a href="#rooms" class="hover:text-amber-400 transition">Rooms</a></li>
                        <li><a href="#gallery" class="hover:text-amber-400 transition">Gallery</a></li>
                        <li><a href="#contact" class="hover:text-amber-400 transition">Contact</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-bold mb-4">Contact Info</h4>
                    <ul class="space-y-2">
                        <li class="flex items-start">
                            <i class="fas fa-map-marker-alt mt-1 mr-2 text-amber-400"></i>
                            <span>Chakrata, Tiger Fall Road, Uttarakhand</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-phone-alt mt-1 mr-2 text-amber-400"></i>
                            <span>+91 8630395282</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-envelope mt-1 mr-2 text-amber-400"></i>
                            <span>info@rishuhomestay.com</span>
                        </li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-bold mb-4">Newsletter</h4>
                    <p class="mb-4">Subscribe to our newsletter for special offers and updates.</p>
                    <form class="flex">
                        <input type="email" placeholder="Your email" class="px-4 py-2 w-full rounded-l focus:outline-none text-gray-800">
                        <button type="submit" class="bg-amber-600 hover:bg-amber-700 px-4 py-2 rounded-r transition">
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </form>
                </div>
            </div>
            
            <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-400">
                <p>&copy; 2023 Rishu Homestay. All rights reserved.</p>
                <p class="mt-2">Designed with <i class="fas fa-heart text-amber-400"></i> for travelers</p>
            </div>
        </div>
    </footer>

    <!-- Back to top button -->
    <button id="back-to-top" class="fixed bottom-6 right-6 bg-amber-600 text-white w-12 h-12 rounded-full shadow-lg flex items-center justify-center hidden">
        <i class="fas fa-arrow-up"></i>
    </button>

    <!-- Booking confirmation modal -->
    <div id="booking-modal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50 hidden">
        <div class="bg-white rounded-lg p-8 max-w-md w-full mx-4 animate-fade-in">
            <div class="text-center">
                <i class="fas fa-check-circle text-5xl text-green-500 mb-4"></i>
                <h3 class="text-2xl font-bold mb-2">Booking Confirmed!</h3>
                <p class="mb-6">Thank you for choosing Rishu Homestay. We've sent the details to your email.</p>
                <button id="close-modal" class="bg-amber-600 hover:bg-amber-700 text-white font-bold py-2 px-6 rounded transition">Close</button>
            </div>
        </div>
    </div>

    <script>
        // Mobile menu toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    // Close mobile menu if open
                    document.getElementById('mobile-menu').classList.add('hidden');
                    
                    // Scroll to target
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Back to top button
        const backToTopButton = document.getElementById('back-to-top');
        window.addEventListener('scroll', function() {
            if (window.pageYOffset > 300) {
                backToTopButton.classList.remove('hidden');
            } else {
                backToTopButton.classList.add('hidden');
            }
        });
        
        backToTopButton.addEventListener('click', function() {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });

        // Room booking buttons
        document.querySelectorAll('.book-btn').forEach(button => {
            button.addEventListener('click', function() {
                const roomType = this.getAttribute('data-room');
                document.getElementById('room-type').value = roomType;
                
                // Scroll to booking form
                document.getElementById('booking').scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Booking form submission
        document.getElementById('booking-form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // In a real implementation, you would send this data to your server
            // For this demo, we'll just show a confirmation modal
            document.getElementById('booking-modal').classList.remove('hidden');
            
            // Reset form
            this.reset();
        });

        // Close modal
        document.getElementById('close-modal').addEventListener('click', function() {
            document.getElementById('booking-modal').classList.add('hidden');
        });

        // Set minimum dates for booking
        const today = new Date().toISOString().split('T')[0];
        document.getElementById('check-in').min = today;
        document.getElementById('check-out').min = today;

        // Update check-out min date when check-in changes
        document.getElementById('check-in').addEventListener('change', function() {
            document.getElementById('check-out').min = this.value;
        });

        // Active navigation link highlighting
        const sections = document.querySelectorAll('section');
        const navLinks = document.querySelectorAll('nav a');

        window.addEventListener('scroll', function() {
            let current = '';
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                
                if (pageYOffset >= (sectionTop - 100)) {
                    current = section.getAttribute('id');
                }
            });
            
            navLinks.forEach(link => {
                link.classList.remove('active-tab');
                if (link.getAttribute('href') === `#${current}`) {
                    link.classList.add('active-tab');
                }
            });
        });
    </script>
</body>
</html>
