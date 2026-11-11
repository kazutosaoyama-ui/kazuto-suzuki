<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>伊賀白鳳高校陸上部OB ランニングイベント2027</title>
<meta name="description" content="伊賀白鳳高校陸上部23年卒OBによるランニング教室。現役大学ランナーが走りの基本から大会に向けたアドバイスまで直接指導します。">
<meta property="og:title" content="伊賀白鳳高校陸上部OB ランニングイベント2027">
<meta property="og:type" content="website">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@600;700;800&family=Noto+Sans+JP:wght@400;500;700;900&display=swap" rel="stylesheet">
<style>
/* Layout concept: 陸上競技場のトラックとゼッケンをモチーフにした縦長ランディングページ。
   レーンライン区切り / 巨大な英語見出し / ゼッケン型の選手カード / タイムテーブル形式の当日の流れ */
:root {
  --ink: #0e1726;        /* 本文・ダーク面 */
  --ink-soft: #3b4658;
  --track: #e0452c;      /* タータントラックの赤 */
  --track-deep: #b8321c;
  --paper: #f2f4f7;      /* 背景（ごくわずかに青みのあるグレー） */
  --white: #ffffff;
  --line: #dde2ea;
  --mute: #6b7586;

  --toyo: #1e3a8a;
  --komazawa: #9b111e;
  --surugadai: #0284c7;
  --meiji: #5b21b6;

  --font-display: 'Barlow Condensed', 'Noto Sans JP', sans-serif;
  --font-body: 'Noto Sans JP', system-ui, -apple-system, sans-serif;
  --gutter: clamp(18px, 5vw, 48px);
}

* { box-sizing: border-box; }
html { scroll-behavior: smooth; scroll-padding-top: 72px; }
body {
  margin: 0;
  font-family: var(--font-body);
  color: var(--ink);
  background: var(--paper);
  line-height: 1.85;
  letter-spacing: .03em;
  -webkit-font-smoothing: antialiased;
}
img { max-width: 100%; display: block; }
a { color: inherit; }
.wrap { width: 100%; max-width: 1120px; margin: 0 auto; padding-inline: var(--gutter); }

