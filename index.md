---
layout: default
---

<style>
    /* 1. 徹底解除主題限制，讓頁面變寬 */
    aside#sidebar, footer, .view { display: none !important; }
    section#main_content { 
        width: 100% !important; 
        max-width: 1200px !important; 
        margin: 0 auto !important; 
        float: none !important; 
        padding: 40px 20px !important;
    }

    /* 2. 遊戲卡片容器：橫向並排 */
    .game-grid {
        display: flex;
        gap: 25px;
        margin-top: 40px;
        justify-content: center;
        flex-wrap: nowrap; /* 強制橫向不換行 */
    }

    /* 3. 卡片細節設計 */
    .game-card {
        flex: 1;
        padding: 35px 25px;
        border: 1px solid #e1e4e8;
        border-radius: 20px;
        background: #ffffff;
        text-align: center;
        box-shadow: 0 8px 20px rgba(0,0,0,0.06);
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        min-height: 380px;
        transition: transform 0.3s ease, border-color 0.3s ease;
        text-decoration: none !important;
    }

    .game-card:hover {
        transform: translateY(-10px);
        border-color: #28a745;
        box-shadow: 0 15px 35px rgba(0,0,0,0.12);
    }

    .game-icon { font-size: 3em; margin-bottom: 15px; display: block; }
    .game-title { font-size: 1.8em; font-weight: bold; color: #28a745; margin-bottom: 10px; display: block; }
    .game-desc { color: #555; font-size: 1em; line-height: 1.5; margin-bottom: 20px; flex-grow: 1; display: block; }

    /* 4. 遊戲按鈕 */
    .btn-play {
        display: block;
        padding: 12px 0;
        background: #28a745;
        color: white !important;
        border-radius: 12px;
        font-weight: bold;
        font-size: 1.1em;
        transition: background 0.2s;
    }
    .btn-play:hover { background: #218838; }
</style>

# 🕹️ C++ 遊戲線上工作坊
歡迎來到我的工程專題成果展！這裡的所有遊戲都可以直接在瀏覽器中執行。

<div class="game-grid">

    <a href="1A2B" class="game-card">
        <div>
            <span class="game-icon">🔢</span>
            <span class="game-title">1A2B</span>
            <span class="game-desc">經典邏輯推理遊戲。挑戰在最少次數內猜出正確數字，考驗你的大腦極限！</span>
        </div>
        <span class="btn-play">直接在網頁玩</span>
    </a>

    <a href="bomb" class="game-card">
        <div>
            <span class="game-icon">💣</span>
            <span class="game-title">終極密碼</span>
            <span class="game-desc">數字範圍不斷縮小，誰會踩到最後的地雷？緊張刺激的運氣對決。</span>
        </div>
        <span class="btn-play">直接在網頁玩</span>
    </a>

    <a href="guess" class="game-card">
        <div>
            <span class="game-icon">🎲</span>
            <span class="game-title">猜數字</span>
            <span class="game-desc">基礎而有趣的數字挑戰，透過系統提示的高低範圍找出隱藏的目標。</span>
        </div>
        <span class="btn-play">直接在網頁玩</span>
    </a>

</div>

---


### 💡 執行小撇步
點擊「直接在網頁玩」後，您會看到一個 **JupyterLite** 視窗。
1. 等待左下角出現 **Idle**。
2. 將該頁面下方的程式碼複製並貼入視窗。
3. 按下鍵盤 **Shift + Enter** 即可開始遊戲！
