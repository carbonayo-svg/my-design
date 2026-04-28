# my-design
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>個人簡歷 | Professional Portfolio</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --bg-color: #f8f9fa;
            --text-main: #2d3436;
            --accent-color: #0984e3;
            --secondary-color: #636e72;
            --section-bg: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "PingFang TC", "Microsoft JhengHei", sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.8;
        }

        header {
            height: 60vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background: #2d3436;
            color: white;
            text-align: center;
            padding: 20px;
        }

        header h1 {
            font-size: 3rem;
            letter-spacing: 5px;
            margin-bottom: 10px;
            font-weight: 300;
        }

        header p {
            font-size: 1.1rem;
            opacity: 0.8;
            letter-spacing: 2px;
        }

        nav {
            position: sticky;
            top: 0;
            background: rgba(255, 255, 255, 0.95);
            padding: 15px 0;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
            z-index: 1000;
        }

        nav a {
            margin: 0 20px;
            text-decoration: none;
            color: var(--text-main);
            font-weight: 500;
            font-size: 0.9rem;
            transition: 0.3s;
        }

        nav a:hover {
            color: var(--accent-color);
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 60px 20px;
        }

        section {
            margin-bottom: 80px;
        }

        .section-title {
            font-size: 1.8rem;
            border-left: 4px solid var(--text-main);
            padding-left: 15px;
            margin-bottom: 30px;
            font-weight: 600;
        }

        .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .card {
            background: var(--section-bg);
            padding: 30px;
            border-radius: 4px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.02);
            transition: transform 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card h3 {
            margin-bottom: 15px;
            color: var(--accent-color);
            font-size: 1.2rem;
        }

        .card ul {
            list-style: none;
        }

        .card ul li {
            margin-bottom: 8px;
            font-size: 0.95rem;
            color: var(--secondary-color);
        }

        .card ul li::before {
            content: "•";
            margin-right: 8px;
            color: var(--accent-color);
        }

        .highlight-box {
            background: #dfe6e9;
            padding: 40px;
            border-radius: 8px;
            margin-top: 40px;
        }

        .timeline-item {
            border-bottom: 1px solid #ddd;
            padding: 15px 0;
        }

        footer {
            background: #2d3436;
            color: white;
            text-align: center;
            padding: 40px 0;
            font-size: 0.8rem;
            letter-spacing: 1px;
        }

        /* 針對筆記中的特殊重點優化 */
        .ai-section {
            background: #f1f2f6;
            padding: 20px;
            border-radius: 4px;
            border-left: 4px solid #ff7675;
        }

        @media (max-width: 600px) {
            header h1 { font-size: 2rem; }
            nav a { margin: 0 10px; font-size: 0.8rem; }
        }
    </style>
</head>
<body>

    <header>
        <h1>PERSONAL RESUME</h1>
        <p>設計 · 數位技術 · 多元實踐</p>
    </header>

    <nav>
        <a href="#about">自傳</a>
        <a href="#design">專業設計</a>
        <a href="#digital">數位學習</a>
        <a href="#tech">數位技術</a>
        <a href="#extra">多元經歷</a>
    </nav>

    <div class="container">
        
        <section id="about">
            <h2 class="section-title">關於我 / 自傳</h2>
            <div class="card">
                <p>致力於在設計與技術之間找到平衡，不僅是解決問題，更是在服務中尋找意義。面對AI時代的挑戰，我擁抱變革，並持續在跨領域中學習與成長。</p>
                <div style="margin-top: 20px;">
                    <strong>核心理念：</strong>
                    <ul>
                        <li>服務的意義：透過設計創造價值</li>
                        <li>對數位領域的想法：持續演進與突破</li>
                        <li>我想成為的人：合作、默契、專業的貢獻者</li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="design">
            <h2 class="section-title">設計專業 (Design)</h2>
            <div class="grid-container">
                <div class="card">
                    <h3>學習歷程</h3>
                    <ul>
                        <li>設計動機與核心理念</li>
                        <li>修課記錄與個人努力</li>
                        <li>修課計劃大表</li>
                    </ul>
                </div>
                <div class="card">
                    <h3>專業實踐</h3>
                    <ul>
                        <li>歷年設計專案作品</li>
                        <li>未來規劃 (身障十年計畫+設計APP)</li>
                        <li>設計方向的長遠規劃</li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="digital">
            <h2 class="section-title">數位學習 (Digital Learning)</h2>
            <div class="card">
                <div class="grid-container" style="display: flex; flex-wrap: wrap;">
                    <div style="flex: 1; min-width: 250px;">
                        <ul>
                            <li>數位學習動機探討</li>
                            <li>數位學習相關專案研究</li>
                            <li>修課記錄與未來規劃</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <section id="tech">
            <h2 class="section-title">數位技術 (Digital Technology)</h2>
            <div class="grid-container">
                <div class="card">
                    <h3>技術開發</h3>
                    <ul>
                        <li>數位技術研究動機</li>
                        <li>實作專案歷程</li>
                        <li>技術修課與自我提升</li>
                    </ul>
                </div>
                <div class="card ai-section">
                    <h3>面對 AI 的挑戰</h3>
                    <ul>
                        <li>面對 AI 的適應與思考</li>
                        <li>做題的嘗試 (各種 AI 工具運用)</li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="extra">
            <h2 class="section-title">多元表現</h2>
            <div class="highlight-box">
                <div class="grid-container">
                    <div>
                        <h3>影音與美學</h3>
                        <ul>
                            <li>金穗、金馬影展參與</li>
                            <li>東華電影節經歷</li>
                            <li>對動態影片的思考</li>
                        </ul>
                    </div>
                    <div>
                        <h3>科學與人文</h3>
                        <ul>
                            <li>科學背景跨界應用</li>
                            <li>閱讀與寫作深度積累</li>
                            <li>劇場實作、身心障礙者權益關注</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <section>
            <h2 class="section-title">最後心得</h2>
            <blockquote style="font-style: italic; color: #636e72; border-left: 2px solid #ccc; padding-left: 20px;">
                在合作中建立默契，在服務中感受意義。
            </blockquote>
        </section>

    </div>

    <footer>
        <p>© 2024 PORTFOLIO. All Rights Reserved.</p>
    </footer>

</body>
</html>
