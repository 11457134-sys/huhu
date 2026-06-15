* ==========================================
   基礎樣式與淡紫色主題 
   ========================================== */
body {
    font-family: 'Helvetica Neue', Helvetica, Arial, "Microsoft JhengHei", sans-serif;
    background-color: #f4f0fa; /* 極淺淡紫底色 */
    color: #3a2d4a; /* 深紫灰文字 */
    margin: 0;
    padding: 0;
    line-height: 1.6;
}

/* ==========================================
   頁首標題 (Header)
   ========================================== */
header {
    background-color: #4a3765; /* 濃郁紫 */
    padding: 25px 20px;
    text-align: center;
    border-bottom: 3px solid #6c528d;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
}

header h1 {
    color: #f3e8ff; /* 亮淡紫 */
    margin: 0;
    font-size: 26px;
    letter-spacing: 1.5px;
    font-weight: bold;
}

.author-tag {
    color: #d8b4fe;
    font-size: 14px;
    margin-top: 8px;
}

/* ==========================================
   響應式導覽列 (Navigation)
   ========================================== */
nav {
    background-color: #5c457c; /* 中度紫 */
    position: sticky;
    top: 0;
    z-index: 1000;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.08);
}

/* 第一層選單外層 */
.nav-container {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 0;
    list-style: none;
}

/* 主選單項目 */
.nav-item {
    position: relative;
}

.nav-item > a {
    color: #f3e8ff;
    text-decoration: none;
    padding: 15px 20px;
    display: block;
    font-size: 15px;
    font-weight: 500;
    transition: all 0.3s ease;
}

.nav-item:hover > a {
    color: #ffffff;
    background-color: #745b99;
}

/* 第二層下拉選單 (電腦版) */
.dropdown-menu {
    display: none;
    position: absolute;
    top: 100%;
    left: 0;
    background-color: #ffffff;
    box-shadow: 0 8px 16px rgba(0,0,0,0.1);
    min-width: 200px;
    list-style: none;
    padding: 5px 0;
    margin: 0;
    border-radius: 0 0 6px 6px;
    border: 1px solid #e1d7ec;
}

.dropdown-menu li a {
    color: #3a2d4a;
    padding: 10px 20px;
    text-decoration: none;
    display: block;
    font-size: 14px;
    transition: background 0.2s;
}

.dropdown-menu li a:hover {
    background-color: #f3e8ff;
    color: #6d28d9;
}

/* 滑鼠懸停顯示下拉選單 */
.nav-item:hover .dropdown-menu {
    display: block;
}

/* ==========================================
   主要內容區佈局與通用卡片 (Main & Cards)
   ========================================== */
main {
    max-width: 1100px;
    margin: 30px auto;
    padding: 0 20px;
}

.info-card {
    background-color: #ffffff;
    border-radius: 12px;
    padding: 30px;
    margin-bottom: 30px;
    box-shadow: 0 6px 15px rgba(74, 55, 101, 0.04);
    border: 1px solid #e1d7ec;
}

h2 {
    color: #4a3765;
    font-size: 20px;
    margin-top: 0;
    margin-bottom: 18px;
    border-left: 5px solid #8b5cf6;
    padding-left: 12px;
}

h3 {
    color: #6d28d9;
    font-size: 16px;
    margin-top: 20px;
    margin-bottom: 10px;
}

hr {
    border: 0;
    height: 1px;
    background: #e1d7ec;
    margin-bottom: 20px;
}

p {
    margin: 0 0 15px 0;
    font-size: 15px;
    text-align: justify;
}

/* ==========================================
   地圖與互動區塊
   ========================================== */
.map-wrapper {
    width: 100%;
    max-width: 600px;
    margin: 0 auto 20px auto;
    border-radius: 8px;
    overflow: hidden;
    border: 1px solid #dcd1e8;
}

.map-wrapper iframe {
    display: block;
    width: 100%;
}

.info-box {
    display: flex;
    align-items: center;
    background-color: #faf5ff;
    padding: 15px 20px;
    border-radius: 8px;
    font-size: 14.5px;
    border: 1px dashed #c084fc;
    max-width: 560px;
    margin: 0 auto;
}

/* ==========================================
   鳥類入口網格與卡片頁樣式 (Bird Cards Section)
   ========================================== */
.grid-title {
    text-align: center;
    color: #4a3765;
    margin: 40px 0 20px 0;
    font-size: 22px;
}

.card-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* 電腦版一行三張 */
    gap: 25px;
    margin-bottom: 40px;
}

.bird-card {
    background-color: #ffffff;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 6px 18px rgba(74, 55, 101, 0.06);
    border: 1px solid #e1d7ec;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    display: flex;
    flex-direction: column;
}

.bird-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 25px rgba(74, 55, 101, 0.12);
}

/* 縮圖容器 */
.thumbnail-wrapper {
    width: 100%;
    height: 200px;
    overflow: hidden;
    background-color: #eaeaea;
}

.thumbnail-wrapper img {
    width: 100%;
    height: 100%;
    object-fit: cover; /* 自動縮放並填滿，保持完美比例
