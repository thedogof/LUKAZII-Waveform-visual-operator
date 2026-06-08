
# LUKAZII Waveform Visual Operator

**[ Node-GL Hybrid Signal Flow Architecture ]**

LUKAZII Waveform Visual Operator 是一個專為音訊創作者與視覺設計師打造的高效能即時視覺化工具。它拋棄了傳統 Canvas 2D 的效能瓶頸，採用 **WebGL (Three.js)** 核心引擎，將運算完全交給 GPU，確保在處理多圖層疊加與複雜殘影時，依然能維持絲滑的 60FPS 體驗。

本工具的核心設計哲學在於 **「理性測量」與「感性流動」的平衡** —— 保留專業儀器的精確度，同時賦予聲音流動的有機感。

---

## ⚙️ 核心特色 (Key Features)

*   **Node-based Signal Flow**: 採用節點式邏輯，訊號從 `Audio Source` 到 `Master FX` 層層處理，直觀且具備高度擴充性。
*   **Independent Layer System**: 每個圖層皆為獨立的 WebGL 渲染緩存 (FBO)，支援獨立的混和模式 (Additive/Normal)、透明度與空間變形 (Transform)。
*   **GPU Accelerated**: 利用 `Three.js` 與 `BufferGeometry` 處理數以萬計的粒子與複雜波形，告別 CPU 運算卡頓。
*   **Pro-grade Aesthetics**: 極簡、包浩斯風格的 HUD 介面，支援多種專業配色預設 (Amber HUD, Mono Tech, Matrix, Paper Ink...)。
*   **Audio Reactive**: 即時 Web Audio API 串接，波形、粒子密度皆可與音頻頻段連動。

## 🛠 技術堆疊 (Tech Stack)

*   **Engine**: Three.js (WebGL)
*   **Audio**: Web Audio API (FFT / Time Domain Analysis)
*   **UI/Logic**: Vanilla JavaScript (Modular Architecture)
*   **Style**: CSS Grid / Flexbox (Industrial HUD Aesthetic)

## 🚀 如何使用 (Usage)

1. **Clone/Download**: 下載或 Clone 此專案。
2. **Open**: 直接以現代瀏覽器 (Chrome/Edge/Firefox) 開啟 `index.html`。
3. **Inject**: 點擊 `[ LOAD AUDIO ]` 上傳你的音樂檔案。
4. **Operate**: 
    * 左側 **Signal Flow** 管理你的圖層 (Layer) 堆疊與排序 (Z-index)。
    * 右側 **Inspector** 調節各個圖層的波形參數、粒密度與 FX 效果。

## 💡 創作理念 (Design Philosophy)

此專案深受特斯拉與工業控制介面啟發。我們不追求炫目的動效，而是專注於「數據的可視化」。每一個線條、每一份粉塵的漂浮，都是為了輔助創作者在進行混音、編曲時，能從視覺上「看見」聲音的質感。

## 📅 Roadmap (未來計畫)

- [ ] **Custom Shader Integration**: 引入自定義 GLSL Shader 節點。
- [ ] **MIDI Integration**: 透過 Web MIDI API 連動實體硬體控制台。
- [ ] **Advanced Triggering**: 加入波形觸發 (Zero-crossing detection) 以穩定示波器畫面。

---

**Built with love by LUKAZII**
*Let the signal flow.*

---
