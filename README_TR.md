<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Şerit Tespiti Projesi</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            color: #333;
        }
        header {
            background: #007acc;
            color: #fff;
            padding: 20px;
            text-align: center;
        }
        h1, h2 {
            color: #007acc;
        }
        section {
            margin: 20px auto;
            max-width: 900px;
            padding: 20px;
            background: #fff;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }
        img {
            max-width: 100%;
            height: auto;
            display: block;
            margin: 10px 0;
        }
        .output-gif {
            text-align: center;
        }
        footer {
            text-align: center;
            padding: 10px;
            background: #007acc;
            color: #fff;
            margin-top: 20px;
        }
        code {
            background: #f4f4f4;
            padding: 5px;
            border-radius: 5px;
            font-family: Consolas, monospace;
        }
        .technologies, .how-to-run {
            background-color: #eaf5ff;
            padding: 10px;
            border-left: 5px solid #007acc;
            margin: 10px 0;
        }
    </style>
</head>
<body>

<header>
    <h1>🚗 Şerit Tespiti Projesi</h1>
    <p>Bu proje, görüntü işleme teknikleri kullanarak yol şeritlerini tespit etmeyi amaçlamaktadır.</p>
</header>

<section>
    <h2>📋 Proje Adımları</h2>

    <h3>1. Videodan Görüntü Alınması</h3>
    <p>Videodan analiz için bir kare görsel alınır.</p>
    <img src="Images/test.png" alt="Videodan Görüntü Alınması">

    <h3>2. BGR'den RGB'ye Dönüşüm</h3>
    <p>OpenCV BGR formatında okuduğu görselleri, Matplotlib ile doğru görüntülemek için RGB formatına dönüştürüyoruz.</p>
    <img src="Images/BGRtoRGB.png" alt="BGR Formatı">
    <img src="Images/Matplotlib.png" alt="RGB Formatı">

    <h3>3. Görüntü Boyutlarının Belirlenmesi</h3>
    <p>Görselin boyutları belirlenerek analiz yapılır.</p>
    <img src="Images/Shape.png" alt="Görsel Boyutları">

    <h3>4. Görselin Kesilmesi (ROI)</h3>
    <p>Şeritlerin bulunduğu bölgeye odaklanmak için görsel kesilir.</p>
    <img src="Images/Cropped_Image.png" alt="Kesilmiş Görsel">

    <h3>5. Görseli Gri Formata Dönüştürme</h3>
    <p>Görsel gri tonlamaya dönüştürülerek analiz kolaylaştırılır.</p>
    <img src="Images/Gray.png" alt="Gri Tonlama">

    <h3>6. Kenar Tespiti (Canny Filtresi)</h3>
    <p>Canny algoritması kullanarak kenarlar belirlenir.</p>
    <img src="Images/Canny.png" alt="Canny Filtresi">
    <img src="Images/Cropped_Canny.png" alt="Kesilmiş Canny Görseli">

    <h3>7. Şerit Çizgilerinin Çizilmesi</h3>
    <p>Görselde tespit edilen kenarların üzerine şerit çizgileri çizilir.</p>
</section>

<section class="output-gif">
    <h2>🎥 Çıktı</h2>
    <p>Projenin nihai çıktısı aşağıda gösterilmiştir.</p>
    <img src="Videos/output_gif.gif" alt="Çıktı GIF">
</section>

<section>
    <h2>🛠️ Kullanılan Teknolojiler</h2>
    <div class="technologies">
        <ul>
            <li><strong>Python</strong></li>
            <li><strong>OpenCV</strong> - Görüntü işleme</li>
            <li><strong>Matplotlib</strong> - Görsel analiz</li>
        </ul>
    </div>
</section>

<section>
    <h2>📂 Projeyi Çalıştırma</h2>
    <div class="how-to-run">
        <p>Projeyi çalıştırmak için aşağıdaki adımları takip edebilirsiniz:</p>
        <ol>
            <li>Projeyi klonlayın:  
                <code>git clone https://github.com/username/serit-tespiti.git</code>  
                <code>cd serit-tespiti</code>
            </li>
            <li>Gerekli kütüphaneleri yükleyin:  
                <code>pip install opencv-python matplotlib</code>
            </li>
            <li>Proje dosyasını çalıştırın:  
                <code>python main.py</code>
            </li>
        </ol>
    </div>
</section>

<section>
    <h2>👨‍💻 Geliştirici</h2>
    <p><strong>Adınız Soyadınız</strong></p>
    <p><strong>Email:</strong> your-email@example.com</p>
    <p><strong>LinkedIn:</strong> <a href="https://linkedin.com/in/yourname" target="_blank">Profilinizi Ziyaret Edin</a></p>
</section>

<footer>
    <p>© 2024 Şerit Tespiti Projesi | Tüm Hakları Saklıdır</p>
</footer>

</body>
</html>
