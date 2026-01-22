DERİN ÖĞRENME İLE MEME ULTRASON TÜMÖRÜ SINIFLANDIRMASI
YILDIZ TEKNİK ÜNİVERSİTESİ - BİLGİSAYAR MÜHENDİSLİĞİ BÖLÜMÜ
ARA PROJE (OCAK 2026)

🚀 PROJENİN TEKNİK DERİNLİĞİ VE EMEK ANALİZİ
Bu proje, sadece bir sınıflandırma modeli değil, 80'den fazla bağımsız eğitim senaryosunu içeren devasa bir deneysel çalışmadır. Projenin sıradan çalışmalardan farkı, her modelin en ince ayrıntısına kadar optimize edilmesi ve farklı veri setleri arasında "Bilgi Aktarımı" mühendisliği yapılmış olmasıdır.

1. Kapsamlı Hiperparametre Optimizasyonu (80+ Deney)
Her bir mimari (CNN ve Transformer), ezbere dayalı bir öğrenmeyi engellemek adına 3 farklı Öğrenme Oranı (Learning Rate: 10⁻³, 10⁻⁴, 10⁻⁵) ile ayrı ayrı eğitilmiştir.
Toplamda 80'e yakın eğitim döngüsü gerçekleştirilerek her modelin en kararlı çalıştığı "çalışma noktası" tespit edilmiştir.
Bu hassas ayar sayesinde, tıbbi görüntü teşhisinde kritik olan hata payları minimuma indirilmiştir.

2. Alan Uyarlaması (Domain Adaptation - DA) Stratejisi
Projenin en güçlü mühendislik kısmı, modellerin farklı klinik ortamlarına uyum sağlama yeteneğidir:
Süreç: Modeller önce BUSI veri setiyle eğitilmiş, ardından bu ön-bilgiler kullanılarak farklı cihazlardan alınan BUS-UCLM veri setine uyarlanmıştır.
Sonuç: Bu strateji sayesinde, kısıtlı veriye sahip klinik ortamlarda bile yüksek genelleme kapasitesi elde edilmiştir.


📊 KULLANILAN MİMARİLER VE PERFORMANS
Evrişimli Sinir Ağları (CNN) - Transfer Learning
6 farklı mimari üzerinde yoğun Learning Rate (LR) deneyleri yapılmıştır:
EfficientNet, InceptionV3, ResNet-50, DenseNet, NasNetLarge ve Xception.
Vision Transformer (ViT) - Modern SOTA Yaklaşımlar
Görüntünün tamamına odaklanan self-attention mekanizmalı en güncel modeller karşılaştırılmıştır:
CaiT (En İyi Performans: %91,30), BEIT, Swin Transformer, DeiT-Tiny ve Standart ViT.

📈 DENEYSEL SONUÇLAR TABLOSU
Yöntem,Model Adı,Accuracy,Precision,F1-Score
Transformer (TL),CaiT,0.9130,0.9310,0.9084
Alan Uyarlaması (DA),EfficientNet,0.9260,0.8870,0.9030
Transformer (TL),BEIT,0.8957,0.9266,0.8953
CNN (TL),InceptionV3,0.8783,0.9247,0.8269
Alan Uyarlaması (DA),ResNet-50,0.8675,0.8745,0.8537

🛠️ KURULUM VE KULLANIM
Gerekli kütüphaneleri yüklemek için terminale şu komutu yazınız: pip install -r requirements.txt
Bu çalışma, Yıldız Teknik Üniversitesi Bilgisayar Mühendisliği Bölümü "Bilgisayar Projesi" dersi kapsamında Ceyda Babuz ve Muhammed Dilber tarafından, Prof. Dr. Gökhan Bilgin danışmanlığında akademik bir karar destek mekanizması olarak tamamlanmıştır.
