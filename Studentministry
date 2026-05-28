<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Студентське Служіння</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400;1,600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
        /* ОСНОВНІ НАЛАШТУВАННЯ */
        * { box-sizing: border-box; margin: 0; padding: 0; }
        
        body { 
            background-color: #E5E5E5; 
            display: flex; 
            flex-direction: column; 
            align-items: center; 
            padding: 60px 0; 
            gap: 60px;
        }

        /* КОНТЕЙНЕР СЛАЙДУ */
        .slide-container {
            width: 1280px;
            height: 720px;
            background-color: #FBF1E7; 
            position: relative;
            display: flex;
            flex-direction: column;
            padding: 60px 80px;
            font-family: 'Inter', sans-serif;
            color: #1A1A1A; 
            overflow: hidden;
            box-shadow: 0 30px 60px rgba(0,0,0,0.1);
        }

        /* ТИПОГРАФІЯ */
        h1, h2, h3, .serif-text { 
            font-family: 'Playfair Display', serif; 
        }
        
        h1 { 
            font-size: 110px; 
            font-weight: 700; 
            line-height: 0.9; 
            text-transform: uppercase;
            letter-spacing: -2px;
            margin-bottom: 20px;
        }
        
        h2.slide-title { 
            font-size: 64px; 
            font-weight: 400; 
            margin-bottom: 50px; 
            line-height: 1.1;
        }
        
        h3 { 
            font-size: 32px; 
            font-weight: 600; 
            margin-bottom: 20px; 
        }

        p { 
            font-size: 18px; 
            line-height: 1.6; 
            font-weight: 300; 
            color: #333;
        }

        .label {
            font-family: 'Inter', sans-serif;
            font-size: 12px;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-weight: 600;
            display: block;
            margin-bottom: 15px;
        }

        .accent-highlight {
            background-color: #E4F946; 
            padding: 0 10px;
            display: inline-block;
        }

        /* ДЕКОРАТИВНІ ЕЛЕМЕНТИ */
        .fine-line {
            width: 100%;
            height: 1px;
            background-color: #1A1A1A;
            margin: 40px 0;
        }

        .content-area { flex-grow: 1; display: flex; flex-direction: column; justify-content: center; }

        /* МАКЕТИ */
        
        /* 1. Title Slide */
        .title-slide { justify-content: space-between; }
        .title-header { display: flex; justify-content: space-between; align-items: flex-start; }
        .title-footer { display: flex; justify-content: space-between; border-top: 1px solid #1A1A1A; padding-top: 20px; }
        .large-italic { font-style: italic; font-weight: 400; text-transform: none; color: #555; }

        /* 2. Split Screen */
        .split-screen {
            display: grid;
            grid-template-columns: 5fr 7fr;
            height: 100%;
            gap: 80px;
            align-items: center;
        }
        .image-box {
            width: 100%;
            height: 500px;
            background-color: #E5E5E5;
            position: relative;
            overflow: hidden;
        }
        .image-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            filter: grayscale(10%) contrast(105%);
        }

        /* 3. Quote Layout */
        .quote-slide { text-align: center; align-items: center; }
        .quote-slide blockquote {
            font-size: 52px;
            line-height: 1.2;
            max-width: 900px;
            margin: 0 auto;
        }
        .quote-slide cite {
            display: block;
            margin-top: 40px;
            font-family: 'Inter', sans-serif;
            font-size: 14px;
            text-transform: uppercase;
            letter-spacing: 3px;
            font-weight: 600;
            font-style: normal;
        }

        /* 4. List Layout */
        .editorial-list {
            list-style: none;
            border-top: 1px solid #1A1A1A;
        }
        .editorial-list li {
            display: grid;
            grid-template-columns: 100px 1fr 2fr;
            border-bottom: 1px solid #1A1A1A;
            padding: 30px 0;
            align-items: start;
        }
        .editorial-list .number {
            font-family: 'Playfair Display', serif;
            font-size: 24px;
            font-style: italic;
        }

        /* 5. Support & Connect Layout */
        .support-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            height: 100%;
            align-items: center;
        }
        
        .support-box {
            border: 1px solid #1A1A1A;
            padding: 50px;
            height: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            transition: 0.3s ease;
        }
        
        .support-box:hover {
            background-color: #1A1A1A;
            color: #FBF1E7;
        }
        
        .support-box:hover p, .support-box:hover .label {
            color: #FBF1E7;
        }
        
        .support-box i {
            font-size: 40px;
            margin-bottom: 30px;
        }

        /* 6. Footer/Contact Slide */
        .contact-slide { justify-content: center; text-align: center; }
        .social-links {
            display: flex;
            justify-content: center;
            gap: 40px;
            margin-top: 50px;
        }
        .social-link {
            font-size: 20px;
            font-family: 'Inter', sans-serif;
            font-weight: 600;
            text-transform: uppercase;
            color: #1A1A1A;
            text-decoration: none;
            border-bottom: 2px solid transparent;
            padding-bottom: 5px;
            transition: 0.3s;
        }
        .social-link:hover {
            border-color: #E4F946;
        }
        
        .huge-background-text {
            position: absolute;
            font-size: 250px;
            font-family: 'Inter', sans-serif;
            font-weight: 800;
            color: rgba(0,0,0,0.03);
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            white-space: nowrap;
            z-index: 0;
            pointer-events: none;
        }
        
        .z-index-1 { position: relative; z-index: 1; }
    </style>
