<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>伊賀白鳳高校陸上部OB ランニングイベント2027</title>
    <style>
        /* 全体の基本設定 */
        :root {
            --primary-color: #0f172a;
            --accent-color: #f59e0b;
            --bg-color: #f8fafc;
            --text-color: #334155;
            --white: #ffffff;
        }

        html {
            scroll-behavior: smooth; /* タブをクリックした時に滑らかにスクロール */
        }

        body {
            font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            line-height: 1.7;
            margin: 0;
            padding: 0;
            color: var(--text-color);
            background-color: var(--bg-color);
        }

        /* ヘッダー・ナビゲーション（上部固定メニュー） */
        header {
            background-color: var(--primary-color);
            color: var(--white);
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
        }
        .header-container {
            max-width: 1100px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 12px 20px;
            flex-wrap: wrap;
        }
        .header-title {
            font-size: 1rem;
            font-weight: bold;
            letter-spacing: 0.05em;
            margin: 0;
        }
        nav ul {
            display: flex;
            list-style: none;
            padding: 0;
            margin: 0;
            gap: 15px;
            flex-wrap: wrap;
        }
        nav a {
            color: #cbd5e1;
            text-decoration: none;
            font-size: 0.9rem;
            font-weight: 500;
            transition: color 0.3s;
        }
        nav a:hover {
            color: var(--white);
            border-bottom: 2px solid var(--accent-color);
        }

        /* メインビジュアル（15秒自動スライダー） */
        .hero-slider {
            position: relative;
            width: 100%;
            height: 60vh;
            min-height: 420px;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: #0f172a;
        }

        .slide {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-size: contain;
            background-position: center;
            background-repeat: no-repeat;
            opacity: 0;
            transition: opacity 1.5s ease-in-out;
            z-index: 1;
        }
        .slide.active {
            opacity: 1;
        }

        .hero-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(15, 23, 42, 0.45);
            z-index: 2;
        }

        .hero-content {
            position: relative;
            z-index: 3;
            text-align: center;
            padding: 0 20px;
            max-width: 900px;
        }

        .hero-content h1 {
            font-size: 2.5rem;
            margin-bottom: 15px;
            font-weight: 900;
            letter-spacing: 0.05em;
            background: linear-gradient(45deg, #ffffff, #fde047, #f97316, #ffffff);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: shineText 5s ease infinite;
            text-shadow: 0 2px 10px rgba(0,0,0,0.5);
        }

        @keyframes shineText {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .hero-content p {
            font-size: 1.4rem;
            color: #fde047;
            font-weight: bold;
            letter-spacing: 0.1em;
            text-shadow: 0 2px 5px rgba(0,0,0,0.8);
            margin-top: 0;
        }

        .slider-dots {
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: 10px;
            z-index: 4;
        }
        .dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background-color: rgba(255, 255, 255, 0.5);
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
        }
        .dot.active {
            background-color: var(--accent-color);
            transform: scale(1.2);
        }

        /* 各セクション共通 */
        section {
            max-width: 900px;
            margin: 50px auto;
            padding: 40px 30px;
            background: var(--white);
            border-radius: 12px;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.05);
        }
        h2 {
            color: var(--primary-color);
            font-size: 1.6rem;
            border-left: 5px solid var(--accent-color);
            padding-left: 15px;
            margin-top: 0;
            margin-bottom: 25px;
        }

        /* テーブル設定（イベント概要・連絡先情報用） */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }
        table th, table td {
            border-bottom: 1px solid #e2e8f0;
            padding: 16px;
            text-align: left;
        }
        table th {
            background-color: #f1f5f9;
            color: var(--primary-color);
            width: 28%;
            font-weight: 600;
        }

        /* タイムスケジュール */
        .timeline {
            list-style: none;
            padding: 0;
        }
        .timeline li {
            padding: 14px 0;
            border-bottom: 1px dashed #cbd5e1;
            display: flex;
            align-items: center;
        }
        .timeline .time {
            font-weight: bold;
            width: 120px;
            color: var(--accent-color);
            font-size: 1.05rem;
        }

        /* 主催者カード */
        .organizer-container {
            display: flex;
            justify-content: center;
        }
        .organizer-card {
            max-width: 350px;
            width: 100%;
            border: 1px solid #e2e8f0;
            border-radius: 12px;
            overflow: hidden;
            background: var(--white);
            box-shadow: 0 4px 12px rgba(0,0,0,0.05);
            text-align: center;
        }
        .organizer-card img {
            width: 100%;
            height: 280px;
            object-fit: cover;
            object-position: top;
        }

        /* カードグリッド（OB選手用） */
        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 25px;
            margin-top: 25px;
        }
        .card {
            border: 1px solid #e2e8f0;
            border-radius: 8px;
            overflow: hidden;
            background: var(--white);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.08);
        }
        .card img {
            width: 100%;
            height: 220px;
            object-fit: cover;
        }
        .card-content {
            padding: 20px;
        }
        .card-content h3 {
            margin: 0 0 8px 0;
            color: var(--primary-color);
            font-size: 1.15rem;
        }
        .card-content p {
            margin: 6px 0;
            font-size: 0.95rem;
        }

        /* 連絡先エリア（お問い合わせリンク） */
        .contact-mail {
            color: var(--accent-color);
            font-weight: bold;
            text-decoration: none;
        }
        .contact-mail:hover {
            text-decoration: underline;
        }

        /* 応募ボタン */
        .btn-apply {
            display: inline-block;
            background-color: var(--accent-color);
            color: var(--primary-color);
            padding: 18px 50px;
            font-size: 1.25rem;
            font-weight: 900;
            text-decoration: none;
            border-radius: 50px;
            transition: background 0.3s, transform 0.2s;
            box-shadow: 0 4px 15px rgba(245, 158, 11, 0.4);
        }
        .btn-apply:hover {
            background-color: #d97706;
            transform: scale(1.03);
            color: var(--white);
        }
        .apply-container {
            text-align: center;
            padding: 10px;
        }

        /* フッター */
        footer {
            text-align: center;
            padding: 30px;
            background-color: var(--primary-color);
            color: #94a3b8;
            margin-top: 80px;
            font-size: 0.85rem;
        }

        /* スマホ対応 */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                text-align: center;
                gap: 10px;
            }
            nav ul {
                justify-content: center;
                gap: 8px;
            }
            nav a {
                font-size: 0.85rem;
                padding: 4px 6px;
            }
            .hero-slider {
                height: 50vh;
                min-height: 350px;
            }
            .hero-content h1 {
                font-size: 1.6rem;
            }
            .hero-content p {
                font-size: 1.05rem;
            }
            section {
                margin: 20px 10px;
                padding: 25px 15px;
            }
            table th {
                width: 35%;
            }
        }
    </style>
