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

    <section id="athletes">
        <h2>参加OB選手紹介</h2>
        <p>伊賀白鳳高校23年卒の豪華メンバーが集結します！</p>
        <div class="card-grid">
            <div class="card">
                <img src="IMG_9443.jpg" alt="OB選手1">
                <div class="card-content">
                    <h3>選手のお名前 A</h3>
                    <p>〇〇大学 陸上競技部</p>
                    <p>自己ベスト：5000m 〇分〇秒</p>
                </div>
            </div>
            <div class="card">
                <img src="IMG_9439.jpg" alt="OB選手2">
                <div class="card-content">
                    <h3>選手のお名前 B</h3>
                    <p>〇〇大学 陸上競技部</p>
                    <p>自己ベスト：10000m 〇分〇秒</p>
                </div>
            </div>
        </div>
    </section>

    <section id="apply">
        <h2>参加者応募</h2>
        <div class="apply-container">
            <p>イベントへのご参加はこちらのフォームよりお申し込みください。（定員に達し次第締め切ります）</p>
            <!-- Googleフォームなどのリンクを href="" に設置します -->
            <a href="https://forms.google.com/" target="_blank" class="btn-apply">参加申し込みフォームはこちら</a>
        </div>
    </section>

    <footer>
        <p>&copy; 23年卒 伊賀白鳳高校陸上部OB ランニングイベント実行委員会</p>
    </footer>

</body>
</html>

<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>鈴木千翔 & 伊賀白鳳高校陸上部23年卒OB ランニング教室 公式HP</title>
    <style>
        /* 全体の基本設定・コーポレート風リセット */
        :root {
            --primary-color: #0f172a; /* 高級感のあるダークネイビー */
            --accent-color: #d97706;  /* 引き締まるゴールド・オレンジ */
            --bg-color: #f8fafc;      /* 上品なライトグレー */
            --text-color: #334155;    /* 読みやすいダークグレー */
            --white: #ffffff;
        }

        body {
            font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            line-height: 1.7;
            margin: 0;
            padding: 0;
            color: var(--text-color);
            background-color: var(--bg-color);
        }

        /* ヘッダー・ナビゲーション（固定型） */
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

        /* メインビジュアル（FV） */
        .hero {
            background: linear-gradient(rgba(15, 23, 42, 0.8), rgba(15, 23, 42, 0.8)), url('https://github.com/user-attachments/assets/c37e14f4-1a98-4d36-8695-bf669c77403d') center/cover no-repeat;
            color: var(--white);
            text-align: center;
            padding: 100px 20px;
        }
        .hero h1 {
            font-size: 2.2rem;
            margin-bottom: 15px;
            letter-spacing: 0.05em;
        }
        .hero p {
            font-size: 1.2rem;
            color: #94a3b8;
            font-weight: 300;
        }

        /* 各セクション共通 */
        section {
            max-width: 900px;
            margin: 60px auto;
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

        /* イベント概要（テーブル） */
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
            width: 25%;
            font-weight: 600;
            border-radius: 4px 0 0 4px;
        }

        /* タイムスケジュール（タイムライン風） */
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

        /* 選手・主催者カードグリッド */
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
            height: 240px;
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

        /* 応募ボタン（CTAセクション） */
        .btn-apply {
            display: inline-block;
            background-color: var(--accent-color);
            color: var(--white);
            padding: 16px 45px;
            font-size: 1.15rem;
            font-weight: bold;
            text-decoration: none;
            border-radius: 50px;
            transition: background 0.3s, transform 0.2s;
            box-shadow: 0 4px 10px rgba(217, 119, 6, 0.3);
        }
        .btn-apply:hover {
            background-color: #b45309;
            transform: scale(1.02);
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

        /* レスポンシブ対応 */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                text-align: center;
                gap: 10px;
            }
            nav ul {
                justify-content: center;
            }
            .hero h1 {
                font-size: 1.7rem;
            }
            section {
                margin: 20px 10px;
                padding: 25px 15px;
            }
        }
    </style>
</head>
<body>

    <!-- ヘッダー（ナビゲーション） -->
    <header>
        <div class="header-container">
            <p class="header-title">伊賀白鳳高校 23年卒OB ランニングイベント</p>
            <nav>
                <ul>
                    <li><a href="#about">概要</a></li>
                    <li><a href="#organizer">主催者</a></li>
                    <li><a href="#schedule">スケジュール</a></li>
                    <li><a href="#athletes">OB選手</a></li>
                    <li><a href="#apply">お申し込み</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- メインビジュアル -->
    <div class="hero">
        <h1>次世代ランナーへ、魂の継承を。</h1>
        <p>2026年3月7日(土) ＠地元・三重県</p>
    </div>

    <!-- 1. イベント概要 -->
    <section id="about">
        <h2>イベント概要</h2>
        <p>地元三重県への恩返しと、次世代ランナーの育成を目的に、伊賀白鳳高校陸上部23年卒OBによるランニング教室を開催いたします。走りの基本から大会に向けたアドバイスまで、現役大学生ランナーが直接指導します！</p>
        <table>
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

    <!-- 2. 主催者紹介 -->
    <section id="organizer">
        <h2>主催者紹介</h2>
        <div class="card-grid">
            <div class="card">
                <img src="https://github.com/user-attachments/assets/c37e14f4-1a98-4d36-8695-bf669c77403d" alt="鈴木千翔">
                <div class="card-content">
                    <h3>鈴木 千翔（すずき かずと）</h3>
                    <p><strong>青山学院大学 陸上競技部</strong></p>
                    <p>伊賀白鳳高校 23年卒。地元三重県の皆様と一緒に走れることを楽しみにしています！</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 3. イベント当日の流れ -->
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

    <!-- 4. 参加OB選手紹介 -->
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

    <!-- 5. 参加者応募 -->
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

