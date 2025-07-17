<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MBTI & Emlak Eğitimi - Müşteri Değil, Karakter Satın Alıyor!</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .header {
            text-align: center;
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            color: white;
            padding: 60px 20px;
            border-radius: 20px;
            margin-bottom: 40px;
            box-shadow: 0 15px 35px rgba(30, 60, 114, 0.3);
            position: relative;
            overflow: hidden;
        }

        .header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            animation: float 6s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(180deg); }
        }

        .header h1 {
            font-size: 3.2em;
            font-weight: 700;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            position: relative;
            z-index: 2;
        }

        .subtitle {
            font-size: 1.3em;
            font-weight: 300;
            opacity: 0.95;
            position: relative;
            z-index: 2;
        }

        .mottos {
            background: white;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            margin-bottom: 40px;
            border-left: 5px solid #17a2b8;
        }

        .motto {
            font-size: 1.2em;
            font-weight: 500;
            margin: 15px 0;
            color: #2a5298;
            padding-left: 30px;
            position: relative;
        }

        .motto::before {
            content: '🎯';
            position: absolute;
            left: 0;
            top: 0;
            font-size: 1.2em;
        }

        .content-section {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            margin-bottom: 40px;
        }

        .info-card {
            background: white;
            padding: 35px;
            border-radius: 15px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .info-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0,0,0,0.15);
        }

        .info-card h2 {
            color: #1e3c72;
            font-size: 1.8em;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
        }

        .info-card h2::before {
            content: '🧠';
            margin-right: 15px;
            font-size: 1.2em;
        }

        .info-card p {
            font-size: 1.1em;
            line-height: 1.7;
            color: #555;
        }

        .education-content {
            background: white;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
            margin-bottom: 40px;
        }

        .education-content h2 {
            color: #1e3c72;
            font-size: 2em;
            margin-bottom: 25px;
            text-align: center;
        }

        .content-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }

        .content-item {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            border-left: 4px solid #17a2b8;
            transition: background 0.3s ease;
        }

        .content-item:hover {
            background: #e9ecef;
        }

        .content-item h3 {
            color: #2a5298;
            font-size: 1.2em;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }

        .content-item h3::before {
            content: '✔️';
            margin-right: 10px;
        }

        .event-details {
            background: linear-gradient(135deg, #17a2b8 0%, #138496 100%);
            color: white;
            padding: 40px;
            border-radius: 15px;
            margin-bottom: 40px;
            text-align: center;
        }

        .event-details h2 {
            font-size: 2em;
            margin-bottom: 25px;
        }

        .details-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }

        .detail-item {
            background: rgba(255,255,255,0.1);
            padding: 20px;
            border-radius: 10px;
            backdrop-filter: blur(10px);
        }

        .detail-item h3 {
            font-size: 1.3em;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .detail-item h3::before {
            content: '📅';
            margin-right: 10px;
        }

        .detail-item:nth-child(2) h3::before { content: '⏱️'; }
        .detail-item:nth-child(3) h3::before { content: '🌐'; }

        .instructor-section {
            background: white;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
            margin-bottom: 40px;
            text-align: center;
        }

        .instructor-section h2 {
            color: #1e3c72;
            font-size: 2em;
            margin-bottom: 20px;
        }

        .instructor-info {
            font-size: 1.3em;
            color: #2a5298;
            margin-bottom: 15px;
            font-weight: 500;
        }

        .instructor-email {
            color: #17a2b8;
            font-size: 1.1em;
        }

        .cta-section {
            text-align: center;
            padding: 40px 0;
        }

        .cta-button {
            display: inline-block;
            background: linear-gradient(135deg, #28a745 0%, #20c997 100%);
            color: white;
            padding: 20px 40px;
            font-size: 1.3em;
            font-weight: 600;
            text-decoration: none;
            border-radius: 50px;
            box-shadow: 0 10px 30px rgba(40, 167, 69, 0.4);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .cta-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
            transition: left 0.6s;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 40px rgba(40, 167, 69, 0.6);
        }

        .cta-button:hover::before {
            left: 100%;
        }

        @media (max-width: 768px) {
            .header h1 {
                font-size: 2.2em;
            }
            
            .content-section {
                grid-template-columns: 1fr;
                gap: 20px;
            }
            
            .details-grid {
                grid-template-columns: 1fr;
            }
            
            .content-list {
                grid-template-columns: 1fr;
            }
            
            .container {
                padding: 10px;
            }
        }

        .floating-elements {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }

        .floating-icon {
            position: absolute;
            font-size: 2em;
            opacity: 0.1;
            animation: floatAround 15s infinite linear;
        }

        .floating-icon:nth-child(1) { top: 10%; left: 10%; animation-delay: 0s; }
        .floating-icon:nth-child(2) { top: 20%; right: 10%; animation-delay: 3s; }
        .floating-icon:nth-child(3) { bottom: 20%; left: 15%; animation-delay: 6s; }
        .floating-icon:nth-child(4) { bottom: 10%; right: 20%; animation-delay: 9s; }

        @keyframes floatAround {
            0% { transform: translateY(0px) rotate(0deg); }
            25% { transform: translateY(-20px) rotate(90deg); }
            50% { transform: translateY(0px) rotate(180deg); }
            75% { transform: translateY(20px) rotate(270deg); }
            100% { transform: translateY(0px) rotate(360deg); }
        }
    </style>
</head>
<body>
    <div class="floating-elements">
        <div class="floating-icon">🏡</div>
        <div class="floating-icon">🧠</div>
        <div class="floating-icon">📊</div>
        <div class="floating-icon">🎯</div>
    </div>

    <div class="container">
        <div class="header">
            <h1>Müşteri Değil, Karakter Satın Alıyor!</h1>
            <div class="subtitle">MBTI ile Emlak Sektöründe Profesyonel Satış Stratejileri</div>
        </div>

        <div class="mottos">
            <div class="motto">Doğru ev satmak, doğru kişiliği okumakla başlar.</div>
            <div class="motto">Emlak Sektöründe Kişilik Tiplerine Göre Satış Stratejileri</div>
            <div class="motto">Satış bir matematik değil; kişilik çözümüdür.</div>
        </div>

        <div class="content-section">
            <div class="info-card">
                <h2>Neden MBTI?</h2>
                <p>Emlak sektöründe başarı, sadece mükemmel lokasyon ve fiyatla değil, müşterinin kişiliğini doğru okuyarak ona uygun yaklaşım sergilemekle gelir. MBTI, her müşterinin benzersiz karar verme sürecini anlayarak satış stratejinizi kişiselleştirmenizi sağlar.</p>
            </div>
            
            <div class="info-card">
                <h2>Fark Yaratın</h2>
                <p>Rakipleriniz fiyat ve özellik sunarken, siz müşterinin ruhuna hitap edin. Kişilik tiplerini anlayan emlak danışmanları %40 daha yüksek closing oranına sahiptir. Bu eğitimle siz de bu avantajı elde edeceksiniz.</p>
            </div>
        </div>

        <div class="education-content">
            <h2>📚 Eğitim İçeriği</h2>
            <div class="content-list">
                <div class="content-item">
                    <h3>MBTI Temel Farkları</h3>
                    <p>16 kişilik tipinin emlak kararlarındaki etkilerini öğrenin</p>
                </div>
                <div class="content-item">
                    <h3>Müşteri Davranış Örüntüleri</h3>
                    <p>Kişilik tipine göre satın alma motivasyonlarını keşfedin</p>
                </div>
                <div class="content-item">
                    <h3>Kişiliğe Göre Satış Yaklaşımı</h3>
                    <p>Her tip için özel satış stratejileri geliştirin</p>
                </div>
                <div class="content-item">
                    <h3>Rol Canlandırma</h3>
                    <p>Gerçek senaryolarla pratik uygulama yapın</p>
                </div>
                <div class="content-item">
                    <h3>Danışman-Müşteri Uyumu</h3>
                    <p>Kendi kişiliğinizle müşteri kişiliğini eşleştirin</p>
                </div>
                <div class="content-item">
                    <h3>Müşteri Profili Okuma</h3>
                    <p>İlk 5 dakikada kişilik tipini tespit etme teknikleri</p>
                </div>
            </div>
        </div>

        <div class="event-details">
            <h2>🗓️ Eğitim Detayları</h2>
            <div class="details-grid">
                <div class="detail-item">
                    <h3>Tarih</h3>
                    <p>01 Ağustos 2025 itibarıyla<br><small>(Kesin tarih için irtibata geçiniz)</small></p>
                </div>
                <div class="detail-item">
                    <h3>Süre</h3>
                    <p>90 dakika<br>Yoğun ve etkili içerik</p>
                </div>
                <div class="detail-item">
                    <h3>Format</h3>
                    <p>Online / Yüz yüze<br>Esnek katılım seçeneği</p>
                </div>
            </div>
        </div>

        <div class="instructor-section">
            <h2>👨‍🏫 Eğitmen</h2>
            <div class="instructor-info">Dr. Haluk Sak</div>
            <div>Yönetim ve Organizasyon Uzmanı</div>
            <div class="instructor-email">haluksak@gmail.com</div>
        </div>

        <div class="cta-section">
            <a href="mailto:haluksak@gmail.com?subject=MBTI Emlak Eğitimi Hakkında Bilgi&body=Merhaba Dr. Haluk Sak,%0A%0AMBTI ile Emlak Satış Stratejileri eğitimine katılmak istiyorum. Detaylı bilgi alabilir miyim?" class="cta-button">
                📩 Katılmak İçin Bilgi Alın
            </a>
        </div>
    </div>
    <!-- Yazdır Butonu -->
<div style="text-align: center; margin-bottom: 60px;">
  <button onclick="printPage()" style="padding: 15px 30px; font-size: 1.2em; border-radius: 8px; background-color: #1e3c72; color: white; border: none; cursor: pointer; box-shadow: 0 5px 15px rgba(0,0,0,0.2);">
    🖨️ Sayfayı Yazdır
  </button>
</div>

<script>
  function printPage() {
    window.print();
  }
</script>
</body>
</html>
