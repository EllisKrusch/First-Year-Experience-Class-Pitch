<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lehigh First-Year Experience Survey</title>
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Load Inter font -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    
    <style>
        /* Custom styles */
        body {
            font-family: 'Inter', sans-serif;
            /* Using amber-900 as a proxy for Lehigh Brown, and amber-50 for a soft white */
            --lehigh-brown: #78350f;
            --lehigh-white: #fffbeb;
        }
        .slide {
            flex-shrink: 0;
            width: 100%;
            height: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 2rem 4rem;
            text-align: center;
            box-sizing: border-box; /* Ensures padding doesn't break layout */
        }
    </style>
</head>
<body class="bg-slate-100 flex items-center justify-center min-h-screen p-4">

    <!-- Slideshow Container -->
    <main class="relative w-full max-w-4xl aspect-[16/10] sm:aspect-[16/9] bg-white rounded-xl shadow-2xl overflow-hidden">
        
        <!-- Slides -->
        <div id="slides-container" class="flex h-full transition-transform duration-500 ease-in-out">
            
            <!-- Slide 1: Title -->
            <div class="slide bg-[var(--lehigh-brown)] text-white">
                <div class="w-full max-w-lg text-center">
                    
                    <h1 class="text-4xl md:text-5xl font-bold mb-4 mt-4">The Lehigh First-Year Experience</h1>
                    <p class="text-2xl md:text-3xl opacity-90">We want to hear from you!</p>
                    <footer class="mt-16 text-lg opacity-70">
                        A JOUR 025 Data Journalism Project
                    </footer>
                </div>
            </div>
            
            <!-- Slide 2: Why We're Here -->
            <div class="slide bg-[var(--lehigh-white)] text-[var(--lehigh-brown)]">
                <h2 class="text-3xl md:text-4xl font-bold mb-8">Why are we here?</h2>
                <ul class="space-y-6 text-xl md:text-2xl text-left max-w-lg">
                    <li class="flex items-start">
                        <span class="text-2xl mr-4 mt-1">📊</span>
                        <p>We're students in <strong>JOUR 025 (Data Journalism)</strong> conducting a survey for our class project.</p>
                    </li>
                    <li class="flex items-start">
                        <span class="text-2xl mr-4 mt-1">🎓</span>
                        <p>Our project is all about the <strong>Lehigh first-year experience</strong>.</p>
                    </li>
                </ul>
            </div>
            
            <!-- Slide 3: Our Goal -->
            <div class="slide bg-[var(--lehigh-brown)] text-white">
                <h2 class="text-3xl md:text-4xl font-bold mb-6">Our Goal</h2>
                <div class="max-w-2xl space-y-5 text-xl md:text-2xl opacity-95">
                    <p>To understand what factors impact your first-year experience and academic readiness.</p>
                    <p class="font-semibold">Specifically, we want to know how first-year students choose their academic focus and how effective Lehigh's programs are at supporting that choice.</p>
                </div>
            </div>

            <!-- Slide 4: Survey Details -->
            <div class="slide bg-[var(--lehigh-white)] text-[var(--lehigh-brown)]">
                <h2 class="text-3xl md:text-4xl font-bold mb-10">About the Survey</h2>
                <div class="flex flex-col sm:flex-row gap-8 max-w-3xl w-full justify-around">
                    <!-- Detail 1: Time -->
                    <div class="flex flex-col items-center p-4">
                        <svg class="w-16 h-16 mb-3" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M12 6v6h4.5m4.5 0a9 9 0 11-18 0 9 9 0 0118 0z" />
                        </svg>
                        <span class="text-xl md:text-2xl font-semibold">Takes ~5 Minutes</span>
                    </div>
                    <!-- Detail 2: Anonymous -->
                    <div class="flex flex-col items-center p-4">
                        <svg class="w-16 h-16 mb-3" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M16.5 10.5V6.75a4.5 4.5 0 10-9 0v3.75m-.75 11.25h10.5a2.25 2.25 0 002.25-2.25v-6.75a2.25 2.25 0 00-2.25-2.25H6.75a2.25 2.25 0 00-2.25 2.25v6.75a2.25 2.25 0 002.25 2.25z" />
                        </svg>
                        <span class="text-xl md:text-2xl font-semibold">Completely Anonymous</span>
                    </div>
                </div>
                <p class="mt-8 text-xl md:text-2xl font-semibold">Your participation is invaluable to our project!</p>
            </div>
            
            <!-- Slide 5: Call to Action (Link/QR) -->
            <div class="slide bg-[var(--lehigh-brown)] text-white">
                <h2 class="text-3xl md:text-4xl font-bold mb-6">How to Participate</h2>
                <div class="flex flex-col md:flex-row items-center gap-8 md:gap-12">
                    <!-- QR Code Placeholder -->
                    <div class="text-center">
                        <img src="https://placehold.co/250x250/fffbeb/78350f?text=Scan+Me%21%0A(Survey+QR)" 
                             alt="QR Code for survey" 
                             class="rounded-lg w-48 h-48 sm:w-64 sm:h-64 object-cover"
                             onerror="this.src='https://placehold.co/250x250/fffbeb/78350f?text=QR+Code+Here'">
                        <p class="mt-2 text-lg font-semibold">Scan the QR Code</p>
                    </div>
                    
                    <!-- Link -->
                    <div class="text-center md:text-left">
                        <p class="text-xl mb-3">Or use the link:</p>
                        <a href="https://lehigh.co1.qualtrics.com/jfe/form/SV_8eHZfSYyU6inClM" 
                           target="_blank" 
                           class="text-lg sm:text-xl font-medium text-white bg-white/20 px-4 py-2 rounded-lg hover:bg-white/30 transition-all break-all">
                           lehigh.co1.qualtrics.com/...
                        </a>
                    </div>
                </div>
            </div>

            <!-- Slide 6: Thank You / Questions -->
            <div class="slide bg-[var(--lehigh-white)] text-[var(--lehigh-brown)]">
                <h2 class="text-4xl md:text-5xl font-bold mb-8">Thank You!</h2>
                <p class="text-xl md:text-2xl mb-12 max-w-lg">Thank you so much for your time and consideration.</p>
                <div class="border-t-2 border-[var(--lehigh-brown)]/30 pt-8">
                    <p class="text-lg md:text-xl">Questions?</p>
                    <p class="text-lg md:text-xl font-semibold">Contact Professor Haiyan Jia</p>
                    <p class="text-lg md:text-xl">haiyan.jia@lehigh.edu</p>
                </div>
            </div>

        </div>
        
        <!-- Navigation Buttons -->
        <button id="prev" class="absolute left-4 top-1/2 -translate-y-1/2 bg-black/30 text-white p-2 rounded-full hover:bg-black/50 transition-all disabled:opacity-0 disabled:cursor-not-allowed z-10">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5L8.25 12l7.5-7.5" />
            </svg>
        </button>
        
        <button id="next" class="absolute right-4 top-1/2 -translate-y-1/2 bg-black/30 text-white p-2 rounded-full hover:bg-black/50 transition-all disabled:opacity-0 disabled:cursor-not-allowed z-10">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
            </svg>
        </button>

    </main>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const slidesContainer = document.getElementById('slides-container');
            const slides = document.querySelectorAll('.slide');
            const prevBtn = document.getElementById('prev');
            const nextBtn = document.getElementById('next');
            
            let currentSlide = 0;
            const totalSlides = slides.length;

            function updateSlides() {
                // Move the slide container
                slidesContainer.style.transform = `translateX(-${currentSlide * 100}%)`;
                
                // Update button states
                prevBtn.disabled = currentSlide === 0;
                nextBtn.disabled = currentSlide === totalSlides - 1;
            }

            // Next button click
            nextBtn.addEventListener('click', () => {
                if (currentSlide < totalSlides - 1) {
                    currentSlide++;
                    updateSlides();
                }
            });

            // Previous button click
            prevBtn.addEventListener('click', () => {
                if (currentSlide > 0) {
                    currentSlide--;
                    updateSlides();
                }
            });

            // Allow keyboard navigation
            document.addEventListener('keydown', (e) => {
                if (e.key === 'ArrowRight') {
                    nextBtn.click();
                } else if (e.key === 'ArrowLeft') {
                    prevBtn.click();
                }
            });

            // Initial setup
            updateSlides();
        });
    </script>
</body>
</html>