</head>
<body>

<!-- SLIDE 1: TITLE -->
<div class="slide-container title-slide">
    <div class="huge-background-text">MINISTRY</div>
    
    <div class="title-header z-index-1">
        <div>
            <span class="label">Vol. 1 — The Mission</span>
        </div>
        <div>
            <span class="label">UKRAINE / 2024-2026</span>
        </div>
    </div>
    
    <div class="content-area z-index-1" style="justify-content: center;">
        <h1>Student<br><span class="large-italic">Ministry</span></h1>
        <p style="max-width: 400px; margin-top: 20px;">
            <span class="accent-highlight">Разом задля Божого Царства.</span><br>
            Ми маємо велику місію та бачення — бачити, як якомога більше студентів чують про Христа.
        </p>
    </div>
    
    <div class="title-footer z-index-1">
        <span class="label">IRENE & VLAD PATSAMAI</span>
        <span class="label">SCROLL TO DISCOVER</span>
    </div>
</div>

<!-- SLIDE 2: ABOUT US -->
<div class="slide-container">
    <div class="split-screen">
        <div class="image-box">
            <!-- ФОТО З GITHUB №1 -->
            <img src="https://raw.githubusercontent.com/aleksandrkilusik-blip/VladPatsamai/main/IMG_6190.jpeg" alt="Irene & Vlad Patsamai">
        </div>
        <div class="content-area">
            <span class="label">01. Про нас</span>
            <h2 class="slide-title">Щиро вітаємо<br>вас на сторінці.</h2>
            <p style="font-size: 20px; margin-bottom: 20px;">
                Тут ми хочемо ділитися з вами тим, що Бог робить у служінні студентам.
            </p>
            <p>
                Щомісяця ми надсилаємо молитовні листи, в яких розповідаємо про події в служінні та нашому житті. Дякуємо за ваші молитви та спільну працю для Божого Царства!
            </p>
            <div class="fine-line" style="margin-top: 50px;"></div>
            <span class="label">Ірина та Влад Пацамай</span>
        </div>
    </div>
</div>

<!-- SLIDE 3: BOLD QUOTE -->
<div class="slide-container quote-slide" style="justify-content: center; background-color: #1A1A1A; color: #FBF1E7;">
    <div class="content-area">
        <span class="label" style="color: #E4F946;">Святе Письмо</span>
        <blockquote class="serif-text">
            «Також моліться й за нас, щоб Бог відчинив нам двері для проповіді слова, щоб звіщати таємницю Христову...»
        </blockquote>
        <cite style="color: #888;">— Колосянам 4:3</cite>
    </div>
</div>

<!-- SLIDE 4: VISION / LIST -->
<div class="slide-container">
    <div class="content-area">
        <span class="label">02. Наше Бачення</span>
        <h2 class="slide-title">Місія та<br><span class="accent-highlight">Цілі</span></h2>
        
        <ul class="editorial-list">
            <li>
                <div class="number">01</div>
                <h3>Студенти</h3>
                <p>Ми прагнемо, щоб якомога більше молодих людей почули про Христа та отримали можливість змінити своє життя.</p>
            </li>
            <li>
                <div class="number">02</div>
                <h3>Партнерство</h3>
                <p>Ми запрошуємо людей до партнерства — це спільне служіння, де кожен відіграє важливу роль.</p>
            </li>
            <li>
                <div class="number">03</div>
                <h3>Вплив</h3>
                <p>Бачення місії полягає в тому, щоб залучити більше людей до здійснення реального впливу на життя наступного покоління.</p>
            </li>
        </ul>
    </div>
