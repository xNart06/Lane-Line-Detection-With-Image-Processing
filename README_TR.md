# Görüntü İşleme İle Şerit Tespit Sistemi

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
<p align="center">
  <a href="README.md">
    <img src="https://img.shields.io/badge/lang-English-blue.svg" alt="English">
  </a>
  <a href="README_TR.md">
    <img src="https://img.shields.io/badge/lang-Türkçe-red.svg" alt="Türkçe">
  </a>
</p>

## Proje Hakkında

Bu proje, görüntü işleme teknikleri kullanarak, özellikle yol şeritlerinin doğru bir şekilde tespit edilmesine odaklanan bir sistemin oluşturulmasını amaçlamaktadır. Sistem, bir video kaydından veya canlı yayından alınan görüntüleri analiz ederek yol şeritlerini tespit eder ve bu şeritleri görsel olarak işaretler. Bu proje, şerit tespiti için modern görüntü işleme yöntemlerinin uygulamalarını incelemektedir.

• **Hedef**: Yol şeritlerini doğru bir şekilde tanımlamak ve takip etmek. Bu, özellikle otonom araç sistemleri için çok önemlidir.

• **Teknikler**: OpenCV, Matplotlib gibi popüler kütüphaneler kullanılarak, görüntü işleme adımları gerçekleştirilmiştir.

• **Model Durumu**: Proje, belirli bir model eğitimi içermemektedir; yalnızca görüntü işleme adımlarını içeren temel bir uygulamadır.

<h2>📋 Proje Adımları</h2>

<h3>1. Videodan Görüntü Alınması</h3>
<p>Videodan analiz için bir kare görsel alınır. Bu görselin alınma amacı, videoda çalışması için işlemleri ayarlamaktır.</p>
• Bu adım, gerçek zamanlı video akışlarından veri almak için temel bir adımdır.  
<img src="images/test.png" alt="Videodan Görüntü Alınması">

<h3>2. BGR'den RGB'ye Dönüşüm</h3>
<p>OpenCV BGR formatında okuduğu görselleri, Matplotlib ile doğru görüntülemek için RGB formatına dönüştürüyoruz.</p>
• Görüntülerin doğru bir şekilde görselleştirilmesi için renk formatı dönüştürülür.  
<img src="images/BGRtoRGB.png" alt="BGR Formatı">
<img src="images/Matplotlib.png" alt="RGB Formatı">

<h3>3. Görüntü Boyutlarının Belirlenmesi</h3>
<p>Görselin boyutları belirlenerek analiz yapılır.</p>
• Görüntünün genişlik, yükseklik ve kanal sayısı hesaplanır. Bu, sonraki işleme adımlarının doğru uygulanabilmesi için önemlidir.  
<img src="images/Shape.png" alt="Görsel Boyutları">

<h3>4. Görselin Kesilmesi (ROI)</h3>
<p>Şeritlerin bulunduğu bölgeye odaklanmak için görsel kesilir.</p>
• Bu adımda, şeritlerin bulunduğu bölgeyi belirlemek ve gereksiz kısımları kesmek için ROI (Region of Interest) kesimi yapılır.  
<img src="images/Cropped_Image.png" alt="Kesilmiş Görsel">

<h3>5. Bulanıklaştırma ve görseli Gri Formata Dönüştürme</h3>
<p>Görsel gri tonlamaya dönüştürülerek analiz kolaylaştırılır.</p>
• Gri tonlama, görüntüdeki renk bilgilerini atarak sadece parlaklık bilgilerini kullanmaya olanak tanır. Bu, kenar tespiti gibi işlemleri kolaylaştırır.  
<img src="images/Blurred.png" alt="Bulanıklaştırma">
<img src="images/Gray.png" alt="Gri Tonlama">

<h3>6. Kenar Tespiti (Canny Filtresi)</h3>
<p>Canny algoritması kullanarak kenarlar belirlenir.</p>
• Canny kenar algılama filtresi, görüntüdeki kenarları tespit etmek için kullanılır. Bu adım, şeritlerin sınırlarını net bir şekilde tanımlamamıza olanak tanır.  
<img src="images/Canny.png" alt="Canny Filtresi">
<img src="images/Cropped_Canny.png" alt="Kesilmiş Canny Görseli">

<h3>7. Şerit Çizgilerinin Çizilmesi</h3>
<p>Görselde tespit edilen kenarların üzerine şerit çizgileri çizilir.</p>
• Şeritlerin tespitinden sonra, bu kenarlara şerit çizgileri eklenir, böylece yol üzerindeki şeritler net bir şekilde vurgulanır.

<h2>🎥 Çıktı</h2>
<p>Projenin nihai çıktısı aşağıda gösterilmiştir.</p>
<img src="Videos/output.gif" alt="Çıktı GIF">

<h2>🛠️ Kullanılan Teknolojiler</h2>
<ul>
  <li><strong>Python</strong> - Projenin ana programlama dili.</li>
  <li><strong>OpenCV</strong> - Görüntü işleme işlemleri için kullanılan kütüphane.</li>
  <li><strong>Matplotlib</strong> - Görselleri analiz etmek ve görselleştirmek için kullanılan kütüphane.</li>
</ul>

<h2>👨‍💻 Geliştiriciler</h2>
<p><strong>Furkan Hamza BOLAT</strong></p>
<p><strong>Email:</strong> <a href="mailto:furkanhamzabolat@gmail.com">furkanhamzabolat@gmail.com</a></p>
<p><strong>Furkan DAYI</strong></p>
<p><strong>Email:</strong> <a href="mailto:furkan.dyi@hotmail.com">furkan.dyi@hotmail.com</a></p>