</head>
<body>

    <!-- ヘッダー（上部固定ナビゲーションタブ） -->
    <header>
        <div class="header-container">
            <p class="header-title">伊賀白鳳高校 23年卒OB ランニングイベント</p>
            <nav>
                <ul>
                    <li><a href="#about">イベント情報</a></li>
                    <li><a href="#contact">運営元連絡先</a></li>
                    <li><a href="#organizer">主催者</a></li>
                    <li><a href="#schedule">当日の流れ</a></li>
                    <li><a href="#athletes">参加OB選手</a></li>
                    <li><a href="#apply">お申し込み</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- メインビジュアル（15秒自動切り替えスライダー） -->
    <div class="hero-slider">
        <div class="slide active" style="background-image: url('https://github.com/user-attachments/assets/bd058cdc-9978-4ec1-afab-8caebe05635c');"></div>
        <div class="slide" style="background-image: url('https://github.com/user-attachments/assets/6b486f94-cb59-4365-bced-ab18cbd034c6');"></div>
        <div class="slide" style="background-image: url('https://github.com/user-attachments/assets/06540e3d-c217-4e20-88fc-b14f46b5483c');"></div>
        <div class="slide" style="background-image: url('https://github.com/user-attachments/assets/f8d02b5f-be84-48ac-a684-87f5b850df4a');"></div>
        
        <div class="hero-overlay"></div>

        <div class="hero-content">
            <h1>伊賀白鳳高校陸上部OB ランニングイベント2027</h1>
            <p>すべては感動のために</p>
        </div>

        <div class="slider-dots">
            <span class="dot active" onclick="setSlide(0)"></span>
            <span class="dot" onclick="setSlide(1)"></span>
            <span class="dot" onclick="setSlide(2)"></span>
            <span class="dot" onclick="setSlide(3)"></span>
        </div>
    </div>

    <!-- 1. イベント情報 (最初のメインセクション) -->
    <section id="about">
        <h2>ランニングイベント情報</h2>
        <p>地元三重県への恩返しと次世代ランナーの育成を目的に、伊賀白鳳高校陸上部23年卒OBによるランニング教室を開催いたします。走りの基本から大会に向けたアドバイスまで、現役大学生ランナーが直接指導します！</p>
        <table>
            <tr>
                <th>イベント名</th>
                <td>伊賀白鳳高校陸上部OB ランニングイベント2027</td>
            </tr>
            <tr>
                <th>日時</th>
                <td>3月7日(土) 9:00〜12:00（受付開始 8:30〜）</td>
            </tr>
            <tr>
                <th>会場</th>
                <td>三重県内 陸上競技場（詳細な場所が入ります）</td>
            </tr>
            <tr>
                <th>対象</th>
                <td>小・中学生、高校生、市民ランナーの皆様</td>
            </tr>
            <tr>
                <th>持ち物</th>
                <td>走れる服装、ランニングシューズ、飲み物、タオル</td>
            </tr>
            <tr>
                <th>参加費</th>
                <td>無料（または〇〇円）</td>
            </tr>
        </table>
    </section>

    <!-- 2. 大会運営元・連絡先情報 -->
    <section id="contact">
        <h2>大会運営元・お問い合わせ</h2>
        <p>イベントに関する質問、取材のお申し込み、協賛についてのお問い合わせは下記運営事務局までご連絡ください。</p>
        <table>
            <tr>
                <th>運営団体</th>
                <td>伊賀白鳳高校陸上部23年卒OB ランニングイベント実行委員会</td>
            </tr>
            <tr>
                <th>代表責任者</th>
                <td>鈴木 千翔（青山学院大学 陸上競技部）</td>
            </tr>
            <tr>
                <th>所在地・活動拠点</th>
                <td>三重県伊賀市（またはご指定の住所・地域）</td>
            </tr>
            <tr>
                <th>メールアドレス</th>
                <td><a href="mailto:example@email.com" class="contact-mail">example@email.com</a>（※ご指定のアドレスに変更してください）</td>
            </tr>
            <tr>
                <th>電話番号</th>
                <td>090-XXXX-XXXX（※必要な場合のみ記入）</td>
            </tr>
        </table>
    </section>

    <!-- 3. 主催者紹介 -->
    <section id="organizer">
        <h2>主催者紹介</h2>
        <div class="organizer-container">
            <div class="organizer-card">
                <img src="https://github.com/user-attachments/assets/c37e14f4-1a98-4d36-8695-bf669c77403d" alt="鈴木千翔">
                <div class="card-content">
                    <h3>鈴木 千翔（すずき かずと）</h3>
                    <p><strong>青山学院大学 陸上競技部</strong></p>
                    <p>伊賀白鳳高校 23年卒。地元三重県の皆様と一緒に走れることを楽しみにしています！</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 4. 当日の流れ -->
    <section id="schedule">
        <h2>イベント当日の流れ</h2>
        <ul class="timeline">
            <li>
                <span class="time">08:30〜</span>
                <span>受付開始</span>
            </li>
            <li>
                <span class="time">09:00〜</span>
                <span>開会式・ウォーミングアップ・動き作り指導</span>
            </li>
            <li>
                <span class="time">09:45〜</span>
                <span>レベル別ランニングセッション / フォーム指導</span>
            </li>
            <li>
                <span class="time">11:00〜</span>
                <span>OB選手と一緒に走るスペシャルセッション</span>
            </li>
            <li>
                <span class="time">11:30〜</span>
                <span>質問コーナー・写真撮影・閉会式</span>
            </li>
        </ul>
    </section>

    <!-- 5. 参加OB選手紹介 -->
    <section id="athletes">
        <h2>参加OB選手紹介</h2>
        <p>伊賀白鳳高校23年卒の豪華メンバーが集結します！</p>
        <div class="card-grid">
            <div class="card">
                <img src="IMG_9443.jpg" alt="OB選手1">
                <div class="card-content">
                    <h3>選手のお名前 A</h3>
                    <p><strong>〇〇大学 陸上競技部</strong></p>
                    <p>自己ベスト：5000m 〇分〇秒</p>
                </div>
            </div>
            <div class="card">
                <img src="IMG_9439.jpg" alt="OB選手2">
                <div class="card-content">
                    <h3>選手のお名前 B</h3>
                    <p><strong>〇〇大学 陸上競技部</strong></p>
                    <p>自己ベスト：10000m 〇分〇秒</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 6. 参加者応募 -->
    <section id="apply">
        <h2>参加者応募</h2>
        <div class="apply-container">
            <p>イベントへのご参加はこちらのフォームよりお申し込みください。（定員に達し次第締め切ります）</p>
            <a href="https://forms.google.com/" target="_blank" class="btn-apply">参加申し込みフォームはこちら</a>
        </div>
    </section>

    <footer>
        <p>&copy; 2027 23年卒 伊賀白鳳高校陸上部OB ランニングイベント実行委員会</p>
    </footer>

    <!-- スライダー切替用JavaScript -->
    <script>
        let currentSlide = 0;
        const slides = document.querySelectorAll('.slide');
        const dots = document.querySelectorAll('.dot');
        const intervalTime = 15000;
        let slideInterval;

        function showSlide(index) {
            slides.forEach((slide, i) => {
                slide.classList.remove('active');
                dots[i].classList.remove('active');
            });
            slides[index].classList.add('active');
            dots[index].classList.add('active');
            currentSlide = index;
        }

        function nextSlide() {
            let next = (currentSlide + 1) % slides.length;
            showSlide(next);
        }

        function setSlide(index) {
            showSlide(index);
            resetTimer();
        }

        function resetTimer() {
            clearInterval(slideInterval);
            slideInterval = setInterval(nextSlide, intervalTime);
        }

        slideInterval = setInterval(nextSlide, intervalTime);
    </script>
</body>
</html>
