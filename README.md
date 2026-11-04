# kazuto-suzuki
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <青山学院大学>鈴木千翔_伊賀白鳳OBランニング教室公式HP<青山学院大学>
</head>
<body>
    <h1>こんにちは！ホームページへようこそ</h1>
    <p>これは私がはじめて作ったホームページです。</p>
</body>
</html>
<!DOCTYPE html>

<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>鈴木千翔 & 伊賀白鳳高校陸上部23年卒OB ランニング教室</title>
    <style>
        /* 全体の基本設定 */
        body {
            font-family: "Helvetica Neue", Arial, "平角ゴシック ProN", "Hiragino Kaku Gothic ProN", "メイリオ", Meiryo, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            color: #333;
            background-color: #f8f9fa;
        }

        /* ヘッダー・ナビゲーション（タブ） */
        header {
            background-color: #004d40; /* 陸上・スポーツに合う深みのあるグリーン */
            color: #fff;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .header-title {
            text-align: center;
            padding: 15px 10px 5px;
            font-size: 1.2rem;
            margin: 0;
        }
        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
            padding: 10px 0;
            margin: 0;
            flex-wrap: wrap;
            background-color: #00352c;
        }
        nav li {
            margin: 5px 10px;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            font-weight: bold;
            padding: 6px 12px;
            border-radius: 4px;
            transition: background 0.3s;
        }
        nav a:hover {
            background-color: #00796b;
        }

        /* メインビジュアル */
        .hero {
            background: linear-gradient(rgba(0, 77, 64, 0.7), rgba(0, 77, 64, 0.7)), url('IMG_9645.jpg') center/cover no-repeat;
            color: white;
            text-align: center;
            padding: 60px 20px;
        }
        .hero h1 {
            font-size: 2rem;
            margin-bottom: 10px;
        }
        .hero p {
            font-size: 1.2rem;
        }

        /* 各セクション共通 */
        section {
            max-width: 900px;
            margin: 40px auto;
            padding: 30px 20px;
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.05);
        }
        h2 {
            color: #004d40;
            border-bottom: 3px solid #00796b;
            padding-bottom: 8px;
            margin-top: 0;
        }

        /* テーブルスタイル（イベント概要用） */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
        }
        table th, table td {
            border-bottom: 1px solid #ddd;
            padding: 12px;
            text-align: left;
        }
        table th {
            background-color: #e0f2f1;
            width: 30%;
        }

        /* タイムスケジュール */
        .timeline {
            list-style: none;
            padding: 0;
        }
        .timeline li {
            padding: 10px 0;
            border-bottom: 1px dashed #ccc;
            display: flex;
        }
        .timeline .time {
            font-weight: bold;
            width: 100px;
            color: #00796b;
        }

        /* 選手・主催者カード */
        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        .card {
            border: 1px solid #e0e0e0;
            border-radius: 8px;
            overflow: hidden;
            text-align: center;
            background: #fafafa;
        }
        .card img {
            width: 100%;
            height: 220px;
            object-fit: cover;
        }
        .card-content {
            padding: 15px;
        }
        .card-content h3 {
            margin: 5px 0;
            color: #004d40;
        }

        /* 応募ボタン */
        .btn-apply {
            display: inline-block;
            background-color: #e65100;
            color: #fff;
            padding: 15px 40px;
            font-size: 1.2rem;
            font-weight: bold;
            text-decoration: none;
            border-radius: 30px;
            transition: background 0.3s;
            margin-top: 15px;
        }
        .btn-apply:hover {
            background-color: #ff6d00;
        }
        .apply-container {
            text-align: center;
            padding: 20px;
        }

        /* フッター */
        footer {
            text-align: center;
            padding: 20px;
            background-color: #004d40;
            color: #fff;
            margin-top: 50px;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <!-- ヘッダー（ナビゲーションタブ） -->
    <header>
        <div class="header-title">青山学院大学 鈴木千翔 & 伊賀白鳳OB ランニング教室</div>
        <nav>
            <ul>
                <li><a href="#about">イベント概要</a></li>
                <li><a href="#organizer">主催者紹介</a></li>
                <li><a href="#schedule">当日の流れ</a></li>
                <li><a href="#athletes">参加OB選手</a></li>
                <li><a href="#apply">参加応募</a></li>
            </ul>
        </nav>
    </header>

    <!-- メインビジュアル -->
    <div class="hero">
        <h1>23年卒 伊賀白鳳高校陸上部OB<br>ランニングイベント in 三重</h1>
        <p>開催日：3月7日(土)</p>
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
                <!-- 実際の写真ファイル名に置き換えてください -->
                <img src="IMG_9645.jpg" alt="鈴木千翔">
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

    <!-- 5. 参加者応募 -->
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
