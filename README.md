# 🎨 AR_Coloring

> **將手繪 2D 圖紙透過 AR 技術轉換成可互動的 3D 立體模型**

AR_Coloring 是一個使用 **Unity** 開發的擴增實境（Augmented Reality, AR）專案。

使用者可以先在紙本圖紙上進行彩繪，再透過手機掃描完成的圖紙，將原本的 **2D 彩繪作品轉換成具有立體效果的 3D 模型**，並在 AR 環境中查看。

本專案以「**貓咪**」作為實例，使用者可以分別彩繪貓咪的正面與背面，完成後透過手機進行掃描，即可在 AR 環境中呈現一隻完整的 **3D 立體彩繪貓咪**。

---

## 📱 Demo

### 使用流程

```text
紙本圖紙
   ↓
使用者彩繪
   ↓
完成正面 / 背面彩繪
   ↓
使用手機 AR_Coloring 掃描
   ↓
辨識彩繪內容
   ↓
套用至 3D 模型
   ↓
呈現 AR 3D 立體貓咪
```

### 🐱 實際案例

本專案以「空白貓咪」作為範例：

1. 準備空白的貓咪圖紙。
2. 使用者在紙張上替貓咪進行彩繪。
3. 分別完成貓咪正面與背面的圖案。
4. 開啟 `AR_Coloring`。
5. 使用手機鏡頭掃描彩繪完成的圖紙。
6. 系統將彩繪內容對應至 3D 貓咪模型。
7. 最終在手機 AR 環境中呈現彩繪完成的 **3D 立體貓咪**。

也就是：

**2D 手繪 → AR 掃描 → 3D 立體呈現**

---

## ✨ Project Features

- 🎨 **紙本彩繪**
  - 使用者可以直接在實體圖紙上自由創作。

- 📷 **AR 圖像掃描**
  - 使用手機鏡頭掃描完成的彩繪圖紙。

- 🧩 **彩繪內容與 3D 模型結合**
  - 將使用者在紙張上的彩繪內容對應至 3D 模型。

- 🐱 **2D → 3D**
  - 將原本的平面彩繪作品轉換成具有立體效果的 AR 物件。

- 🔄 **正面與背面彩繪**
  - 透過正面及背面的彩繪內容，呈現完整的 3D 立體角色。

- 📱 **Mobile AR**
  - 使用手機即可查看完成後的 AR 3D 模型。

---

## 🛠️ Technology

| Technology | Purpose |
|---|---|
| Unity | AR 應用程式開發 |
| C# | Unity 程式邏輯 |
| AR Technology | 圖像辨識與 AR 物件呈現 |
| 3D Model | 立體角色模型 |
| Mobile Camera | 掃描與辨識彩繪圖紙 |

---

## 🏗️ System Concept

AR_Coloring 的核心概念是將「**實體彩繪**」與「**數位 3D 模型**」結合。

```text
┌──────────────────┐
│   Physical Paper │
│                  │
│   🎨 User Color  │
│                  │
└────────┬─────────┘
         │
         │ Camera Scan
         ▼
┌──────────────────┐
│   AR Recognition │
│                  │
│  Detect Artwork  │
└────────┬─────────┘
         │
         │ Texture / Image Mapping
         ▼
┌──────────────────┐
│    3D Model      │
│                  │
│  Apply Artwork   │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│   AR 3D Object   │
│                  │
│    🐱 Cat        │
│                  │
└──────────────────┘
```

---

## 🎯 Example: AR Coloring Cat

本專案的展示案例為一隻空白貓咪。

### Step 1 — Blank Model

首先準備一個沒有顏色的貓咪圖紙。

```text
        /\_/\
       ( o.o )
        > ^ <
```

使用者可以在紙張上自由設計貓咪的外觀。

### Step 2 — Coloring

使用者分別對貓咪的：

- 正面
- 背面

進行彩繪。

例如：

```text
      Front                Back

    🎨 Color              🎨 Color
       ↓                     ↓

    [ Cat ]               [ Cat ]
```

### Step 3 — AR Scanning

完成彩繪後，使用手機開啟 AR_Coloring，利用手機鏡頭掃描圖紙。

系統辨識圖像後，將使用者的彩繪內容與對應的 3D 模型進行結合。

### Step 4 — 3D AR Result

最後，手機畫面中會出現一隻具有使用者彩繪內容的 **3D 立體貓咪**。

```text
       📱
        │
        ▼

       /\_/\
      ( •.• )
      /     \
     /  🎨   \
    /_________\
       🐾 🐾

      3D Cat
```

