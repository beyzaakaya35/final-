# final-
my website
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>Mavi Zihin Psikolojik Danışmanlık</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- Bootstrap -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

    <!-- CSS -->
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <!-- <header class="text-center py-5">
    <div class="logo">BK</div>
    <h1 class="site-title"></h1>
    <p class="site-subtitle"></p> -->
    <header class="text-center py-5">
    <img src="logooo bk.png" width="5000" height="250" class="logo-img" alt="Logo">
    
</header>

</header>


<div class="overlay">

    <!-- HEADER -->
    <header class="text-center py-5">
        <h1 class="site-title">Mavi Zihin</h1>
        <p class="site-subtitle">Zihninizdeki dalgalar sakinleşsin</p>
        <p>Güçlü Olmak Değil,Farkında Olmak İyileştirir</p>

    </header>

    <!-- NAV -->
    <div class="container text-center mb-4">
        <button class="btn btn-info mx-2" onclick="toggleBox('about')">Hakkımda</button>
        <button class="btn btn-info mx-2" onclick="toggleBox('services')">Hizmetlerimiz</button>
        <button class="btn btn-info mx-2" onclick="toggleBox('contact')">İletişim</button>
    </div>

    <div class="container">

        <!-- HAKKIMDA -->
        <div id="about" class="content-box">
            <h2>Hakkımda</h2>
            <p>
                   Ben Psikolog Beyza Kaya. 
        Her insan zaman zaman yorulur.Düşünceler ağırlaşır,duygular karışır.
        Bu alan;kendini anlaman,duygularını fark etmen ve iç huzurunu yeniden inşa etmen için var.
        
            </p>
            
                <p>Güvenli, sakin ve destekleyici bir alanda kendini keşfetmeye hazır mısın?</p>
        <p>Burada yargı yok,acele yok.Sadece sen varsın. </p>
            
        </div>

        <!-- HİZMETLER -->
        <div id="services" class="content-box">
            <h2>Hizmetlerimiz</h2>
            <ul>
                <li><strong>Bireysel Terapi:</strong> Kaygı, stres ve özgüven problemleri</li>
                <li><strong>Depresyon Danışmanlığı:</strong> Duygusal yüklerle baş etme</li>
                <li><strong>Ergen Danışmanlığı:</strong> Kimlik, sınav ve uyum sorunları</li>
                <li><strong>Çift Terapisi:</strong> İletişim ve ilişki güçlendirme</li>
                <li><strong>Stres Yönetimi:</strong> Nefes ve farkındalık çalışmaları</li>
                <li><strong>Motivasyon & Hedef:</strong> Yaşam amaçlarını netleştirme</li>
            </ul>
        </div>

        <!-- İLETİŞİM -->
        <div id="contact" class="content-box">
            <h2>İletişim</h2>
            <p>📞 <strong>05XX XXX XX XX</strong></p>
            <p>📸 <strong>@mavizihinpsikoloji</strong></p>
        </div>

        <!-- MOTİVASYON -->
        <div class="motivation text-center mt-5" id="motivation">
            Motivasyon sözü yükleniyor...
        </div>

        <!-- GÖRSELLER -->
        <div class="row mt-5 justify-content-center">
            <div class="col-md-5 mb-3">
                <img src="deniz.jpg" class="img-fluid rounded-4">
            </div>
            <div class="col-md-5 mb-3">
                <img src="terapi.jpg" class="img-fluid rounded-4">
            </div>
        </div>

    </div>

    <footer class="text-center mt-5 pb-4">
        © 2025 Mavi Zihin Psikolojik Danışmanlık
    </footer>

</div>

<script>
    function toggleBox(id) {
        const box = document.getElementById(id);
        box.style.display = box.style.display === "block" ? "none" : "block";
    }

    const sozler = [
        "Kendine nazik ol, iyileşme böyle başlar.",
        "Bugün kendin için küçük bir adım at.",
        "Her şey geçer, sen güçlüsün.",
        "Zihnin sakinleştiğinde kalbin konuşur."
    ];

    document.getElementById("motivation").innerText =
        sozler[Math.floor(Math.random() * sozler.length)];
</script>

    <!-- FORM -->
    <form class="contact-form">
        <input type="text" placeholder="Ad Soyad" required>
        <input type="email" placeholder="E-posta" required>
        <textarea placeholder="Mesajınız"></textarea>
        <button type="submit">Gönder</button>
    </form>
</section>


</body>
</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Segoe UI", sans-serif;

}
.logo {
    width: 90px;
    height: 90px;
    margin: 0 auto 15px;
    border-radius: 50%;
    background: linear-gradient(135deg, #40e0d0, #0077b6);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 32px;
    font-weight: bold;
    color: white;
    letter-spacing: 2px;
    box-shadow: 0 8px 20px rgba(0,0,0,0.4);
}

.logo-img {
    width: 100px;
    margin-bottom: 15px;
}


body {
    min-height: 100vh;
    background-image: url("https://images.unsplash.com/photo-1500530855697-b586d89ba3ee");
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    color: white;
}

.overlay {
    min-height: 100vh;
    background: rgba(0, 90, 120, 0.65);
}

.site-title {
    font-size: 48px;
    color: #e0ffff;
}

.site-subtitle {
    font-size: 18px;
    color: #ccefff;
}

.content-box {
    display: none;
    background: rgba(255, 255, 255, 0.15);
    border-radius: 20px;
    padding: 30px;
    margin-top: 25px;
    backdrop-filter: blur(6px);
}

.content-box h2 {
    color: #e0ffff;
    margin-bottom: 15px;
}

.content-box p,
.content-box li {
    line-height: 1.7;
}

.motivation {
    font-size: 22px;
    font-style: italic;
    color: #f0ffff;
}
/* FORM */
form {
    max-width: 400px;
    margin: auto;
}

form input,
form textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 15px;
}

form button {
    width: 100%;
    padding: 12px;
    background-color: teal;
    color: white;
    border: none;
    border-radius: 25px;
}

footer {
    font-size: 14px;
    color: #ccefff;
}
.logo-img {
    width: 100px;
    margin-bottom: 15px;
}