/* ---------- Header ---------- */
.site-header {
  position: fixed; inset: 0 0 auto 0; z-index: 100;
  background: rgba(14, 23, 38, .92);
  backdrop-filter: blur(10px);
  color: #fff;
}
.site-header .wrap { display: flex; align-items: center; justify-content: space-between; height: 64px; gap: 16px; }
.brand { font-family: var(--font-display); font-weight: 700; font-size: 1.05rem; letter-spacing: .12em; text-decoration: none; text-transform: uppercase; white-space: nowrap; }
.brand b { color: var(--track); }
.gnav ul { display: flex; gap: 28px; list-style: none; margin: 0; padding: 0; }
.gnav a { font-family: var(--font-display); font-weight: 600; font-size: .95rem; letter-spacing: .16em; text-decoration: none; color: #c7cfdb; text-transform: uppercase; transition: color .2s; }
.gnav a:hover { color: #fff; }
.menu-btn { display: none; background: none; border: 0; width: 44px; height: 44px; padding: 0; cursor: pointer; position: relative; }
.menu-btn span { position: absolute; left: 10px; right: 10px; height: 2px; background: #fff; transition: transform .25s, opacity .25s; }
.menu-btn span:nth-child(1) { top: 15px; }
.menu-btn span:nth-child(2) { top: 21px; }
.menu-btn span:nth-child(3) { top: 27px; }
.menu-btn[aria-expanded="true"] span:nth-child(1) { transform: translateY(6px) rotate(45deg); }
.menu-btn[aria-expanded="true"] span:nth-child(2) { opacity: 0; }
.menu-btn[aria-expanded="true"] span:nth-child(3) { transform: translateY(-6px) rotate(-45deg); }

/* ---------- Hero ---------- */
.hero { padding-top: 64px; background: var(--ink); color: #fff; position: relative; overflow: hidden; }
.hero-grid { display: grid; grid-template-columns: minmax(0, 5fr) minmax(0, 7fr); min-height: min(78vh, 700px); }
.hero-copy { display: flex; flex-direction: column; justify-content: center; gap: 22px; padding: 56px var(--gutter) 56px max(var(--gutter), calc((100vw - 1120px) / 2 + var(--gutter))); position: relative; z-index: 2; }
.hero-kicker { font-family: var(--font-display); font-weight: 700; letter-spacing: .28em; font-size: .95rem; color: var(--track); text-transform: uppercase; display: flex; align-items: center; gap: 14px; }
.hero-kicker::before { content: ''; width: 44px; height: 3px; background: var(--track); }
.hero h1 { margin: 0; font-weight: 900; font-size: clamp(2rem, 4.2vw, 3.6rem); line-height: 1.22; letter-spacing: .06em; }
.hero h1 em { font-style: normal; display: block; color: var(--track); }
.hero-tagline { margin: 0; font-weight: 700; letter-spacing: .22em; font-size: 1.05rem; color: #dfe5ee; }
.hero-date { display: flex; align-items: flex-end; gap: 14px; margin-top: 6px; }
.hero-date .big { font-family: var(--font-display); font-weight: 800; font-size: clamp(3.4rem, 7vw, 5.6rem); line-height: .9; letter-spacing: .02em; }
.hero-date .big small { font-size: .38em; letter-spacing: .1em; margin-left: .15em; }
.hero-date .meta { font-size: .88rem; line-height: 1.5; color: #c7cfdb; padding-bottom: 6px; }
.hero-date .meta strong { display: block; color: #fff; font-size: 1.05rem; letter-spacing: .12em; }

.hero-visual { position: relative; min-height: 340px; background: #070d18; }
.slide { position: absolute; inset: 0; background-size: cover; background-position: center 30%; opacity: 0; transition: opacity 1.4s ease; }
.slide.active { opacity: 1; }
.hero-visual::after { content: ''; position: absolute; inset: 0; background: linear-gradient(90deg, rgba(14,23,38,.85) 0%, rgba(14,23,38,0) 28%); pointer-events: none; }
.dots { position: absolute; right: 24px; bottom: 22px; display: flex; gap: 8px; z-index: 3; }
.dot { width: 28px; height: 4px; background: rgba(255,255,255,.4); border: 0; padding: 0; cursor: pointer; transition: background .3s; }
.dot.active { background: var(--track); }
.dot:focus-visible, .btn:focus-visible, a:focus-visible, .menu-btn:focus-visible { outline: 3px solid var(--track); outline-offset: 3px; }

/* レーンライン */
.lanes { height: 22px; background: repeating-linear-gradient(180deg, var(--track) 0 3px, transparent 3px 7px); opacity: .9; }

/* ---------- Sections ---------- */
section { padding-block: clamp(64px, 9vw, 110px); }
.sec-head { margin-bottom: clamp(32px, 5vw, 56px); position: relative; }
.sec-en { display: block; font-family: var(--font-display); font-weight: 800; text-transform: uppercase; font-size: clamp(3rem, 9vw, 6.4rem); line-height: .9; letter-spacing: .04em; color: transparent; -webkit-text-stroke: 1.5px rgba(14,23,38,.22); }
.sec-ja { display: inline-flex; align-items: center; gap: 12px; margin: -14px 0 0 4px; font-weight: 900; font-size: clamp(1.25rem, 2.6vw, 1.7rem); letter-spacing: .1em; position: relative; }
.sec-ja::before { content: ''; width: 28px; height: 4px; background: var(--track); }
.dark .sec-en { -webkit-text-stroke-color: rgba(255,255,255,.28); }

.lead { max-width: 46em; font-size: 1.02rem; color: var(--ink-soft); margin: 0 0 36px; }

/* Info strip */
.facts { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 0; margin: -44px 0 0; position: relative; z-index: 5; background: var(--white); box-shadow: 0 18px 40px rgba(14,23,38,.12); }
.fact { padding: 26px 28px; border-right: 1px solid var(--line); }
.fact:last-child { border-right: 0; }
.fact .k { font-family: var(--font-display); font-weight: 700; letter-spacing: .24em; font-size: .85rem; color: var(--track); text-transform: uppercase; }
.fact .v { font-weight: 900; font-size: 1.25rem; line-height: 1.5; margin-top: 4px; }
.fact .v small { display: block; font-weight: 500; font-size: .85rem; color: var(--mute); }

/* News */
.news-list { list-style: none; margin: 0; padding: 0; border-top: 2px solid var(--ink); }
.news-list li { display: grid; grid-template-columns: 130px 1fr; gap: 18px; padding: 20px 4px; border-bottom: 1px solid var(--line); align-items: baseline; }
.news-list time { font-family: var(--font-display); font-weight: 700; font-size: 1.05rem; letter-spacing: .1em; color: var(--mute); }
.news-list p { margin: 0; font-weight: 500; }

/* Points */
.points { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 24px; }
.point { background: var(--white); padding: 34px 28px 30px; position: relative; border-top: 5px solid var(--track); }
.point .tag { font-family: var(--font-display); font-weight: 800; letter-spacing: .2em; font-size: .85rem; color: var(--track); }
.point h3 { margin: 6px 0 12px; font-size: 1.2rem; font-weight: 900; line-height: 1.5; letter-spacing: .06em; }
.point p { margin: 0; font-size: .93rem; color: var(--ink-soft); }

/* Definition tables */
.spec { border-top: 2px solid var(--ink); margin: 0; }
.spec .row { display: grid; grid-template-columns: 200px 1fr; gap: 20px; padding: 20px 4px; border-bottom: 1px solid var(--line); }
.spec dt { font-weight: 900; letter-spacing: .1em; }
.spec dd { margin: 0; min-width: 0; overflow-wrap: anywhere; }
.spec a { color: var(--track-deep); font-weight: 700; }
.note { font-size: .82rem; color: var(--mute); margin-top: 18px; }

/* Schedule: タイムテーブル */
.dark { background: var(--ink); color: #fff; }
.timetable { list-style: none; margin: 0; padding: 0; border-top: 2px solid var(--track); }
.timetable li { display: grid; grid-template-columns: minmax(130px, 200px) 1fr; gap: 22px; align-items: center; padding: 24px 6px; border-bottom: 1px solid rgba(255,255,255,.14); }
.timetable .t { font-family: var(--font-display); font-weight: 800; font-size: clamp(1.9rem, 4vw, 2.8rem); line-height: 1; letter-spacing: .04em; }
.timetable .t small { font-size: .5em; color: var(--track); margin-left: 2px; letter-spacing: .1em; }
.timetable .d { font-weight: 700; font-size: 1.02rem; }
.timetable .d span { display: block; font-weight: 400; font-size: .85rem; color: #aab4c4; margin-top: 2px; }
.timetable li.hl .d { color: #fff; }
.timetable li.hl .t { color: var(--track); }

/* Organizer */
.org-grid { display: grid; grid-template-columns: minmax(0, 360px) minmax(0, 1fr); gap: clamp(28px, 5vw, 64px); align-items: center; }
.org-photo { position: relative; }
.org-photo img { width: 100%; aspect-ratio: 4 / 5; object-fit: cover; object-position: top; background: #cfd5df; }
.org-photo::after { content: ''; position: absolute; inset: 14px -14px -14px 14px; border: 3px solid var(--track); z-index: -1; }
.org-body .univ { font-weight: 700; color: var(--track-deep); letter-spacing: .1em; }
.org-body h3 { font-size: clamp(1.7rem, 3.6vw, 2.4rem); font-weight: 900; margin: 4px 0 2px; letter-spacing: .08em; line-height: 1.3; }
.org-body .yomi { color: var(--mute); font-size: .9rem; letter-spacing: .12em; margin-bottom: 18px; }
.org-body p { margin: 0; color: var(--ink-soft); }

/* Athletes: ゼッケン型カード */
.athletes { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 28px; }
.bib { --c: var(--ink); background: var(--white); display: flex; flex-direction: column; transition: transform .3s, box-shadow .3s; box-shadow: 0 6px 20px rgba(14,23,38,.06); }
.bib:hover { transform: translateY(-5px); box-shadow: 0 18px 36px rgba(14,23,38,.12); }
.bib.toyo { --c: var(--toyo); } .bib.komazawa { --c: var(--komazawa); } .bib.surugadai { --c: var(--surugadai); } .bib.meiji { --c: var(--meiji); }
.bib-top { background: var(--c); color: #fff; padding: 18px 26px 16px; display: flex; justify-content: space-between; align-items: flex-end; gap: 12px; }
.bib-top .uni-en { font-family: var(--font-display); font-weight: 800; font-size: 2.2rem; line-height: 1; letter-spacing: .12em; text-transform: uppercase; }
.bib-top .grade { font-weight: 700; font-size: .85rem; letter-spacing: .1em; text-align: right; line-height: 1.5; opacity: .95; }
.bib-name { padding: 22px 26px 6px; }
.bib-name h3 { margin: 0; font-size: 1.5rem; font-weight: 900; letter-spacing: .08em; line-height: 1.4; }
.bib-name .yomi { font-size: .82rem; color: var(--mute); letter-spacing: .12em; }
.bib-name .uni-ja { font-weight: 700; color: var(--c); font-size: .92rem; margin-top: 6px; }
.pb { margin: 14px 26px 0; display: grid; grid-template-columns: repeat(auto-fit, minmax(110px, 1fr)); border: 1px solid var(--line); }
.pb div { padding: 12px 14px; border-right: 1px solid var(--line); min-width: 0; }
.pb div:last-child { border-right: 0; }
.pb dt { font-family: var(--font-display); font-weight: 700; letter-spacing: .16em; font-size: .78rem; color: var(--mute); text-transform: uppercase; }
.pb dd { margin: 0; font-family: var(--font-display); font-weight: 700; font-size: 1.28rem; letter-spacing: .04em; line-height: 1.35; color: var(--ink); overflow-wrap: anywhere; }
.pb dd.jp { font-family: var(--font-body); font-size: .92rem; font-weight: 700; }
.bib-ach { padding: 22px 26px 28px; }
.bib-ach h4 { margin: 0 0 12px; font-size: .82rem; font-weight: 900; letter-spacing: .18em; color: var(--c); text-transform: uppercase; }
.bib-ach ul { margin: 0; padding: 0; list-style: none; display: grid; gap: 14px; }
.bib-ach li { padding-left: 16px; position: relative; font-size: .9rem; color: var(--ink-soft); line-height: 1.75; }
.bib-ach li::before { content: ''; position: absolute; left: 0; top: .75em; width: 7px; height: 3px; background: var(--c); }
.race { display: inline-block; font-weight: 900; font-size: .78rem; letter-spacing: .06em; background: var(--paper); color: var(--ink); padding: 1px 9px; margin-right: 6px; }
.res { font-weight: 700; color: var(--ink); }

/* Entry */
.entry { background: var(--track); color: #fff; text-align: center; position: relative; overflow: hidden; }
.entry .sec-en { -webkit-text-stroke-color: rgba(255,255,255,.4); }
.entry .sec-ja::before { background: #fff; }
.entry .sec-head { display: flex; flex-direction: column; align-items: center; }
.entry p { max-width: 36em; margin: 0 auto 34px; font-weight: 500; }
.btn { display: inline-flex; align-items: center; gap: 14px; background: #fff; color: var(--track-deep); font-weight: 900; font-size: 1.15rem; letter-spacing: .1em; padding: 22px 54px; text-decoration: none; transition: transform .2s, box-shadow .2s, background .2s, color .2s; box-shadow: 0 14px 30px rgba(0,0,0,.2); }
.btn::after { content: '→'; font-family: var(--font-display); font-size: 1.5rem; transition: transform .2s; }
.btn:hover { transform: translateY(-3px); background: var(--ink); color: #fff; }
.btn:hover::after { transform: translateX(4px); }

/* Contact */
.contact-card { background: var(--white); padding: clamp(26px, 4vw, 44px); border-left: 6px solid var(--track); }
.contact-card .spec { border-top: 0; }
.contact-card .spec .row:last-child { border-bottom: 0; }

/* Footer */
footer { background: #080e1a; color: #8b96a8; padding: 40px var(--gutter) 100px; text-align: center; font-size: .82rem; letter-spacing: .08em; }
footer .brand { display: inline-block; color: #fff; margin-bottom: 10px; }

/* Floating entry */
.float-entry { position: fixed; right: 18px; bottom: 18px; z-index: 90; background: var(--track); color: #fff; text-decoration: none; font-family: var(--font-display); font-weight: 800; letter-spacing: .22em; font-size: 1.05rem; padding: 14px 26px; box-shadow: 0 10px 24px rgba(0,0,0,.28); transition: background .2s, transform .2s; }
.float-entry:hover { background: var(--track-deep); transform: translateY(-2px); }

/* Reveal（JSが動いた場合のみ） */
.js .reveal { opacity: 0; transform: translateY(22px); transition: opacity .7s ease, transform .7s ease; }
.js .reveal.in { opacity: 1; transform: none; }

/* ---------- Responsive ---------- */
@media (max-width: 900px) {
  .hero-grid { grid-template-columns: 1fr; min-height: 0; }
  .hero-visual { order: -1; min-height: 0; aspect-ratio: 4 / 3; }
  .hero-visual::after { background: linear-gradient(0deg, rgba(14,23,38,.7) 0%, rgba(14,23,38,0) 35%); }
  .hero-copy { padding: 40px var(--gutter) 70px; }
  .facts { grid-template-columns: 1fr; margin-top: -28px; }
  .fact { border-right: 0; border-bottom: 1px solid var(--line); padding: 20px 22px; }
  .fact:last-child { border-bottom: 0; }
  .points { grid-template-columns: 1fr; }
  .athletes { grid-template-columns: 1fr; }
  .org-grid { grid-template-columns: 1fr; }
  .org-photo { max-width: 320px; margin-right: 14px; }
}
@media (max-width: 820px) {
  .menu-btn { display: block; }
  .gnav { position: fixed; inset: 64px 0 auto 0; background: var(--ink); padding: 10px var(--gutter) 26px; transform: translateY(-120%); transition: transform .3s ease; border-bottom: 3px solid var(--track); }
  .gnav.open { transform: none; }
  .gnav ul { flex-direction: column; gap: 0; }
  .gnav a { display: block; padding: 16px 0; border-bottom: 1px solid rgba(255,255,255,.12); font-size: 1.1rem; }
}
@media (max-width: 560px) {
  .brand { font-size: .9rem; letter-spacing: .06em; }
  .news-list li { grid-template-columns: 1fr; gap: 2px; }
  .spec .row { grid-template-columns: 1fr; gap: 4px; }
  .timetable li { grid-template-columns: 1fr; gap: 6px; }
  .btn { padding: 18px 30px; font-size: 1.02rem; width: 100%; justify-content: center; }
  .float-entry { right: 12px; bottom: 12px; padding: 12px 20px; }
}
@media (prefers-reduced-motion: reduce) {
  html { scroll-behavior: auto; }
  .slide, .js .reveal, .bib, .btn { transition: none; }
}
</style>
</head>
<body>

<!-- Header -->
<header class="site-header">
  <div class="wrap">
    <a class="brand" href="#top">Iga Hakuho <b>OB</b> Running</a>
    <button class="menu-btn" id="menuBtn" aria-label="メニューを開く" aria-expanded="false" aria-controls="gnav"><span></span><span></span><span></span></button>
    <nav class="gnav" id="gnav" aria-label="メインメニュー">
      <ul>
        <li><a href="#news">News</a></li>
        <li><a href="#about">Info</a></li>
        <li><a href="#schedule">Schedule</a></li>
        <li><a href="#athletes">Athletes</a></li>
        <li><a href="#organizer">Organizer</a></li>
        <li><a href="#entry">Entry</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </div>
</header>

<main id="top">

<!-- Hero -->
<div class="hero">
  <div class="hero-grid">
    <div class="hero-copy">
      <div class="hero-kicker">Iga Hakuho High School Track &amp; Field OB</div>
      <h1>伊賀白鳳高校陸上部OB<em>ランニングイベント2027</em></h1>
      <p class="hero-tagline">すべては感動のために</p>
      <div class="hero-date">
        <div class="big">3.7<small>SAT</small></div>
        <div class="meta"><strong>2027年3月7日（土）</strong>9:00 – 12:00 ／ 受付 8:30〜<br>三重県内 陸上競技場</div>
      </div>
    </div>
    <div class="hero-visual" id="slider" aria-label="イベントの写真">
      <div class="slide active" style="background-image:url('https://github.com/user-attachments/assets/bd058cdc-9978-4ec1-afab-8caebe05635c')"></div>
      <div class="slide" style="background-image:url('https://github.com/user-attachments/assets/6b486f94-cb59-4365-bced-ab18cbd034c6')"></div>
      <div class="slide" style="background-image:url('https://github.com/user-attachments/assets/06540e3d-c217-4e20-88fc-b14f46b5483c')"></div>
      <div class="slide" style="background-image:url('https://github.com/user-attachments/assets/f8d02b5f-be84-48ac-a684-87f5b850df4a')"></div>
      <div class="dots">
        <button class="dot active" aria-label="1枚目を表示"></button>
        <button class="dot" aria-label="2枚目を表示"></button>
        <button class="dot" aria-label="3枚目を表示"></button>
        <button class="dot" aria-label="4枚目を表示"></button>
      </div>
    </div>
  </div>
  <div class="lanes" aria-hidden="true"></div>
</div>

<!-- Key facts -->
<div class="wrap">
  <div class="facts reveal">
    <div class="fact"><div class="k">Date</div><div class="v">3月7日(土)<small>9:00〜12:00（受付 8:30〜）</small></div></div>
    <div class="fact"><div class="k">Place</div><div class="v">三重県内 陸上競技場<small>詳細な場所が入ります</small></div></div>
    <div class="fact"><div class="k">Entry fee</div><div class="v">無料（または〇〇円）<small>小・中学生、高校生、市民ランナー</small></div></div>
  </div>
</div>

<!-- News -->
<section id="news">
  <div class="wrap">
    <div class="sec-head reveal"><span class="sec-en">News</span><span class="sec-ja">新着情報</span></div>
    <ul class="news-list reveal">
      <li><time datetime="2026-11-11">2026.11.11</time><p>ランニングイベント2027の特設ページを公開しました。</p></li>
      <li><time datetime="2026-11-11">2026.11.XX</time><p>参加者の募集を開始します。お申し込みは下記「Entry」から。（日付と内容は差し替えてください）</p></li>
    </ul>
  </div>
</section>

<!-- Points -->
<section id="about" style="padding-top:0">
  <div class="wrap">
    <div class="sec-head reveal"><span class="sec-en">Event Info</span><span class="sec-ja">イベントについて</span></div>
    <p class="lead reveal">地元三重県への恩返しと次世代ランナーの育成を目的に、伊賀白鳳高校陸上部23年卒OBによるランニング教室を開催いたします。走りの基本から大会に向けたアドバイスまで、現役大学生ランナーが直接指導します。</p>

    <div class="points">
      <article class="point reveal"><div class="tag">POINT 01</div><h3>走りの基本から、動き作りまで</h3><p>ウォーミングアップと動き作りの指導から始め、フォームを現役の大学ランナーが一人ひとり見ていきます。</p></article>
      <article class="point reveal"><div class="tag">POINT 02</div><h3>レベル別のランニングセッション</h3><p>初めての方も、大会を目指す方も。レベルに合わせたセッションで、それぞれの課題に取り組みます。</p></article>
      <article class="point reveal"><div class="tag">POINT 03</div><h3>OB選手と一緒に走る</h3><p>箱根駅伝や三大駅伝を走った選手たちと、同じ時間に同じトラックを走るスペシャルセッションがあります。</p></article>
    </div>

    <dl class="spec reveal" style="margin-top:56px">
      <div class="row"><dt>イベント名</dt><dd>伊賀白鳳高校陸上部OB ランニングイベント2027</dd></div>
      <div class="row"><dt>日時</dt><dd>3月7日(土) 9:00〜12:00（受付開始 8:30〜）</dd></div>
      <div class="row"><dt>会場</dt><dd>三重県内 陸上競技場（詳細な場所が入ります）</dd></div>
      <div class="row"><dt>対象</dt><dd>小・中学生、高校生、市民ランナーの皆様</dd></div>
      <div class="row"><dt>持ち物</dt><dd>走れる服装、ランニングシューズ、飲み物、タオル</dd></div>
      <div class="row"><dt>参加費</dt><dd>無料（または〇〇円）</dd></div>
    </dl>
  </div>
</section>

<!-- Schedule -->
<section id="schedule" class="dark">
  <div class="wrap">
    <div class="sec-head reveal"><span class="sec-en">Schedule</span><span class="sec-ja">イベント当日の流れ</span></div>
    <ol class="timetable reveal">
      <li><div class="t">08:30<small>〜</small></div><div class="d">受付開始</div></li>
      <li><div class="t">09:00<small>〜</small></div><div class="d">開会式・ウォーミングアップ・動き作り指導</div></li>
      <li><div class="t">09:45<small>〜</small></div><div class="d">レベル別ランニングセッション / フォーム指導</div></li>
      <li class="hl"><div class="t">11:00<small>〜</small></div><div class="d">OB選手と一緒に走るスペシャルセッション</div></li>
      <li><div class="t">11:30<small>〜</small></div><div class="d">質問コーナー・写真撮影・閉会式</div></li>
    </ol>
  </div>
</section>

<!-- Athletes -->
<section id="athletes">
  <div class="wrap">
    <div class="sec-head reveal"><span class="sec-en">Athletes</span><span class="sec-ja">参加OB選手紹介</span></div>
    <p class="lead reveal">伊賀白鳳高校23年卒のメンバーが集結します。現役の大学陸上界で活躍する選手たちから、直接アドバイスを受けることができます。</p>

    <div class="athletes">

      <article class="bib toyo reveal">
        <div class="bib-top"><div class="uni-en">Toyo</div><div class="grade">総合情報学部<br>3年</div></div>
        <div class="bib-name"><h3>倉本 晃羽</h3><div class="yomi">くらもと あきは</div><div class="uni-ja">東洋大学</div></div>
        <dl class="pb">
          <div><dt>5000m</dt><dd>14:09.26</dd></div>
          <div><dt>10000m</dt><dd>29:24.55</dd></div>
          <div><dt>Half</dt><dd>1:02:57</dd></div>
        </dl>
        <div class="bib-ach">
          <h4>Highlights</h4>
          <ul>
            <li>東洋大学の主力選手層の一角として、長距離部門で頭角を現しチームの上位層を支える。</li>
            <li><span class="race">第58回 全日本大学駅伝</span><span class="res">6区（12.8km）38分14秒（区間11位）</span><br>長距離区間の6区で粘りの走りを見せ、安定したペースを刻む。</li>
          </ul>
        </div>
      </article>

      <article class="bib komazawa reveal">
        <div class="bib-top"><div class="uni-en">Komazawa</div><div class="grade">経営学部<br>3年</div></div>
        <div class="bib-name"><h3>島子 公佑</h3><div class="yomi">しまこ こうすけ</div><div class="uni-ja">駒澤大学</div></div>
        <dl class="pb">
          <div><dt>5000m</dt><dd>13:29.78</dd></div>
          <div><dt>10000m</dt><dd class="jp">28分台<br>（東海大記録会等）</dd></div>
        </dl>
        <div class="bib-ach">
          <h4>Highlights</h4>
          <ul>
            <li>高校時代は三重県高校駅伝4区で区間賞を獲得。</li>
            <li><span class="race">第36回 出雲駅伝</span><span class="res">5区（6.4km）18分25秒（区間2位）</span><br>三大駅伝初出走で2位をキープし、総合準優勝に大きく貢献。</li>
            <li><span class="race">第56回 全日本大学駅伝</span><span class="res">1区（9.5km）28分25秒（区間14位／首位差7秒）</span><br>地元三重県を通る1区を担当し、ラスト200mの混戦で集団に食らいつく力走。</li>
          </ul>
        </div>
      </article>

      <article class="bib surugadai reveal">
        <div class="bib-top"><div class="uni-en">Surugadai</div><div class="grade">スポーツ科学部<br>4年</div></div>
        <div class="bib-name"><h3>古橋 希翁</h3><div class="yomi">ふるはし まれお</div><div class="uni-ja">駿河台大学</div></div>
        <dl class="pb">
          <div><dt>5000m</dt><dd>13:51.03</dd></div>
          <div><dt>10000m</dt><dd>28:19.45</dd></div>
          <div><dt>Half</dt><dd>1:02:13</dd></div>
        </dl>
        <div class="bib-ach">
          <h4>Highlights</h4>
          <ul>
            <li>駿河台大学のエース格としてチームを牽引。第102回箱根駅伝では関東学生連合チームの2区を担当。</li>
            <li><span class="race">第103回 箱根駅伝予選会</span><span class="res">ハーフマラソン 1時間02分40秒（個人17位／日本人上位）</span><br>チーム内2番手として予選会上位でフィニッシュ。</li>
            <li><span class="race">第100回 箱根駅伝 本大会</span><span class="res">3区（21.4km）1時間04分11秒（区間18位）</span></li>
          </ul>
        </div>
      </article>

      <article class="bib meiji reveal">
        <div class="bib-top"><div class="uni-en">Meiji</div><div class="grade">経営学部<br>4年</div></div>
        <div class="bib-name"><h3>小林 周太郎</h3><div class="yomi">こばやし しゅうたろう</div><div class="uni-ja">明治大学</div></div>
        <dl class="pb">
          <div><dt>5000m</dt><dd>14:20.72</dd></div>
          <div><dt>10000m</dt><dd>31:32.91</dd></div>
          <div><dt>Half</dt><dd>1:04:30</dd></div>
        </dl>
        <div class="bib-ach">
          <h4>Highlights</h4>
          <ul>
            <li>明治大学競走部で4年間主軸としてチームをリード。上尾シティハーフ等でも自己ベストを更新する勝負強さを発揮。</li>
            <li><span class="race">関東インカレ 男子1部 3000m障害</span><span class="res">予選 8分55秒70（2着・決勝進出）/ 決勝 8分54秒06（11位）</span><br>タフなレースで1部残留に向け貢献。</li>
          </ul>
        </div>
      </article>

    </div>
  </div>
</section>

<!-- Organizer -->
<section id="organizer" style="padding-top:0">
  <div class="wrap">
    <div class="sec-head reveal"><span class="sec-en">Organizer</span><span class="sec-ja">主催者紹介</span></div>
    <div class="org-grid reveal">
      <div class="org-photo"><img src="https://github.com/user-attachments/assets/c37e14f4-1a98-4d36-8695-bf669c77403d" alt="鈴木千翔"></div>
      <div class="org-body">
        <div class="univ">青山学院大学 陸上競技部</div>
        <h3>鈴木 千翔</h3>
        <div class="yomi">すずき かずと</div>
        <p>伊賀白鳳高校 23年卒。地元三重県の皆様と一緒に走れることを楽しみにしています。</p>
      </div>
    </div>
  </div>
</section>

<!-- Entry -->
<section id="entry" class="entry">
  <div class="wrap">
    <div class="sec-head reveal"><span class="sec-en">Entry</span><span class="sec-ja">参加者応募</span></div>
    <p class="reveal">イベントへのご参加は、下記のフォームからお申し込みください。定員に達し次第、締め切ります。</p>
    <a class="btn reveal" href="https://forms.google.com/" target="_blank" rel="noopener">参加申し込みフォーム</a>
  </div>
</section>

<!-- Contact -->
<section id="contact">
  <div class="wrap">
    <div class="sec-head reveal"><span class="sec-en">Contact</span><span class="sec-ja">大会運営元・お問い合わせ</span></div>
    <p class="lead reveal">イベントに関するご質問、取材のお申し込み、協賛についてのお問い合わせは、運営事務局までご連絡ください。</p>
    <div class="contact-card reveal">
      <dl class="spec">
        <div class="row"><dt>運営団体</dt><dd>伊賀白鳳高校陸上部23年卒OB ランニングイベント実行委員会</dd></div>
        <div class="row"><dt>代表責任者</dt><dd>鈴木 千翔（青山学院大学 陸上競技部）</dd></div>
        <div class="row"><dt>所在地・活動拠点</dt><dd>三重県伊賀市</dd></div>
        <div class="row"><dt>メールアドレス</dt><dd><a href="mailto:example@email.com">example@email.com</a></dd></div>
        <div class="row"><dt>電話番号</dt><dd>090-XXXX-XXXX</dd></div>
      </dl>
    </div>
  </div>
</section>

</main>

<footer>
  <a class="brand" href="#top">Iga Hakuho <b>OB</b> Running</a>
  <p>&copy; 2027 23年卒 伊賀白鳳高校陸上部OB ランニングイベント実行委員会</p>
</footer>

<a class="float-entry" href="#entry">ENTRY</a>

<script>
document.documentElement.classList.add('js');

/* スライダー（15秒ごとに切り替え） */
(function () {
  var slides = document.querySelectorAll('.slide');
  var dots = document.querySelectorAll('.dot');
  var current = 0, timer;
  function show(i) {
    slides[current].classList.remove('active');
    dots[current].classList.remove('active');
    current = i;
    slides[current].classList.add('active');
    dots[current].classList.add('active');
  }
  function start() { clearInterval(timer); timer = setInterval(function () { show((current + 1) % slides.length); }, 15000); }
  dots.forEach(function (d, i) { d.addEventListener('click', function () { show(i); start(); }); });
  start();
})();

/* モバイルメニュー */
(function () {
  var btn = document.getElementById('menuBtn');
  var nav = document.getElementById('gnav');
  function set(open) {
    nav.classList.toggle('open', open);
    btn.setAttribute('aria-expanded', open ? 'true' : 'false');
    btn.setAttribute('aria-label', open ? 'メニューを閉じる' : 'メニューを開く');
  }
  btn.addEventListener('click', function () { set(!nav.classList.contains('open')); });
  nav.querySelectorAll('a').forEach(function (a) { a.addEventListener('click', function () { set(false); }); });
})();

/* スクロール時のフェードイン */
(function () {
  var els = document.querySelectorAll('.reveal');
  if (!('IntersectionObserver' in window)) { els.forEach(function (e) { e.classList.add('in'); }); return; }
  var io = new IntersectionObserver(function (entries) {
    entries.forEach(function (en) { if (en.isIntersecting) { en.target.classList.add('in'); io.unobserve(en.target); } });
  }, { threshold: 0.12, rootMargin: '0px 0px -40px 0px' });
  els.forEach(function (e) { io.observe(e); });
})();
</script>
</body>
</html>
