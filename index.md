---
layout: default
---

<style>
    /* 移除側邊欄，讓版面加寬 */
    aside#sidebar, footer, .view { display: none !important; }
    section#main_content { 
        width: 100% !important; 
        max-width: 1200px !important; 
        margin: 0 auto !important; 
        float: none !important; 
    }

    .game-grid { display: flex; gap: 20px; margin-top: 40px; }
    .game-card { 
        flex: 1; padding: 30px; border: 1px solid #ddd; border-radius: 15px; 
        text-align: center; text-decoration: none !important; color: #333; 
        transition: 0.3s; background: #fff;
    }
    .game-card:hover { border-color: #28a745; transform: translateY(-5px); box-shadow: 0 10px 20px rgba(0,0,0,0.1); }
    .btn-go { display: block; margin-top: 15px; background: #28a745; color: white; padding: 10px; border-radius: 8px; font-weight: bold; }
</style>

# 🕹️ C++ 網頁遊戲工作坊
點擊下方卡片進入遊戲，程式碼會自動載入。

<div class="game-grid">
    <a href="1A2B" class="game-card">
        <span style="font-size: 3em;">🔢</span>
        <h2>1A2B</h2>
        <p>邏輯推導挑戰</p>
        <span class="btn-go">開始遊戲</span>
    </a>
    <a href="bomb" class="game-card">
        <span style="font-size: 3em;">💣</span>
        <h2>終極密碼</h2>
        <p>緊張刺激的數字地雷</p>
        <span class="btn-go">開始遊戲</span>
    </a>
    <a href="guess" class="game-card">
        <span style="font-size: 3em;">🎲</span>
        <h2>猜數字</h2>
        <p>經典隨機數挑戰</p>
        <span class="btn-go">開始遊戲</span>
    </a>
</div>
