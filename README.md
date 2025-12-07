☁️ 安安天天氣象 (An An Weather) - 前端

這是一個充滿三麗鷗（Sanrio）風格的療癒系天氣預報 Web App。透過粉嫩的配色、可愛的圓體字與溫暖的文案，將查看天氣轉化為一件療癒的日常體驗。

本專案採用 Vibe Coding 精神開發，強調使用者的視覺感受與情感連結。

✨ 特色功能

🌸 三麗鷗視覺風格：

運用 Sanrio Palette（粉紅、奶油白、天空藍）配色。

大量使用圓角 (Border-radius)、虛線邊框與毛玻璃效果。

加入細微的彈跳 (Bounce) 與搖擺 (Sway) 動畫，讓介面「活」起來。

📍 臺北市即時預報：

串接後端 API，取得臺北市未來 36 小時天氣資訊。

顯示即時氣溫、天氣圖示與降雨機率。

🧣 貼心生活建議：

智慧穿搭：根據氣溫判斷該穿「清涼短袖」還是「暖暖外套」。

雨具提醒：將生硬的降雨機率轉化為「放心出門啦」或「記得帶傘喔」等口語化建議。

📱 響應式設計 (RWD)：

針對手機體驗優化，支援觸控滑動查看未來預報。

在桌面版限制最大寬度，保持卡片式設計的美感。

🛠️ 技術堆疊

HTML5: 語意化標籤結構。

CSS3:

CSS Variables (變數) 管理主題配色。

Flexbox & Grid 用於佈局排版。

@keyframes 製作可愛的載入與互動動畫。

JavaScript (Vanilla JS):

ES6+ 語法。

Fetch API 處理非同步資料請求。

DOM 操作與動態渲染。

字體: Zen Maru Gothic (Google Fonts)。

🚀 快速開始

由於本專案為純靜態網頁（Static Web Page），無需複雜的編譯步驟。

方法 1：直接開啟

雙擊資料夾中的 index.html 檔案，透過瀏覽器直接開啟即可預覽（部分瀏覽器可能會因 CORS 限制導致 API 無法抓取，建議使用方法 2）。

方法 2：使用 Live Server (推薦)

如果你使用 VS Code 開發：

安裝 Live Server 擴充套件。

在 index.html 上按右鍵，選擇 "Open with Live Server"。

⚙️ 設定後端連結

預設情況下，前端會連線至設定好的雲端 API。若您要在本地端進行完整測試（包含後端）：

請先啟動後端伺服器 (參見後端 README)。

開啟 index.html。

搜尋 const API_URL 變數。

將其修改為本地後端位址：

// 修改前 (雲端 API)
const API_URL = "[https://cwa-weather-backend-ken.zeabur.app/api/weather/taipei/](https://cwa-weather-backend-ken.zeabur.app/api/weather/taipei/)";

// 修改後 (本地 API)
const API_URL = "http://localhost:3000/api/weather/taipei";


📂 專案結構

AnAnWeather-frontend/
├── index.html      # 主網頁 (包含 HTML, CSS, JS)
├── icon-v2.png     # 網站圖示 (Favicon)
└── README.md       # 說明文件


注意：為了方便部署與展示，目前的 CSS 樣式與 JavaScript 邏輯皆整合在 index.html 單一檔案中。

🎨 設計細節 (Vibe Coding)

字體優化：針對標題與內文使用了不同的字重 (Weight) 與字距 (Letter-spacing)，增加閱讀的舒適度。

載入畫面：設計了專屬的 Loading 頁面（正在接收可愛電波...），減少等待時的焦躁感。

互動回饋：按鈕與卡片在載入時會有輕微的動畫效果。

授權

MIT