[c_ng_th_ng_tin_hello_ecosystem (2).html](https://github.com/user-attachments/files/28941875/c_ng_th_ng_tin_hello_ecosystem.2.html)# hello-ecosystem
test
[Uploading <!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hello Ecosystem</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Custom animations */
        .fade-in { animation: fadeIn 0.8s ease-in-out; }
        .slide-up { animation: slideUp 0.6s ease-out forwards; opacity: 0; }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes slideUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Staggered animation delays for cards */
        .delay-100 { animation-delay: 100ms; }
        .delay-200 { animation-delay: 200ms; }
        .delay-300 { animation-delay: 300ms; }
        .delay-400 { animation-delay: 400ms; }
        .delay-500 { animation-delay: 500ms; }

        /* Toast notification */
        #toast {
            visibility: hidden;
            min-width: 250px;
            background-color: #333;
            color: #fff;
            text-align: center;
            border-radius: 8px;
            padding: 16px;
            position: fixed;
            z-index: 50;
            left: 50%;
            bottom: 30px;
            transform: translateX(-50%);
            opacity: 0;
            transition: opacity 0.3s, bottom 0.3s, visibility 0.3s;
        }
        #toast.show {
            visibility: visible;
            opacity: 1;
            bottom: 50px;
        }
    </style>
