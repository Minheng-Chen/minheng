<!DOCTYPE html>
<html lang="zh-Hant">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>中強光電智慧補貨閉環系統 SRCL-Lite v2</title>
    <style>
        /* 主色調：深藍、銀色 */
        :root {
            --primary-color: #001f3f;
            --accent-color: #C0C0C0;
            --text-color: #333;
            --bg-light: #f9f9f9;
        }
        html {
            scroll-behavior: smooth;
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: "Microsoft JhengHei", sans-serif;
            color: var(--text-color);
            background-color: var(--bg-light);
            line-height: 1.6;
        }
        header {
            background-color: var(--primary-color);
            color: #fff;
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        header nav {
            display: flex;
            align-items: center;
            justify-content: space-between;
        }
        header nav .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }
        header nav ul {
            list-style: none;
            display: flex;
            gap: 1rem;
        }
        header nav ul li a {
            color: #fff;
            text-decoration: none;
            padding: 0.5rem;
            transition: background 0.3s;
        }
        header nav ul li a:hover {
            background-color: var(--accent-color);
            color: var(--primary-color);
            border-radius: 4px;
        }
        section {
            padding: 4rem 2rem;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
        }
        h2 {
            font-size: 2rem;
            color: var(--primary-color);
            margin-bottom: 1rem;
            position: relative;
        }
        h2::after {
            content: "";
            display: block;
            width: 50px;
            height: 4px;
            background-color: var(--accent-color);
            margin-top: 0.5rem;
        }
        p {
            margin-bottom: 1rem;
        }
        /* 響應式網格 */
        .grid {
            display: grid;
            gap: 2rem;
        }
        @media (min-width: 768px) {
            .grid-2 {
                grid-template-columns: 1fr 1fr;
            }
            .grid-3 {
                grid-template-columns: repeat(3, 1fr);
            }
        }
        /* 卡片樣式 */
        .card {
            background-color: #fff;
            border: 1px solid var(--accent-color);
            border-radius: 8px;
            padding: 1.5rem;
            box-shadow: 0 2px 6px rgba(0,0,0,0.1);
            opacity: 0;
            transform: translateY(20px);
            animation: fadeInUp 0.8s forwards paused;
        }
        .card:nth-child(1) { animation-delay: 0.2s; }
        .card:nth-child(2) { animation-delay: 0.4s; }
        .card:nth-child(3) { animation-delay: 0.6s; }
        .card:nth-child(4) { animation-delay: 0.8s; }
        .card:nth-child(5) { animation-delay: 1s; }
        @keyframes fadeInUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        /* 圖片與文字排版 */
        .image-text {
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }
        .image-text img {
            width: 100%;
            border-radius: 8px;
        }
        @media (min-width: 768px) {
            .image-text {
                flex-direction: row;
            }
            .image-text .text {
                flex: 1;
            }
            .image-text .img-wrapper {
                flex: 1;
            }
        }
        /* Footer */
        footer {
            background-color: var(--primary-color);
            color: #fff;
            text-align: center;
            padding: 2rem 1rem;
        }
        footer a {
            color: var(--accent-color);
            text-decoration: none;
        }
    </style>
