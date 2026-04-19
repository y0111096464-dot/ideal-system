<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>إبداع | وكالة التصميم والتطوير المتكاملة</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Cairo', sans-serif;
            scroll-behavior: smooth;
        }
        .hero-pattern {
            background-color: #ffffff;
            background-image: radial-gradient(#3b82f6 0.5px, #ffffff 0.5px);
            background-size: 24px 24px;
            background-opacity: 0.1;
        }
        .nav-blur {
            backdrop-filter: blur(12px);
            background-color: rgba(255, 255, 255, 0.85);
        }
        .animate-float {
            animation: float 6s ease-in-out infinite;
        }
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }
        .reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s ease-out;
        }
        .reveal.active {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body class="bg-white text-gray-900">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 nav-blur border-b border-gray-100">
        <div class="max-w-7xl mx-auto px-6">
            <div class="flex justify-between h-20 items-center">
                <div class="flex items-center">
                    <a href="#" class="text-2xl font-extrabold tracking-tighter text-black flex items-center gap-2">
                        <div class="w-8 h-8 bg-blue-600 rounded-lg"></div>
                        <span>إبداع.</span>
                    </a>
                </div>
                <div class="hidden md:flex items-center space-x-10 space-x-reverse font-medium">
                    <a href="#home" class="text-blue-600">الرئيسية</a>
                    <a href="#projects" class="text-gray-600 hover:text-blue-600 transition">أعمالنا</a>
                    <a href="#services" class="text-gray-600 hover:text-blue-600 transition">خدماتنا</a>
                    <a href="#testimonials" class="text-gray-600 hover:text-blue-600 transition">عملائنا</a>
                    <a href="#contact" class="bg-blue-600 text-white px-6 py-2.5 rounded-full hover:bg-blue-700 transition shadow-md">ابدأ مشروعك</a>
                </div>
                <button id="menu-btn" class="md:hidden p-2 text-gray-600">
                    <svg class="w-7 h-7" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
                </button>
            </div>
        </div>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-b border-gray-200 p-6 flex flex-col space-y-4">
            <a href="#home" class="text-lg font-bold">الرئيسية</a>
            <a href="#projects" class="text-lg">أعمالنا</a>
            <a href="#services" class="text-lg">خدماتنا</a>
            <a href="#contact" class="text-blue-600 font-bold">تواصل معنا</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-pattern min-h-screen flex items-center pt-20 px-6">
        <div class="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
            <div class="text-right">
                <span class="inline-block px-4 py-1.5 bg-blue-50 text-blue-600 rounded-full text-sm font-bold mb-6">وكالة رقمية رائدة في المنطقة</span>
                <h1 class="text-5xl md:text-7xl font-extrabold leading-tight mb-8">
                    نصمم المستقبل <br> <span class="text-transparent bg-clip-text bg-gradient-to-l from-blue-600 to-indigo-500">بلمسة إبداعية.</span>
                </h1>
                <p class="text-xl text-gray-600 mb-10 leading-relaxed max-w-xl">
                    نحن نؤمن بأن كل علامة تجارية تستحق أن تكون فريدة. نجمع بين أحدث تقنيات الويب وأرقى معايير التصميم العالمي لنضعك في المقدمة.
                </p>
                <div class="flex flex-wrap gap-4">
                    <a href="#projects" class="bg-black text-white px-10 py-4 rounded-2xl font-bold text-lg hover:scale-105 transition shadow-xl">استكشف أعمالنا</a>
                    <div class="flex items-center gap-3 px-6 py-4">
                        <div class="flex -space-x-3 space-x-reverse">
                            <div class="w-10 h-10 rounded-full border-2 border-white bg-gray-200"></div>
                            <div class="w-10 h-10 rounded-full border-2 border-white bg-blue-200"></div>
                            <div class="w-10 h-10 rounded-full border-2 border-white bg-indigo-200"></div>
                        </div>
                        <span class="text-sm font-bold">+500 عميل سعيد</span>
                    </div>
                </div>
            </div>
            <div class="hidden lg:block relative">
                <div class="absolute -top-20 -left-20 w-64 h-64 bg-blue-100 rounded-full blur-3xl opacity-50"></div>
                <div class="animate-float relative z-10">
                    <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&q=80&w=800" alt="[بيئة عمل برمجية]" class="rounded-3xl shadow-2xl border-8 border-white">
                </div>
                <div class="absolute -bottom-10 -right-10 bg-white p-6 rounded-2xl shadow-xl z-20 border border-gray-100">
                    <p class="text-3xl font-bold text-blue-600">98%</p>
                    <p class="text-gray-500 text-sm">معدل رضاء العملاء</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="py-16 bg-gray-50 border-y border-gray-100">
        <div class="max-w-7xl mx-auto px-6 grid grid-cols-2 md:grid-cols-4 gap-8">
            <div class="text-center">
                <p class="text-4xl font-bold mb-2">120+</p>
                <p class="text-gray-500">مشروع مكتمل</p>
            </div>
            <div class="text-center">
                <p class="text-4xl font-bold mb-2">15+</p>
                <p class="text-gray-500">جائزة تصميم</p>
            </div>
            <div class="text-center">
                <p class="text-4xl font-bold mb-2">8</p>
                <p class="text-gray-500">سنوات خبرة</p>
            </div>
            <div class="text-center">
                <p class="text-4xl font-bold mb-2">100%</p>
                <p class="text-gray-500">التزام بالمواعيد</p>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-24 px-6">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-20 reveal">
                <h2 class="text-4xl md:text-5xl font-extrabold mb-6">أعمال نفخر بها</h2>
                <div class="w-20 h-1.5 bg-blue-600 mx-auto rounded-full"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-10">
                <!-- Project Item -->
                <div class="group reveal cursor-pointer">
                    <div class="relative overflow-hidden rounded-[2rem] bg-gray-100 mb-6 aspect-[4/5]">
                        <img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?auto=format&fit=crop&q=80&w=800" alt="[مشروع برمجي]" class="w-full h-full object-cover transition duration-700 group-hover:scale-110">
                        <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition duration-500 flex items-end p-8">
                            <button class="bg-white text-black px-6 py-2 rounded-full font-bold">عرض التفاصيل</button>
                        </div>
                    </div>
                    <p class="text-blue-600 font-bold text-sm mb-2 uppercase">تطوير ويب</p>
                    <h3 class="text-2xl font-bold group-hover:text-blue-600 transition">منصة التعليم الذكي</h3>
                </div>

                <div class="group reveal cursor-pointer" style="transition-delay: 200ms;">
                    <div class="relative overflow-hidden rounded-[2rem] bg-gray-100 mb-6 aspect-[4/5]">
                        <img src="https://images.unsplash.com/photo-1523206489230-c012c64b2b48?auto=format&fit=crop&q=80&w=800" alt="[تطبيق جوال]" class="w-full h-full object-cover transition duration-700 group-hover:scale-110">
                        <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition duration-500 flex items-end p-8">
                            <button class="bg-white text-black px-6 py-2 rounded-full font-bold">عرض التفاصيل</button>
                        </div>
                    </div>
                    <p class="text-blue-600 font-bold text-sm mb-2 uppercase">تطبيقات الجوال</p>
                    <h3 class="text-2xl font-bold group-hover:text-blue-600 transition">تطبيق "صحتي"</h3>
                </div>

                <div class="group reveal cursor-pointer" style="transition-delay: 400ms;">
                    <div class="relative overflow-hidden rounded-[2rem] bg-gray-100 mb-6 aspect-[4/5]">
                        <img src="https://images.unsplash.com/photo-1561070791-26c11d204a3d?auto=format&fit=crop&q=80&w=800" alt="[هوية بصرية]" class="w-full h-full object-cover transition duration-700 group-hover:scale-110">
                        <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition duration-500 flex items-end p-8">
                            <button class="bg-white text-black px-6 py-2 rounded-full font-bold">عرض التفاصيل</button>
                        </div>
                    </div>
                    <p class="text-blue-600 font-bold text-sm mb-2 uppercase">براندينج</p>
                    <h3 class="text-2xl font-bold group-hover:text-blue-600 transition">هوية شركة كابيتال</h3>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-24 bg-gray-950 text-white overflow-hidden">
        <div class="max-w-7xl mx-auto px-6">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-20">
                <div>
                    <h2 class="text-4xl md:text-6xl font-extrabold mb-10 leading-tight">حلولنا تدمج بين <span class="text-blue-500">الفن والتقنية.</span></h2>
                    <p class="text-gray-400 text-xl mb-12">لا نكتفي ببناء المواقع، بل نصنع واجهات رقمية تحول الزوار إلى عملاء دائمين.</p>
                    <div class="space-y-4">
                        <div class="flex items-center gap-4 bg-gray-900 p-6 rounded-2xl border border-gray-800 hover:border-blue-500 transition cursor-default">
                            <div class="w-12 h-12 bg-blue-600/20 rounded-xl flex items-center justify-center text-blue-500">
                                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 4a2 2 0 114 0v1a1 1 0 001 1h3a1 1 0 011 1v3a1 1 0 01-1 1h-1a2 2 0 100 4h1a1 1 0 011 1v3a1 1 0 01-1 1h-3a1 1 0 01-1-1v-1a2 2 0 11-4 0v1a1 1 0 01-1 1H7a1 1 0 01-1-1v-3a1 1 0 011-1h1a2 2 0 100-4H7a1 1 0 01-1-1V7a1 1 0 011-1h3a1 1 0 001-1V4z"></path></svg>
                            </div>
                            <h4 class="text-xl font-bold">تصميم واجهات UI/UX</h4>
                        </div>
                        <div class="flex items-center gap-4 bg-gray-900 p-6 rounded-2xl border border-gray-800 hover:border-blue-500 transition cursor-default">
                            <div class="w-12 h-12 bg-indigo-600/20 rounded-xl flex items-center justify-center text-indigo-500">
                                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"></path></svg>
                            </div>
                            <h4 class="text-xl font-bold">تطوير الويب المتطور</h4>
                        </div>
                    </div>
                </div>
                <div class="relative">
                    <div class="grid grid-cols-2 gap-4">
                        <div class="space-y-4">
                            <div class="bg-gray-900 aspect-square rounded-[2rem] p-8 border border-gray-800">
                                <p class="text-blue-500 font-bold mb-4">01</p>
                                <h5 class="text-xl font-bold mb-2">استشارات برمجية</h5>
                                <p class="text-sm text-gray-500">نخطط لمشروعك من الصفر لضمان النجاح.</p>
                            </div>
                            <div class="bg-blue-600 aspect-square rounded-[2rem] p-8 text-white">
                                <p class="font-bold mb-4">02</p>
                                <h5 class="text-xl font-bold mb-2">سرعة فائقة</h5>
                                <p class="text-sm text-blue-100">نضمن أن موقعك يعمل بسرعة البرق على كل الأجهزة.</p>
                            </div>
                        </div>
                        <div class="space-y-4 pt-12">
                            <div class="bg-gray-800 aspect-square rounded-[2rem] p-8">
                                <p class="text-blue-500 font-bold mb-4">03</p>
                                <h5 class="text-xl font-bold mb-2">دعم فني</h5>
                                <p class="text-sm text-gray-400">نحن معك دائماً حتى بعد إطلاق المشروع.</p>
                            </div>
                            <div class="bg-gray-900 aspect-square rounded-[2rem] p-8 border border-gray-800">
                                <p class="text-blue-500 font-bold mb-4">04</p>
                                <h5 class="text-xl font-bold mb-2">محركات البحث</h5>
                                <p class="text-sm text-gray-500">تهيئة موقعك لتصدر نتائج البحث الأولى.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section id="testimonials" class="py-24 bg-white px-6">
        <div class="max-w-7xl mx-auto">
            <h2 class="text-4xl font-extrabold text-center mb-16">ماذا يقول شركاؤنا؟</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-gray-50 p-10 rounded-[2.5rem] border border-gray-100">
                    <div class="flex text-yellow-400 mb-4">★★★★★</div>
                    <p class="text-gray-600 italic mb-8">"تعاملنا مع الكثير من الوكالات، ولكن فريق إبداع قدم لنا شيئاً مختلفاً تماماً. الاهتمام بالتفاصيل كان مذهلاً."</p>
                    <div class="flex items-center gap-4">
                        <div class="w-12 h-12 rounded-full bg-blue-100"></div>
                        <div>
                            <p class="font-bold">أحمد علي</p>
                            <p class="text-sm text-gray-500">مدير شركة تك-لاين</p>
                        </div>
                    </div>
                </div>
                <div class="bg-blue-600 p-10 rounded-[2.5rem] text-white">
                    <div class="flex text-blue-200 mb-4">★★★★★</div>
                    <p class="italic mb-8">"التطبيق الذي قاموا بتطويره غير مسار شركتنا بالكامل. السرعة والدقة في التنفيذ كانت فوق التوقعات."</p>
                    <div class="flex items-center gap-4">
                        <div class="w-12 h-12 rounded-full bg-blue-400"></div>
                        <div>
                            <p class="font-bold">سارة محمود</p>
                            <p class="text-sm text-blue-200">مؤسسة منصة أثر</p>
                        </div>
                    </div>
                </div>
                <div class="bg-gray-50 p-10 rounded-[2.5rem] border border-gray-100">
                    <div class="flex text-yellow-400 mb-4">★★★★★</div>
                    <p class="text-gray-600 italic mb-8">"أفضل تجربة تصميم مريحة واحترافية خضتها. الموقع أصبح واجهتنا الأساسية لجذب المستثمرين."</p>
                    <div class="flex items-center gap-4">
                        <div class="w-12 h-12 rounded-full bg-blue-100"></div>
                        <div>
                            <p class="font-bold">خالد حسن</p>
                            <p class="text-sm text-gray-500">المدير التقني لشركة فلو</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section id="contact" class="py-24 px-6">
        <div class="max-w-5xl mx-auto bg-gradient-to-r from-blue-600 to-indigo-700 rounded-[3rem] p-12 md:p-20 text-white text-center relative overflow-hidden shadow-2xl">
            <div class="absolute top-0 right-0 w-64 h-64 bg-white/10 rounded-full -mr-32 -mt-32"></div>
            <div class="relative z-10">
                <h2 class="text-4xl md:text-6xl font-extrabold mb-8">جاهز لتحويل فكرتك <br>إلى واقع ملموس؟</h2>
                <p class="text-xl text-blue-100 mb-12 max-w-2xl mx-auto">سواء كنت شركة ناشئة أو مؤسسة كبيرة، نحن هنا لمساعدتك في رحلة التحول الرقمي.</p>
                <div class="flex flex-col sm:flex-row justify-center gap-6">
                    <a href="mailto:hello@ebda.com" class="bg-white text-blue-600 px-10 py-4 rounded-2xl font-extrabold text-lg hover:bg-gray-100 transition shadow-lg">تواصل معنا اليوم</a>
                    <a href="#" class="border border-white/30 bg-white/10 backdrop-blur-md px-10 py-4 rounded-2xl font-extrabold text-lg hover:bg-white/20 transition">احجز استشارة مجانية</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-white py-16 px-6 border-t border-gray-100">
        <div class="max-w-7xl mx-auto">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-16">
                <div class="col-span-1 md:col-span-2">
                    <a href="#" class="text-2xl font-extrabold mb-6 block">إبداع.</a>
                    <p class="text-gray-500 max-w-sm mb-6 leading-relaxed">وكالة تصميم رقمية متخصصة في خلق تجارب استثنائية للمستخدمين وتطوير حلول برمجية مبتكرة.</p>
                    <div class="flex space-x-4 space-x-reverse">
                        <a href="#" class="w-10 h-10 rounded-full bg-gray-100 flex items-center justify-center hover:bg-blue-600 hover:text-white transition"><svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"/></svg></a>
                        <a href="#" class="w-10 h-10 rounded-full bg-gray-100 flex items-center justify-center hover:bg-blue-600 hover:text-white transition"><svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/></svg></a>
                    </div>
                </div>
                <div>
                    <h5 class="font-bold mb-6 text-lg">روابط سريعة</h5>
                    <ul class="space-y-4 text-gray-500">
                        <li><a href="#" class="hover:text-blue-600 transition">من نحن</a></li>
                        <li><a href="#" class="hover:text-blue-600 transition">خدماتنا</a></li>
                        <li><a href="#" class="hover:text-blue-600 transition">أعمالنا</a></li>
                        <li><a href="#" class="hover:text-blue-600 transition">المدونة</a></li>
                    </ul>
                </div>
                <div>
                    <h5 class="font-bold mb-6 text-lg">قانوني</h5>
                    <ul class="space-y-4 text-gray-500">
                        <li><a href="#" class="hover:text-blue-600 transition">سياسة الخصوصية</a></li>
                        <li><a href="#" class="hover:text-blue-600 transition">الشروط والأحكام</a></li>
                        <li><a href="#" class="hover:text-blue-600 transition">اتفاقية الخدمة</a></li>
                    </ul>
                </div>
            </div>
            <div class="pt-8 border-t border-gray-100 flex flex-col md:flex-row justify-between items-center text-gray-400 text-sm">
                <p>© 2024 وكالة إبداع الرقمية. جميع الحقوق محفوظة.</p>
                <p>صنع بكل ❤️ في المنطقة العربية</p>
            </div>    ياسر حسين 
        </div>
    </footer>

    <script>
        // Reveal elements on scroll
        function reveal() {
            var reveals = document.querySelectorAll(".reveal");
            for (var i = 0; i < reveals.length; i++) {
                var windowHeight = window.innerHeight;
                var elementTop = reveals[i].getBoundingClientRect().top;
                var elementVisible = 150;
                if (elementTop < windowHeight - elementVisible) {
                    reveals[i].classList.add("active");
                }
            }
        }
        window.addEventListener("scroll", reveal);

        // Mobile Menu Logic
        const menuBtn = document.getElementById('menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Trigger reveal once on load
        reveal();
    </script>
</body>
</html>