</body>
</html>

<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>鈴木千翔 & 伊賀白鳳高校陸上部23年卒OB ランニング教室 公式HP</title>
    <style>
        /* 全体の基本設定 */
        :root {
            --primary-color: #0f172a; /* 高級感のあるダークネイビー */
            --accent-color: #d97706;  /* アクセントカラー（ゴールド・オレンジ） */
            --bg-color: #f8fafc;      /* 背景のライトグレー */
            --text-color: #334155;    /* 本文の文字色 */
            --white: #ffffff;
        }

        body {
            font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            line-height: 1.7;
            margin: 0;
            padding: 0;
            color: var(--text-color);
            background-color: var(--bg-color);
        }

        /* ヘッダー・ナビゲーション */
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

        /* メインビジュアル（FV）- 添付いただいた集合写真に変更 */
        .hero {
            background: linear-gradient(rgba(15, 23, 42, 0.65), rgba(15, 23, 42, 0.65)), url('IMG_0979.jpg') center/cover no-repeat;
            color: var(--white);
            text-align: center;
            padding: 110px 20px;
        }
        .hero h1 {
            font-size: 2.2rem;
            margin-bottom: 15px;
            letter-spacing: 0.05em;
            text-shadow: 0 2px 4px rgba(0,0,0,0.5);
        }
        .hero p {
            font-size: 1.2rem;
            color: #f1f5f9;
            font-weight: 500;
            text-shadow: 0 1px 3px rgba(0,0,0,0.5);
        }

        /* 各セクション共通 */
        section {
            max-width: 900px;
            margin: 60px auto;
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

        /* イベント概要（テーブル） */
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
            width: 25%;
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

        /* 選手・主催者カードグリッド */
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
            height: 250px;
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

        /* 応募ボタン（CTAセクション） */
        .btn-apply {
            display: inline-block;
            background-color: var(--accent-color);
            color: var(--white);
            padding: 16px 45px;
            font-size: 1.15rem;
            font-weight: bold;
            text-decoration: none;
            border-radius: 50px;
            transition: background 0.3s, transform 0.2s;
            box-shadow: 0 4px 10px rgba(217, 119, 6, 0.3);
        }
        .btn-apply:hover {
            background-color: #b45309;
            transform: scale(1.02);
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

        /* レスポンシブ対応（スマホ表示） */
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
            .hero {
                padding: 70px 15px;
            }
            .hero h1 {
                font-size: 1.6rem;
            }
            section {
                margin: 20px 10px;
                padding: 25px 15px;
            }
            table th {
                width: 30%;
            }
        }
    </style>
</head>
<body>

    <!-- ヘッダー（ナビゲーション） -->
    <header>
        <div class="header-container">
            <p class="header-title">伊賀白鳳高校 23年卒OB ランニングイベント</p>
            <nav>
                <ul>
                    <li><a href="#about">概要</a></li>
                    <li><a href="#organizer">主催者</a></li>
                    <li><a href="#schedule">スケジュール</a></li>
                    <li><a href="#athletes">OB選手</a></li>
                    <li><a href="#apply">お申し込み</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- メインビジュアル（最上部） -->
    <div class="hero">
        <h1>次世代ランナーへ、魂の継承を。</h1>
        <p>2026年3月7日(土) ＠地元・三重県</p>
    </div>

    <!-- 1. イベント概要 -->
    <section id="about">
        <h2>イベント概要</h2>
        <p>地元三重県への恩返しと、次世代ランナーの育成を目的に、伊賀白鳳高校陸上部23年卒OBによるランニング教室を開催いたします。走りの基本から大会に向けたアドバイスまで、現役大学生ランナーが直接指導します！</p>
        <table>
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

    <!-- 2. 主催者紹介 -->
    <section id="organizer">
        <h2>主催者紹介</h2>
        <div class="card-grid">
            <div class="card">
                <img src="https://github.com/user-attachments/assets/c37e14f4-1a98-4d36-8695-bf669c77403d" alt="鈴木千翔">
                <div class="card-content">
                    <h3>鈴木 千翔（すずき かずと）</h3>
                    <p><strong>青山学院大学 陸上競技部</strong></p>
                    <p>伊賀白鳳高校 23年卒。地元三重県の皆様と一緒に走れることを楽しみにしています！</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 3. イベント当日の流れ -->
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

    <!-- 4. 参加OB選手紹介 -->
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

    <!-- 5. 参加者応募 -->
    <section id="apply">
        <h2>参加者応募</h2>
        <div class="apply-container">
            <p>イベントへのご参加はこちらのフォームよりお申し込みください。（定員に達し次第締め切ります）</p>
            <a href="https://forms.google.com/" target="_blank" class="btn-apply">参加申し込みフォームはこちら</a>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 23年卒 伊賀白鳳高校陸上部OB ランニングイベント実行委員会</p>
    </footer>

</body>
</html>