</head>
<body class="bg-gray-50 font-sans text-gray-800 antialiased overflow-x-hidden">

    <!-- Navigation -->
    <nav class="bg-white shadow-sm fixed w-full z-40 top-0">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16 items-center">
                <div class="flex-shrink-0 flex items-center cursor-pointer" onclick="window.scrollTo(0,0)">
                    <span class="text-2xl font-extrabold text-blue-600 tracking-tight">Hello<span class="text-gray-800">Eco</span></span>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#services" class="text-gray-600 hover:text-blue-600 px-3 py-2 rounded-md text-sm font-medium transition-colors">Dịch vụ</a>
                    <a href="#about" class="text-gray-600 hover:text-blue-600 px-3 py-2 rounded-md text-sm font-medium transition-colors">Về chúng tôi</a>
                    <a href="#contact" class="text-gray-600 hover:text-blue-600 px-3 py-2 rounded-md text-sm font-medium transition-colors">Liên hệ</a>
                </div>
                <div class="flex items-center space-x-4">
                    <button class="text-gray-600 hover:text-blue-600 font-medium text-sm hidden sm:block transition-colors">Đăng nhập</button>
                    <button class="bg-blue-600 hover:bg-blue-700 text-white px-4 py-2 rounded-full text-sm font-medium transition-all shadow-md hover:shadow-lg">Đăng ký</button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <div class="relative bg-gradient-to-br from-blue-50 to-indigo-100 pt-32 pb-20 lg:pt-40 lg:pb-28 fade-in">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h1 class="text-4xl tracking-tight font-extrabold text-gray-900 sm:text-5xl md:text-6xl">
                <span class="block">Khám phá hệ sinh thái</span>
                <span class="block text-blue-600 mt-2">Dành riêng cho bạn</span>
            </h1>
            <p class="mt-4 max-w-md mx-auto text-base text-gray-600 sm:text-lg md:mt-8 md:text-xl md:max-w-3xl">
                Từ việc tìm kiếm cơ hội nghề nghiệp, đặt món ăn ngon, chăm sóc thú cưng cho đến mua sắm và giải trí. Tất cả đều có tại Hello Ecosystem.
            </p>
            <div class="mt-10 flex justify-center gap-4">
                <a href="#services" class="bg-blue-600 hover:bg-blue-700 text-white px-8 py-3 border border-transparent text-base font-medium rounded-full shadow-lg hover:shadow-xl transition-all">
                    Khám phá ngay
                </a>
            </div>
        </div>
    </div>

    <!-- Services Section -->
    <div id="services" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-base text-blue-600 font-semibold tracking-wide uppercase">Dịch vụ của chúng tôi</h2>
                <p class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">
                    Mọi thứ bạn cần ở một nơi
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <!-- HelloJob -->
                <div class="bg-white rounded-2xl shadow-sm border border-gray-100 p-8 hover:shadow-xl hover:-translate-y-1 transition-all duration-300 cursor-pointer slide-up delay-100" onclick="showToast('HelloJob đang được phát triển. Cùng đón chờ nhé!')">
                    <div class="w-14 h-14 bg-blue-100 rounded-xl flex items-center justify-center mb-6 text-blue-600">
                        <i class="fa-solid fa-briefcase text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-3">HelloJob</h3>
                    <p class="text-gray-600">Nền tảng tìm kiếm việc làm thông minh, kết nối ứng viên với hàng ngàn doanh nghiệp hàng đầu.</p>
                </div>

                <!-- HelloFood -->
                <div class="bg-white rounded-2xl shadow-sm border border-gray-100 p-8 hover:shadow-xl hover:-translate-y-1 transition-all duration-300 cursor-pointer slide-up delay-200" onclick="showToast('HelloFood đang được phát triển. Cùng đón chờ nhé!')">
                    <div class="w-14 h-14 bg-orange-100 rounded-xl flex items-center justify-center mb-6 text-orange-600">
                        <i class="fa-solid fa-burger text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-3">HelloFood</h3>
                    <p class="text-gray-600">Giao đồ ăn tận nơi nhanh chóng với hàng ngàn lựa chọn nhà hàng và món ăn đa dạng.</p>
                </div>

                <!-- HelloPet -->
                <div class="bg-white rounded-2xl shadow-sm border border-gray-100 p-8 hover:shadow-xl hover:-translate-y-1 transition-all duration-300 cursor-pointer slide-up delay-300" onclick="showToast('HelloPet đang được phát triển. Cùng đón chờ nhé!')">
                    <div class="w-14 h-14 bg-pink-100 rounded-xl flex items-center justify-center mb-6 text-pink-600">
                        <i class="fa-solid fa-paw text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-3">HelloPet</h3>
                    <p class="text-gray-600">Cộng đồng và dịch vụ chăm sóc toàn diện dành cho những người bạn bốn chân của bạn.</p>
                </div>

                <!-- HelloShop -->
                <div class="bg-white rounded-2xl shadow-sm border border-gray-100 p-8 hover:shadow-xl hover:-translate-y-1 transition-all duration-300 cursor-pointer slide-up delay-400" onclick="showToast('HelloShop đang được phát triển. Cùng đón chờ nhé!')">
                    <div class="w-14 h-14 bg-purple-100 rounded-xl flex items-center justify-center mb-6 text-purple-600">
                        <i class="fa-solid fa-cart-shopping text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-3">HelloShop</h3>
                    <p class="text-gray-600">Trải nghiệm mua sắm thương mại điện tử tiện lợi, an toàn và ngập tràn ưu đãi mỗi ngày.</p>
                </div>

                <!-- HelloWorld -->
                <div class="bg-white rounded-2xl shadow-sm border border-gray-100 p-8 hover:shadow-xl hover:-translate-y-1 transition-all duration-300 cursor-pointer slide-up delay-500" onclick="showToast('HelloWorld đang được phát triển. Cùng đón chờ nhé!')">
                    <div class="w-14 h-14 bg-red-100 rounded-xl flex items-center justify-center mb-6 text-red-600">
                        <i class="fa-solid fa-play text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-3">HelloWorld</h3>
                    <p class="text-gray-600">Mạng xã hội video ngắn, nơi bạn thoả sức sáng tạo và chia sẻ những khoảnh khắc thú vị.</p>
                </div>

                <!-- Coming Soon -->
                <div class="bg-gray-50 rounded-2xl border-2 border-dashed border-gray-300 p-8 flex flex-col items-center justify-center text-center slide-up delay-500">
                    <div class="w-14 h-14 bg-gray-200 rounded-full flex items-center justify-center mb-4 text-gray-500">
                        <i class="fa-solid fa-plus text-xl"></i>
                    </div>
                    <h3 class="text-lg font-bold text-gray-700 mb-2">Và nhiều hơn nữa</h3>
                    <p class="text-sm text-gray-500">Hệ sinh thái sẽ không ngừng mở rộng trong tương lai.</p>
                </div>

            </div>
        </div>
    </div>

    <!-- About Section -->
    <div id="about" class="py-24 bg-gray-50 border-t border-gray-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="lg:grid lg:grid-cols-2 lg:gap-16 items-center">
                <div class="mb-12 lg:mb-0 slide-up delay-100">
                    <h2 class="text-base text-blue-600 font-semibold tracking-wide uppercase">Về nhà phát triển</h2>
                    <h3 class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">
                        Xin chào, mình là <span class="text-blue-600">Nguyễn Đình Hào</span>
                    </h3>
                    <p class="mt-6 text-lg text-gray-600 leading-relaxed">
                        Là một học sinh lớp 10 với niềm đam mê cháy bỏng dành cho công nghệ và lập trình, mình đã ấp ủ ý tưởng về <strong class="text-gray-900">Hello Ecosystem</strong>. Nhận thấy sự phân mảnh của các dịch vụ trực tuyến hiện nay, mình mong muốn tạo ra một nền tảng thống nhất.
                    </p>
                    <p class="mt-4 text-lg text-gray-600 leading-relaxed">
                        Mục tiêu của dự án này không chỉ là thử thách bản thân trong việc học hỏi kiến thức lập trình mới (từ Web đến App), mà còn là khát vọng xây dựng một hệ sinh thái tiện ích, mang lại giá trị thực tế và trải nghiệm liền mạch cho cộng đồng.
                    </p>
                    <div class="mt-8 flex gap-4">
                        <div class="flex items-center gap-2 text-gray-700">
                            <i class="fa-solid fa-code text-blue-600"></i>
                            <span class="font-medium">Web Developer</span>
                        </div>
                        <div class="flex items-center gap-2 text-gray-700">
                            <i class="fa-solid fa-mobile-screen-button text-blue-600"></i>
                            <span class="font-medium">Future App Maker</span>
                        </div>
                    </div>
                </div>
                
                <div class="relative slide-up delay-300">
                    <div class="relative rounded-2xl overflow-hidden shadow-2xl aspect-[4/3] bg-gradient-to-br from-blue-100 to-indigo-200 flex items-center justify-center group">
                        <div class="absolute inset-0 bg-blue-600 mix-blend-multiply opacity-10 group-hover:opacity-0 transition-opacity duration-300"></div>
                        <!-- Placeholder avatar if you don't have an image yet -->
                        <div class="text-center">
                            <div class="w-32 h-32 bg-white rounded-full mx-auto mb-4 flex items-center justify-center shadow-lg transform group-hover:scale-110 transition-transform duration-300">
                                <span class="text-5xl font-bold text-blue-600">H</span>
                            </div>
                            <p class="text-indigo-800 font-semibold text-xl tracking-wide">Nguyễn Đình Hào</p>
                            <p class="text-indigo-600 text-sm">Founder & Developer</p>
                        </div>
                        
                        <!-- If you have an actual photo, you can replace the div above with an img tag like this: -->
                        <!-- <img src="link-anh-cua-em.jpg" alt="Nguyễn Đình Hào" class="object-cover w-full h-full transform hover:scale-105 transition-transform duration-500"> -->
                    </div>
                    
                    <!-- Decorative elements -->
                    <div class="absolute -bottom-6 -right-6 w-24 h-24 bg-dots pattern-dots text-blue-600 opacity-20"></div>
                </div>
            </div>
        </div>
    </div>

    <!-- Contact Section -->
    <div id="contact" class="py-24 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16 slide-up delay-100">
                <h2 class="text-base text-blue-600 font-semibold tracking-wide uppercase">Liên hệ</h2>
                <p class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">
                    Kết nối với tôi
                </p>
                <p class="mt-4 max-w-2xl mx-auto text-xl text-gray-500">
                    Bạn có câu hỏi, ý tưởng hợp tác hay đơn giản chỉ muốn chia sẻ? Đừng ngần ngại liên hệ nhé.
                </p>
            </div>

            <div class="max-w-4xl mx-auto bg-white rounded-2xl shadow-xl overflow-hidden slide-up delay-200 border border-gray-100">
                <div class="grid grid-cols-1 md:grid-cols-2">
                    <!-- Contact Info -->
                    <div class="bg-blue-600 p-10 text-white flex flex-col justify-center relative overflow-hidden">
                        <!-- Decorative background circle -->
                        <div class="absolute -top-16 -right-16 w-48 h-48 bg-blue-500 rounded-full opacity-50 blur-2xl"></div>
                        
                        <h3 class="text-2xl font-bold mb-8 relative z-10">Thông tin liên hệ</h3>
                        
                        <div class="flex items-center mb-8 relative z-10 hover:translate-x-2 transition-transform duration-300">
                            <div class="w-12 h-12 bg-white/20 rounded-full flex items-center justify-center mr-4 flex-shrink-0 backdrop-blur-sm">
                                <i class="fa-solid fa-phone text-xl"></i>
                            </div>
                            <div>
                                <p class="text-blue-200 text-sm font-medium mb-1">Số điện thoại</p>
                                <a href="tel:0768152277" class="text-xl font-bold hover:text-blue-100 transition-colors">0768 152 277</a>
                            </div>
                        </div>

                        <div class="flex items-center mb-8 relative z-10 hover:translate-x-2 transition-transform duration-300">
                            <div class="w-12 h-12 bg-white/20 rounded-full flex items-center justify-center mr-4 flex-shrink-0 backdrop-blur-sm">
                                <i class="fa-solid fa-envelope text-xl"></i>
                            </div>
                            <div>
                                <p class="text-blue-200 text-sm font-medium mb-1">Email</p>
                                <a href="mailto:nguyendinhhao1201@gmail.com" class="text-lg font-semibold hover:text-blue-100 transition-colors">nguyendinhhao1201@gmail.com</a>
                            </div>
                        </div>

                        <div class="flex items-center relative z-10 hover:translate-x-2 transition-transform duration-300">
                            <div class="w-12 h-12 bg-white/20 rounded-full flex items-center justify-center mr-4 flex-shrink-0 backdrop-blur-sm">
                                <i class="fa-solid fa-location-dot text-xl"></i>
                            </div>
                            <div>
                                <p class="text-blue-200 text-sm font-medium mb-1">Vị trí</p>
                                <p class="text-lg font-semibold">Việt Nam</p>
                            </div>
                        </div>
                    </div>

                    <!-- Contact Form -->
                    <div class="p-10">
                        <h3 class="text-2xl font-bold text-gray-900 mb-6">Gửi tin nhắn</h3>
                        <form onsubmit="event.preventDefault(); showToast('Đã gửi tin nhắn thành công! Mình sẽ phản hồi bạn qua số điện thoại sớm nhất.');">
                            <div class="mb-5">
                                <label for="name" class="block text-sm font-medium text-gray-700 mb-2">Tên của bạn</label>
                                <input type="text" id="name" class="w-full px-4 py-3 bg-gray-50 border border-gray-200 rounded-xl focus:bg-white focus:ring-2 focus:ring-blue-500 focus:border-transparent outline-none transition-all" placeholder="Nguyễn Văn A" required>
                            </div>
                            <div class="mb-5">
                                <label for="message" class="block text-sm font-medium text-gray-700 mb-2">Tin nhắn</label>
                                <textarea id="message" rows="4" class="w-full px-4 py-3 bg-gray-50 border border-gray-200 rounded-xl focus:bg-white focus:ring-2 focus:ring-blue-500 focus:border-transparent outline-none transition-all resize-none" placeholder="Xin chào Hào, tôi muốn hỏi về..." required></textarea>
                            </div>
                            <button type="submit" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-semibold py-3 px-4 rounded-xl transition-all duration-300 shadow-md hover:shadow-xl hover:-translate-y-1 flex justify-center items-center gap-2">
                                Gửi tin nhắn <i class="fa-solid fa-paper-plane"></i>
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Call to Action -->
    <div class="bg-blue-600">
        <div class="max-w-7xl mx-auto py-12 px-4 sm:px-6 lg:py-16 lg:px-8 lg:flex lg:items-center lg:justify-between">
            <h2 class="text-3xl font-extrabold tracking-tight text-white sm:text-4xl">
                <span class="block">Sẵn sàng để bắt đầu?</span>
                <span class="block text-blue-200">Đăng ký tài khoản miễn phí ngay hôm nay.</span>
            </h2>
            <div class="mt-8 flex lg:mt-0 lg:flex-shrink-0">
                <div class="inline-flex rounded-md shadow">
                    <button class="inline-flex items-center justify-center px-5 py-3 border border-transparent text-base font-medium rounded-md text-blue-600 bg-white hover:bg-gray-50 transition-colors">
                        Bắt đầu ngay
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer class="bg-gray-900 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row justify-between items-center">
            <div class="flex justify-center items-center mb-4 md:mb-0">
                <span class="text-2xl font-extrabold text-white tracking-tight">Hello<span class="text-gray-400">Eco</span></span>
            </div>
            <p class="text-gray-400 text-sm text-center md:text-left">
                &copy; 2026 Phát triển bởi Nguyễn Đình Hào. Bảo lưu mọi quyền.
            </p>
            <div class="flex space-x-6 mt-4 md:mt-0 text-gray-400">
                <a href="https://www.facebook.com/share/1G8eYpiJHR/?mibextid=wwXIfr" target="_blank" rel="noopener noreferrer" class="hover:text-white transition-colors"><i class="fa-brands fa-facebook text-xl"></i></a>
                <a href="https://www.tiktok.com/@nguyenhao1201._?_r=1&_t=ZS-97DqaxDofIe" target="_blank" rel="noopener noreferrer" class="hover:text-white transition-colors"><i class="fa-brands fa-tiktok text-xl"></i></a>
                <a href="#" class="hover:text-white transition-colors"><i class="fa-brands fa-github text-xl"></i></a>
            </div>
        </div>
    </footer>

    <!-- Custom Toast Element -->
    <div id="toast">Thông báo</div>

    <script>
        // Function to show custom notification (Toast) instead of alert()
        function showToast(message) {
            const toast = document.getElementById("toast");
            toast.textContent = message;
            toast.className = "show";
            
            // Hide the toast after 3 seconds
            setTimeout(function(){
                toast.className = toast.className.replace("show", "");
            }, 3000);
        }

        // Add intersection observer for scroll animations
        document.addEventListener("DOMContentLoaded", function() {
            const observerOptions = {
                root: null,
                rootMargin: '0px',
                threshold: 0.1
            };

            const observer = new IntersectionObserver((entries, observer) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.animationPlayState = 'running';
                        observer.unobserve(entry.target);
                    }
                });
            }, observerOptions);

            // Pause animations initially until they scroll into view
            document.querySelectorAll('.slide-up').forEach(el => {
                el.style.animationPlayState = 'paused';
                observer.observe(el);
            });
        });
    </script>
</body>
</html>c_ng_th_ng_tin_hello_ecosystem (2).html…]()
