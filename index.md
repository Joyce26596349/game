---
layout: default
---

<style>
    /* 1. 徹底隱藏側邊欄位與多餘資訊，釋放所有右側空間 */
    aside#sidebar, footer, .view { display: none !important; }
    
    /* 2. 頁面極致加寬，防止截圖中的窄化變形 */
    section#main_content { 
        width: 100% !important; 
        max-width: 1200px !important; 
        margin: 0 auto !important; 
        float: none !important; 
        display: block !important;
        padding: 40px 20px !important;
    }

    /* 3. 遊戲容器：改為三欄橫向並排 */
    .game-container {
        display: flex;
        gap: 20px;
        margin: 40px 0;
        width: 100%;
        justify-content: center;
        flex-wrap: wrap; /* 在小螢幕時自動換行 */
    }

    /* 4. 遊戲卡片樣式 */
    .game-card {
        flex: 1 1 300px; /* 基本寬度 300px，平分空間 */
        max-width: 380px;
        box-sizing: border-box;
        padding: 40px 25px;
        border: 1px solid #e1e4e8;
        border-radius: 20px;
        background-color: #ffffff;
        text-align: center;
        text-decoration: none !important;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        min-height: 400px;
        transition: all 0.3s ease;
        box-shadow: 0 10px 25px rgba(0,0,0,0.05);
    }
    
    .game-card:hover {
        transform: translateY(-10px);
        box-shadow: 0 20px 40px rgba(0,0,0,0.12);
        border-color: #28a745; /* 懸停時變綠色，增加遊戲感 */
    }

    .game-title { 
        font-size: 1.8em; 
        font-weight: bold; 
        color: #28a745; 
        margin-bottom: 15px; 
        display: block; 
    }
    
    .game-desc { 
        font-size: 1.05em; 
        color: #555; 
        margin-bottom: 25px; 
        line-height: 1.6; 
        display: block; 
        flex-grow: 1;
    }

    /* 5. Colab 徽章樣式 */
    .colab-badge {
        margin: 15px 0;
        display: block;
    }
    .colab-badge img {
        height: 32px;
    }

    /* 6. 進入遊戲按鈕 */
    .btn-play {
        display: block;
        padding: 12px 0;
        width: 100%;           
        background-color: #28a745;
        color: white !important;
        border-radius: 10px;
        font-weight: bold;
        font-size: 1.1em;
        text-decoration: none !important;
    }
</style>

# 🕹️ 我的 C++ 遊戲平台
歡迎來到我的工程專題展示，這裡收集了我使用 C++ 開發的幾款經典邏輯遊戲。

<div class="game-container">

    <a href="1A2B" class="game-card">
        <div>
            <span class="game-title">🔢 1A2B 遊戲</span>
            <span class="game-desc">經典的猜數字遊戲！挑戰在最少次數內猜中不重複的四位數，考驗你的邏輯推論能力。</span>
            <div class="colab-badge">
                <object data="https://colab.research.google.com/assets/colab-badge.svg" type="image/svg+xml">
                    <a href="https://colab.research.google.com/github/Joyce26596349/technology_class-report/blob/main/1A2B.ipynb" target="_blank">
                        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab">
                    </a>
                </object>
            </div>
        </div>
        <span class="btn-play">查看原始碼</span>
    </a>

    <a href="bomb" class="game-card">
        <div>
            <span class="game-title">💣 終極密碼</span>
            <span class="game-desc">在限定範圍內猜出正確數字，範圍會隨之縮小，小心別踩到地雷數字！</span>
            <div class="colab-badge">
                <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Colab Ready" style="filter: grayscale(1); opacity: 0.5;">
            </div>
        </div>
        <span class="btn-play">進入遊戲說明</span>
    </a>

    <a href="guess" class="game-card">
        <div>
            <span class="game-title">🎲 猜數字</span>
            <span class="game-desc">簡單直觀的數字挑戰，練習 C++ 的隨機數生成與條件判斷邏輯。</span>
            <div class="colab-badge">
                <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Colab Ready" style="filter: grayscale(1); opacity: 0.5;">
            </div>
        </div>
        <span class="btn-play">進入遊戲說明</span>
    </a>

</div>