</div>

<!-- SLIDE 5: SPLIT SCREEN (COMMUNITY) -->
<div class="slide-container">
    <div class="split-screen" style="grid-template-columns: 7fr 5fr;">
        <div class="content-area" style="padding-right: 40px;">
            <span class="label">03. Спільнота</span>
            <h2 class="slide-title">Жнива<br><span class="large-italic">великі.</span></h2>
            <p style="font-size: 24px; font-family: 'Playfair Display', serif; font-style: italic; margin-bottom: 20px; line-height: 1.4;">
                «І сказав Він до них: Жнива великі, а робітників мало; отож благайте Господаря жнив, щоб вислав робітників на жниво Своє!»
            </p>
            <span class="label" style="color: #888; margin-bottom: 40px;">— Луки 10:2</span>
            
            <p>Ми хочемо охопити якомога більше студентів. Ваша участь — це інвестиція у вічність та майбутнє цих молодих людей.</p>
        </div>
        <div class="image-box">
             <!-- ФОТО З GITHUB №2 -->
            <img src="https://raw.githubusercontent.com/aleksandrkilusik-blip/VladPatsamai/main/image.png" alt="Студентська конференція">
        </div>
    </div>
</div>

<!-- SLIDE 6: HOW TO HELP / SUPPORT -->
<div class="slide-container">
    <div class="content-area">
        <span class="label">04. Партнерство</span>
        <h2 class="slide-title">Як ви можете<br><span class="accent-highlight">допомогти?</span></h2>
        
        <div class="support-grid">
            <div class="support-box">
                <i class="fa-solid fa-hands-praying"></i>
                <h3 style="font-family: 'Inter', sans-serif; font-size: 24px; margin-bottom: 15px;">Молитовна підтримка</h3>
                <p>Це те, що дає нам сили у важкі часи. Ми мало що можемо зробити самі, але з Божою допомогою — все можливо!</p>
            </div>
            
            <div class="support-box">
                <i class="fa-solid fa-hand-holding-dollar"></i>
                <h3 style="font-family: 'Inter', sans-serif; font-size: 24px; margin-bottom: 15px;">Фінансова підтримка</h3>
                <p>Команда місії повністю довіряє Богу в цьому. Якщо Бог відкриває ваше серце підтримати служіння фінансово, ми будемо вдячні.</p>
            </div>
        </div>
    </div>
</div>

<!-- SLIDE 7: OTHER WAYS TO HELP -->
<div class="slide-container">
    <div class="content-area">
        <span class="label">05. Інші шляхи</span>
        <h2 class="slide-title">Мережа<br><span class="large-italic">Контактів</span></h2>
        
        <p style="font-size: 24px; max-width: 800px; margin-bottom: 30px; line-height: 1.5;">
            Ми хочемо зустріти якомога більше людей, щоб дати їм можливість стати частиною Божої роботи серед студентів.
        </p>
        
        <p style="max-width: 800px; margin-bottom: 40px;">
            Ми впевнені, що у вашій церкві, серед родини, друзів, колег чи знайомих є ті, кому було б цікаво розглянути можливість стати партнерами в такому служінні. Ви можете використовувати список контактів у телефоні, групи в соцмережах або чати.
        </p>
        
        <div class="accent-highlight" style="padding: 20px; font-weight: 500;">
            Дякуємо наперед за ваш час — це неймовірна допомога для нас!
        </div>
    </div>
</div>

<!-- SLIDE 8: CONTACT -->
<div class="slide-container contact-slide">
    <div class="content-area">
        <i class="fa-solid fa-heart" style="font-size: 40px; color: #E4F946; margin-bottom: 30px;"></i>
        <h2 class="slide-title" style="margin-bottom: 20px;">Дякуємо за вашу підтримку,<br>молитви та участь.</h2>
        <p style="font-size: 24px;">Нехай Бог благословить вас та ваші сім'ї!</p>
        
        <div class="fine-line"></div>
        
        <span class="label">Зв'яжіться з нами</span>
        <div class="social-links">
            <a href="#" class="social-link">Instagram</a>
            <a href="#" class="social-link">Facebook</a>
            <a href="#" class="social-link">Telegram</a>
            <a href="#" class="social-link">Email</a>
        </div>
    </div>
</div>

</body>
</html>
