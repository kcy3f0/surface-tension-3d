# 🧪 食鹽水表面張力測定裝置 3D 互動模型與探究分析系統

基於**拉脫法（Detachment Method）**之自然科學探究與實作實驗裝置 3D 數位孿生模型與物理模擬系統。

## 🌐 線上展示 (GitHub Pages)
👉 **[點此進入 3D 線上互動檢視器](https://kcy3f0.github.io/surface-tension-3d/)**

---

## 📷 裝置結構與受力分析
![實驗裝置結構與受力分析圖](apparatus_force_analysis.png)

## 📊 食鹽水濃度與表面張力測定數據
![食鹽水濃度與表面張力數據圖表](salt_concentration_surface_tension_chart.png)

---

## 🔬 物理原理與計算公式
- **槓桿力矩平衡**：$L_1 \cdot F_\gamma = L_2 \cdot W$
- 因採用等臂天平（$L_1 = L_2 = 13.5\text{ cm}$）：
  $$F_\gamma = W = m_{\text{珠}} \cdot g$$
- **表面張力計算公式**：
  $$\gamma = \frac{F_\gamma}{L} = \frac{m_{\text{珠}} \cdot g}{L}$$
  * $L = 21.33\text{ cm} = 0.2133\text{ m}$（塑膠杯緣接觸周長）
  * $g = 9.80\text{ m/s}^2$（重力加速度）
  * $m_{\text{珠}}$：拉脫瞬間右側杯中珠子總重量

---

## 🎬 實驗四步驟流程（依據 1018 實錄影片）
1. **① 測量食鹽克數**：使用精密電子秤精確秤量食鹽（0g、25g、50g、75g、100g）。
2. **② 調配食鹽水溶液**：於 1000mL 燒杯中加入定量純水攪拌溶解，使液面恰好接觸倒扣杯緣。
3. **③ 放入珠子增重拉脫**：等臂木條天平歸零後，向右側杯逐顆投入珠子，直至液面水膜頸縮破裂瞬間拉脫。
4. **④ 測量珠子總重換算表面張力**：將臨界拉脫珠子倒回電子秤秤重，代入公式換算表面張力 $\gamma$。

---

## 📁 檔案說明
- `index.html`：3D WebGL 互動模擬器主頁面（支援視角導航、步驟引導、受力向量切換與模型導出）。
- `interactive_3d_viewer.html`：本地獨立運行的離線 3D 檢視器備份。
- `surface_tension_apparatus.glb`：二進位 GLTF 3D 數位孿生模型（支援 PowerPoint 3D、Windows 3D 檢視器）。
- `surface_tension_apparatus.obj` / `.mtl`：通用 3D CAD 模型（支援 Blender、Maya、AutoCAD）。
- `apparatus_force_analysis.png`：高清實驗裝置結構、支架定位、防墜接盤與受力分析圖。
- `salt_concentration_surface_tension_chart.png`：0%~20% 食鹽水濃度與表面張力測定結果圖表。
- `libs/`：Three.js 核心及 OrbitControls、GLTFExporter、OBJExporter 本地相依庫。
