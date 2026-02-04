---
layout: default
---

# 🎲 猜數字 - 直接執行版

### 🚀 操作說明
1. **點擊 Run**：點擊下方視窗綠色的 **[Run]** 按鈕。
2. **開始互動**：程式執行後，在右側的 **[Input]** 區輸入數字並按 Enter 即可遊玩。

<div style="width: 100%; border: 2px solid #007bff; border-radius: 12px; overflow: hidden;">
    <iframe
      src="https://wandbox.org/embed/cpp?code=%23include+%3Ciostream%3E%0A%23include+%3Cctime%3E%0A%23include+%3Ccstdlib%3E%0Ausing+namespace+std%3B%0Aint+main%28%29+%7B%0A++srand%28time%28NULL%29%29%3B%0A++int+num+%3D+rand%28%29+%25+100+%2B+1%2C+guess%3B%0A++cout+%3C%3C+%22%E7%8C%9C%E4%B8%80%E5%80%8B+1~100+%E7%9A%84%E6%95%B8%E5%AD%97%EF%BC%9A%22+%3C%3C+endl%3B%0A++while+%28cin+%3E%3E+guess%29+%7B%0A++++if+%28guess+%3D%3D+num%29+%7B+cout+%3C%3C+%22%E7%8C%9C%E5%B0%8D%E4%BA%86%EF%BC%81%22+%3C%3C+endl%3B+break%3B+%7D%0A++++cout+%3C%3C+%28guess+%3E+num+%3F+%22%E5%A4%AA%E5%A4%A7%E4%BA%86%22+%3A+%22%E5%A4%AA%E5%B0%8F%E4%BA%86%22%29+%3C%3C+endl%3B%0A++%7D%0A++return+0%3B%0A%7D"
      width="100%"
      height="500px"
      style="border: none;">
    </iframe>
</div>

[⬅️ 回到首頁](index)