</head>
<body>
    <header>
        <nav class="container">
            <div class="logo">中強光電 SRCL-Lite v2</div>
            <ul>
                <li><a href="#overview">概覽</a></li>
                <li><a href="#mems">MEMS 感測</a></li>
                <li><a href="#ai">AI 決策</a></li>
                <li><a href="#logistics">智慧物流</a></li>
                <li><a href="#automation">自動搬運</a></li>
                <li><a href="#ar">AR 校正</a></li>
                <li><a href="#cases">國際案例</a></li>
                <li><a href="#analysis">台灣現況</a></li>
                <li><a href="#scenarios">應用場景</a></li>
                <li><a href="#advantage">整合優勢</a></li>
            </ul>
        </nav>
    </header>
    
    <!-- 概覽 -->
    <section id="overview" class="container">
        <h2>網站整體設計理念</h2>
        <p>本網站以「智慧補貨閉環系統 SRCL-Lite v2」為主軸，採用現代專業的設計風格，以深藍色與銀色為主色調，突顯科技感。網站採用響應式設計，確保在桌面與行動裝置皆能提供良好瀏覽體驗。整體架構分為九大核心區塊，並透過平滑滾動與動態效果，增強使用者體驗。</p>
    </section>

    <!-- MEMS 智能感測 -->
    <section id="mems" class="container">
        <h2>MEMS 智能感測技術</h2>
        <div class="grid grid-2">
            <div class="card">
                <h3>CMC 中光電智能感測</h3>
                <p>壓阻式差壓感測器技術規格：±5 kPa 超低壓力範圍，誤差僅 ±1% F.S。應用於貨架重量變化、振動狀態與環境參數之即時監測。</p>
            </div>
            <div class="card">
                <h3>Jupiter 工業振動監測</h3>
                <p>整合加速度計、氣壓計、壓感傳感器等產品，用於工業環境中的振動與壓力監測，確保設備穩定運行。</p>
            </div>
        </div>
    </section>

    <!-- AI 決策 平台 -->
    <section id="ai" class="container" style="background-color: #fff;">
        <h2>AI 決策平台技術</h2>
        <div class="grid grid-2">
            <div class="card">
                <h3>CiCS 智能雲服</h3>
                <p>採用邊緣 AI 與 LSTM 神經網路進行庫存需求預測，成功導入特力屋、屈臣氏等知名通路。實現智慧零售平台、智能數位系統與智慧媒合平台之開發成果。</p>
            </div>
            <div class="card">
                <h3>案例展示</h3>
                <p>已於多家零售商進行試點，庫存缺貨率降低 25%、存貨週轉率提升 30%。</p>
            </div>
        </div>
    </section>

    <!-- 智慧物流 調度 -->
    <section id="logistics" class="container">
        <h2>智慧物流調度技術</h2>
        <div class="grid grid-2">
            <div class="card">
                <h3>CiLS 智能物流</h3>
                <p>Smart Move 升級計畫，採用 3D 視覺感知套件與動態路徑優化演算法，符合 ISO 3691-4 安全標準。具備即時可視、高效控管、高度整合、客製化服務。</p>
            </div>
            <div class="card">
                <h3>WMS 系統整合</h3>
                <p>無縫串接倉儲管理系統，提供庫存即時更新與動態調度。</p>
            </div>
        </div>
    </section>

    <!-- 自動搬運 執行 -->
    <section id="automation" class="container" style="background-color: #fff;">
        <h2>自動搬運執行技術</h2>
        <div class="grid grid-2">
            <div class="card">
                <h3>CIRC 智能機器人</h3>
                <p>提供 AMR 與商用無人機完整解決方案，符合 AMRA-201 及 CNS 15556 安全標準。整合電腦視覺、AI、高速運算與控制等技術。</p>
            </div>
            <div class="card">
                <h3>技術規格</h3>
                <p>機器人搬運重量可達 500 kg，最高速度 1.5 m/s，定位精度 ±2 cm。</p>
            </div>
        </div>
    </section>

    <!-- AR 視覺 校正 -->
    <section id="ar" class="container">
        <h2>AR 視覺校正技術</h2>
        <div class="grid grid-2">
            <div class="card">
                <h3>CRI 創境</h3>
                <p>基於 Snapdragon XR2 Gen 1 平台之 AR/MR 眼鏡 Turnkey 解決方案，具備 6DoF 空間運算、環境感知、AI 手勢識別等功能，與高通合作進行邊緣運算與生成式 AI 技術整合。</p>
            </div>
            <div class="card">
                <h3>AR 校正場景</h3>
                <p>結合現場環境掃描，進行貨架上架位置校正與操作指引，提高補貨準確度與效率。</p>
            </div>
        </div>
    </section>

    <!-- 國際成功案例 -->
    <section id="cases" class="container" style="background-color: #fff;">
        <h2>豐富的國際成功案例</h2>
        <div class="grid grid-3">
            <div class="card">
                <h3>日本全家便利商店</h3>
                <p>Telexistence TX SCARA 補貨機器人於 300 間門市部署，補貨成功率 98%以上，每日處理超過 1000 瓶飲料，使用 NVIDIA Jetson 邊緣 AI 技術。</p>
            </div>
            <div class="card">
                <h3>新加坡新零售 AMR 系統</h3>
                <p>AMR 拣選系統減少人員走動 40%，降低錯誤率 30%，從訂單下發到配送全自動化流程。</p>
            </div>
            <div class="card">
                <h3>台灣 PChome 智慧物流園區</h3>
                <p>林口 A7 園區四萬五千坪，部署數百台 AMR，搬運貨架可達 1000 kg，揀貨效率提升三倍，每日處理量提升一倍以上，峰值處理 20 萬筆訂單。</p>
            </div>
            <div class="card">
                <h3>ASUS IoT 智慧補貨解決方案</h3>
                <p>與 Macnica DHW 合作，AI 圖像識別與深度學習演算法應用於無條碼商品補貨，即時庫存監測、自動提醒與精確視覺判斷。</p>
            </div>
        </div>
    </section>

    <!-- 台灣零售業 現況與痛點 分析 -->
    <section id="analysis" class="container">
        <h2>台灣零售業現況與痛點分析</h2>
        <div class="grid grid-2">
            <div class="card">
                <h3>缺工問題</h3>
                <p>2024 年勞動部統計顯示，批發零售業占總缺工數 13.6%，總缺工數約 6.6 萬人，其中服務業缺工占 53%。</p>
            </div>
            <div class="card">
                <h3>人力成本壓力</h3>
                <p>主流零售業者調薪 7-10%，中高齡員工比例從 10 位員工中 1 位提升至 5 位中有 1 位，成本持續攀升。</p>
            </div>
            <div class="card">
                <h3>傳統補貨限制</h3>
                <p>人工補貨勞動密集度高、大型商品搬運困難、高錯誤率、無法 24 小時運行、薪資成本持續上升。</p>
            </div>
        </div>
    </section>

    <!-- 應用場景 與實施展望 -->
    <section id="scenarios" class="container" style="background-color: #fff;">
        <h2>應用場景與實施展望</h2>
        <div class="grid grid-2">
            <div class="card">
                <h3>全聯超市情境</h3>
                <p>颱風期間需 24 小時加班，緊急調配人力。五段閉環系統可自動化補貨，降低缺貨率、減少人力依賴，提升服務品質。</p>
            </div>
            <div class="card">
                <h3>家樂福大型賣場</h3>
                <p>面臨大型商品搬運與複雜補貨路徑挑戰，透過 AMR 自動搬運與 AR 導引精準上架，提升效率並改善工作環境。</p>
            </div>
            <div class="card">
                <h3>便利商店智慧化</h3>
                <p>空間狹小、商品眾多、補貨頻繁，導入輕量化 AMR 系統與智慧感測即時監控，可實現 24 小時自動補貨並提升顧客滿意度。</p>
            </div>
        </div>
    </section>

    <!-- 技術整合 優勢 與競爭力 -->
    <section id="advantage" class="container">
        <h2>技術整合優勢與競爭力</h2>
        <p>中強光電集團五大子公司之技術相輔相成，從感測、決策到執行，形成完整閉環，比單點解決方案擁有更高競爭力。本土化技術支援與快速響應能力，確保在特殊需求時可迅速部署與維護。</p>
        <p>本系統符合台灣相關法規，包括 AMRA-201 移動機器人通用要求與 CNS 15556 無人搬運車安全標準。作為自主移動機器人聯盟創始成員，中強光電在安全與技術上具領先優勢。</p>
    </section>

    <footer>
        <p>&copy; 中強光電 智慧補貨閉環系統 2025</p>
        <p>更多資訊：<a href="https://cics.coretronic.com" target="_blank">cics.coretronic.com</a></p>
    </footer>

    <script>
        // 簡易懶加載動畫觸發
        document.addEventListener('DOMContentLoaded', () => {
            const cards = document.querySelectorAll('.card');
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.animationPlayState = 'running';
                        observer.unobserve(entry.target);
                    }
                });
            }, { threshold: 0.2 });
            cards.forEach(card => {
                observer.observe(card);
            });
        });
    </script>
</body>
</html>
