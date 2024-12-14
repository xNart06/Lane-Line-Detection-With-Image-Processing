

<header>
    <h1>Görüntü İşleme İle Şerit Tespit Sistemi</h1>
</header>
<p align="center">
  <a href="https://opencv.org/">
    <img src="https://img.shields.io/badge/OpenCV-4.x-blue?logo=opencv&logoColor=white" alt="OpenCV">
  </a>
  <a href="https://numpy.org/">
    <img src="https://img.shields.io/badge/NumPy-1.x-orange?logo=numpy&logoColor=white" alt="NumPy">
  </a>
  <a href="https://matplotlib.org/">
    <img src="https://img.shields.io/badge/Matplotlib-3.x-green?logo=matplotlib&logoColor=white" alt="Matplotlib">
  </a>
</p>

## Proje Hakkında
Bu proje, görüntü işleme teknikleri kullanılarak şerit tespit sistemi yapmayı amaçlamaktadır. Model eğitilmemiştir.
<section>
<h2>📋 Proje Adımları</h2>

<h3>1. Videodan Görüntü Alınması</h3>
- Videodan analiz için bir kare görsel alınır. Bu görselin alınma amacı, videoda çalışması için işlemleri ayarlamaktır.
- skjvşfsdv
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
    <h2>👨‍💻 Geliştiriciler</h2>
    <p><strong>Adınız Soyadınız</strong></p>
    <p><strong>Email:</strong> your-email@example.com</p>
    <p><strong>LinkedIn:</strong> <a href="https://linkedin.com/in/yourname" target="_blank">Profilinizi Ziyaret Edin</a></p>
</section>

<footer>
    <p>© 2024 Şerit Tespiti Projesi | Tüm Hakları Saklıdır</p>
</footer>

</body>
</html>