使用者可以從不同角度觀察模型，看到原本紙本彩繪在 3D 空間中的呈現效果。

---

## 🔄 2D → 3D Concept

本專案的主要特色可以簡化為：

```text
       2D World
┌─────────────────┐
│                 │
│  ✏️ Draw / Color │
│                 │
│   Paper Artwork │
│                 │
└────────┬────────┘
         │
         │ AR Scan
         ▼
┌─────────────────┐
│  Image / Color  │
│    Processing   │
└────────┬────────┘
         │
         │ Mapping
         ▼
       3D World
┌─────────────────┐
│                 │
│   🐱 3D Model   │
│                 │
│  AR Experience  │
│                 │
└─────────────────┘
```

因此，使用者不需要直接操作複雜的 3D 建模工具，而是可以透過熟悉的「**畫畫**」方式建立自己的 3D AR 作品。

---

## 📂 Project Structure

```text
AR_Coloring/
│
├── Assets/
│   ├── Scenes/
│   ├── Scripts/
│   ├── Models/
│   ├── Materials/
│   ├── Textures/
│   ├── Prefabs/
│   └── ...
│
├── Packages/
│
├── ProjectSettings/
│
└── README.md
```

> 實際資料夾結構會依 Unity 專案版本與專案整理方式有所不同。

---

## 🚀 How to Run

### Requirements

- Unity
- Android / iOS mobile device
- Mobile camera
- AR-supported device

### Installation

1. Clone this repository.

```bash
git clone <YOUR_REPOSITORY_URL>
```

2. 使用 Unity Hub 開啟專案。

3. 開啟對應的 Scene。

4. 將專案 Build 至支援 AR 的手機裝置。

5. 啟動 App。

6. 使用手機鏡頭掃描完成彩繪的圖紙。

7. 查看 AR 3D 模型。

---

## 📸 Project Workflow

```text
┌─────────────┐
│ Blank Paper │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│   Coloring  │
│     🎨      │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│   Scanning  │
│     📷      │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│ AR Detection│
└──────┬──────┘
       │
       ▼
┌─────────────┐
│ Texture /   │
│ Model Apply │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│ 3D AR Cat   │
│     🐱      │
└─────────────┘
```

---

## 💡 Project Motivation

傳統的兒童彩繪作品通常以平面紙張作為最終成果。

本專案希望將「**繪畫**」與「**AR / 3D 技術**」結合，讓使用者完成彩繪後，可以透過手機看到自己的作品以 3D 形式呈現。

透過這種方式，原本的：

> **2D 紙本作品**

可以進一步轉換成：

> **可在 AR 環境中觀看的 3D 數位作品**

讓使用者能夠以更直觀、更具互動性的方式體驗自己的創作。

---

## 🎓 Skills Demonstrated

本專案實作過程中涵蓋以下能力：

- Unity 開發
- C# Programming
- AR Application Development
- Image Recognition / Tracking
- 3D Model Integration
- Texture Mapping
- Mobile Application Development
- Camera Integration
- Unity Scene / Prefab Management
- AR User Experience Design

---

## 🧪 Example Scenario

### Coloring Cat

```text
① 空白貓咪圖紙

       🐱
   ─────────
    Blank Cat
   ─────────

          ↓

② 使用者進行彩繪

       🎨
       🐱
    User Artwork

          ↓

③ 手機掃描

       📱
        │
        │ Camera
        ▼
       🐱

          ↓

④ AR 3D Model

        🐱
      ／   ＼
     /  🎨   \
    /_________\
       🐾 🐾

    3D AR Cat
```

---

## 📌 Project Status

**Completed ✅**

目前已完成：

- [x] Unity AR application
- [x] Image recognition / scanning
- [x] 2D artwork integration
- [x] 3D model presentation
- [x] Front / back coloring
- [x] Mobile AR demonstration
- [x] 2D → 3D AR experience

---

## 👨‍💻 Author

**Yu-Chen Chao**

Computer Science / Information Engineering Student

Interested in:

- Software Development
- Unity
- AR / VR
- Mobile Application Development
- Computer Vision
- Embedded Systems
- FPGA / RISC-V

---

## 📄 License

This project is for **educational and portfolio purposes**.

Please contact the author before using project assets, models, textures, or other copyrighted materials for commercial purposes.

## Unity File

1. https://drive.google.com/file/d/1-lZ1SMx8JoJYXvuxYXrcIFnLS2hI55dV/view?usp=drive_link  (Stable version)
2. https://drive.google.com/file/d/151DE1s6fAdDLGBEslqNwmxj5WqBvVvc5/view?usp=drive_link  
