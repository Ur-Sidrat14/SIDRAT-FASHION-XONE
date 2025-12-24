# SIDRAT-FASHION-XONE
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sïdrat Fashion Xone - সিদ্রাত ফ্যাশন জোন</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Noto+Sans+Bengali:wght@400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #d4a574; --dark: #1a1a1a; --light: #f8f9fa; --accent: #ff6b6b;
        }
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Poppins', sans-serif; line-height: 1.6; color: var(--dark); overflow-x: hidden; }
        .bengali { font-family: 'Noto Sans Bengali', sans-serif; }
        
        /* Header */
        header { background: linear-gradient(135deg, var(--primary), #b89e6a); padding: 1rem 0; position: fixed; width: 100%; top: 0; z-index: 1000; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
        nav { display: flex; justify-content: space-between; align-items: center; max-width: 1200px; margin: 0 auto; padding: 0 2rem; }
        .logo { font-size: 1.8rem; font-weight: 700; color: white; text-decoration: none; }
        .logo .bng { font-family: 'Noto Sans Bengali', sans-serif; font-size: 1.5rem; }
        .lang-toggle { background: rgba(255,255,255,0.2); border: none; color: white; padding: 0.5rem 1rem; border-radius: 25px; cursor: pointer; font-weight: 600; }
        
        /* Hero */
        .hero { background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1521572163474-6864f9cf17ab?w=1920') center/cover; height: 100vh; display: flex; align-items: center; justify-content: center; text-align: center; color: white; padding-top: 80px; }
        .hero h1 { font-size: 3.5rem; margin-bottom: 1rem; }
        .hero .bng { font-size: 2.8rem; font-family: 'Noto Sans Bengali', sans-serif; }
        .hero p { font-size: 1.3rem; margin-bottom: 2rem; max-width: 600px; }
        .cta { background: var(--primary); color: white; padding: 1rem 2.5rem; border: none; border-radius: 50px; font-size: 1.1rem; font-weight: 600; cursor: pointer; text-decoration: none; display: inline-block; transition: transform 0.3s; }
        .cta:hover { transform: scale(1.05); }
        
        /* Sections */
        section { padding: 5rem 2rem; max-width: 1200px; margin: 0 auto; }
        h2 { font-size: 2.5rem; text-align: center; margin-bottom: 3rem; color: var(--dark); }
        h2.bng { font-family: 'Noto Sans Bengali', sans-serif; }
        
        /* Products */
        .products { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 2rem; }
        .product-card { background: white; border-radius: 15px; overflow: hidden; box-shadow: 0 10px 30px rgba(0,0,0,0.1); transition: transform 0.3s; }
        .product-card:hover { transform: translateY(-10px); }
        .product-card img { width: 100%; height: 250px; object-fit: cover; }
        .product-info { padding: 1.5rem; }
        .product-info h3 { font-size: 1.3rem; margin-bottom: 0.5rem; }
        .price { font-size: 1.5rem; font-weight: 700; color: var(--primary); }
        
        /* About */
        .about { background: var(--light); }
        
        /* Contact */
        .contact { background: var(--dark); color: white; text-align: center; }
        .contact-info { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 2rem; margin-bottom: 2rem; }
        .contact-item { text-align: center; }
        .contact-item svg { width: 50px; height: 50px; fill: var(--primary); margin-bottom: 1rem; }
        
        /* Footer */
        footer { background: var(--dark); color: white; text-align: center; padding: 2rem; }
        
        /* Responsive */
        @media (max-width: 768px) { .hero h1 { font-size: 2.5rem; } .hero .bng { font-size: 2rem; } nav { padding: 0 1rem; } }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="#" class="logo">Sïdrat Fashion Xone <span class="bng">সিদ্রাত ফ্যাশন জোন</span></a>
            <button class="lang-toggle" onclick="toggleLang()">বাংলা / English</button>
        </nav>
    </header>
    
    <section class="hero">
        <div>
            <h1 id="hero-title">Premium Fashion for You</h1>
            <h1 class="bng" id="hero-title-bng" style="display:none;">তোমার জন্য প্রিমিয়াম ফ্যাশন</h1>
            <p id="hero-desc">Discover latest trends in ethnic wear, casuals & more at unbeatable prices. Shop now!</p>
            <p class="bng" id="hero-desc-bng" style="display:none;">এথনিক পোশাক, ক্যাজুয়াল ও আরো অনেক কিছু সেরা দামে। এখনই কিনুন!</p>
            <a href="#products" class="cta">Shop Now / এখনই কিনুন</a>
        </div>
    </section>
    
    <section id="about" class="about">
        <h2 id="about-title">About Us / আমাদের সম্পর্কে</h2>
        <p id="about-text">Sïdrat Fashion Xone brings you quality fashion from Narnaund, Haryana. We specialize in trendy outfits for men, women & kids with fast delivery across India.</p>
        <p class="bng" id="about-text-bng" style="display:none;">সিদ্রাত ফ্যাশন জোন হারিয়ানার নারনৌন্ড থেকে আপনার জন্য সেরা ফ্যাশন নিয়ে আসে। পুরুষ, মহিলা ও শিশুদের জন্য ট্রেন্ডি পোশাক দ্রুত ডেলিভারি সহ।</p>
    </section>
    
    <section id="products">
        <h2 id="products-title">New Arrivals / নতুন আগমন</h2>
        <div class="products">
            <!-- EDIT THESE: Replace img src with your product photos -->
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-15933422204-8fa6e38b3e72?w=400" alt="Kurtas">
                <div class="product-info">
                    <h3 id="p1-title">Men's Kurta Set</h3>
                    <h3 class="bng" style="display:none;">পুরুষদের কুর্তা সেট</h3>
                    <div class="price">₹1,499</div>
                </div>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1608252542136-0ff451c3b5bd?w=400" alt="Saree">
                <div class="product-info">
                    <h3 id="p2-title">Designer Saree</h3>
                    <h3 class="bng" style="display:none;">ডিজাইনার শাড়ি</h3>
                    <div class="price">₹2,299</div>
                </div>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1598033124237-ce4a55171c93?w=400" alt="Kids">
                <div class="product-info">
                    <h3 id="p3-title">Kids Ethnic Set</h3>
                    <h3 class="bng" style="display:none;">শিশুদের ইথনিক সেট</h3>
                    <div class="price">₹999</div>
                </div>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1445205170230-053b83016050?w=400" alt="Shirt">
                <div class="product-info">
                    <h3 id="p4-title">Casual Shirt</h3>
                    <h3 class="bng" style="display:none;">ক্যাজুয়াল শার্ট</h3>
                    <div class="price">₹799</div>
                </div>
            </div>
        </div>
    </section>
    
    <section id="contact" class="contact">
        <h2 id="contact-title">Contact Us / যোগাযোগ করুন</h2>
        <div class="contact-info">
            <!-- EDIT THESE: Your WhatsApp, Phone, Address -->
            <div class="contact-item">
                <svg viewBox="0 0 24 24"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994
