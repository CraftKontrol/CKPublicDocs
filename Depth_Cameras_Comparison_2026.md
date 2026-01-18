# 🎥 Depth Camera Comparison 2026
**Updated:** Jan 17, 2026 | **Author:** Arnaud Cassone © Artcraft Visuals

## 🏆 Top Picks

### 📐 Best Resolution

| Rank | Model | Depth Resolution | RGB Resolution | Price | Technology | Notes |
|------|-------|------------------|----------------|-------|------------|-------|
| 🥇 | **ZED 2/2i/X** | **2208×1242** | **2208×1242** | €450-750 | Stereo Vision | Highest overall, 60-120fps, spatial AI |
| 🥈 | **Astra 2** | **1600×1200** | 1920×1080 | €200-250 | Structured Light | Best structured light, best value |
| 🥉 | **Lucid Helios2** | **1456×1088** | - | €1,500-3k | iToF | Industrial grade |
| 4 | **Azure Kinect** | 1024×1024 | **3840×2160 (4K)** | €500 | iToF | Discontinued, highest RGB |
| 5 | **OAK-D Pro** | 1280×800 | **12MP (4K)** | $399 | Stereo Vision | 48 TOPS AI, laser dot |
| 6 | **Intel D435i** | 1280×720 | 1920×1080 | €468 | Stereo Vision | Wide FOV, proven |
| 7 | **L515** | 1024×768 | 1920×1080 | €450+ | LiDAR (dToF) | ±5mm accuracy, discontinued |
| 8 | **Femto Bolt/Mega** | 1024×1024 | 1920×1080 | €300-450 | iToF | Azure compatible |
| 9 | **Photoneo PhoXi 3D** | 1680×1200 | - | €5,000+ | Structured Light | Industrial scanning |
| 10 | **Zivid Two M130** | 1944×1200 | - | €10,000+ | Structured Light | Professional 3D scanning |

### 🌐 Best Connectivity

| Type | Model | Price | Features | Range | Technology | Notes |
|------|-------|-------|----------|-------|------------|-------|
| **PoE** | **D555 PoE** | €720 | Vision SoC V5, IP65, 90fps | 0.4-6m | Stereo Vision | Industrial, GigE, outdoor rated |
| **PoE** | **OAK-D Pro PoE** | $499 | 48 TOPS AI, 802.3af, 12MP RGB | 0.2-35m | Stereo Vision | No USB needed, AI onboard |
| **PoE** | **Femto Mega** | €350-450 | Dual USB/GigE PoE, Azure SDK | 0.4-5.5m | iToF | Dual interface, IMU |
| **PoE** | **OAK-4** | $599+ | 4 cameras, self-healing, 48MP RGB | 0.2-35m | Stereo + Multi | USB-C or PoE selectable |
| **PoE** | **Zivid Two M130** | €10,000+ | Professional 3D, IP65 | 0.3-1.3m | Structured Light | Industrial scanning |
| **PoE** | **Photoneo PhoXi 3D** | €5,000+ | High precision, GigE | 0.4-3m | Structured Light | Factory automation |
| **Dual** | **Femto Mega I** | €400-500 | USB 3.0 + GigE PoE, enhanced | 0.4-5.5m | iToF | Azure compatible |
| **GMSL** | **Intel D457** | €690 | GMSL/FAKRA, IP65, automotive | 0.4-6m | Stereo Vision | Automotive certified |
| **GMSL2** | **ZED X** | €750 | GMSL2 or USB 3.1, 120fps | 0.5-20m | Stereo Vision | Highest FPS option |
| **GigE** | **Basler blaze-101** | €1,000-1,500 | GigE or USB 3.0, compact | 0.3-10m | iToF | Industrial ToF |
| **GigE** | **Lucid Helios2** | €1,500-3,000 | GigE, 1456×1088 depth | 0.3-10m | iToF | High resolution industrial |
| **Ethernet** | **Livox Mid-360** | €500-600 | 360° horizontal, 100K pts/sec | 0.5-40m | LiDAR | Outdoor mapping |
| **Ethernet** | **Ouster OS0/OS1** | €3,000-15k | 2048 beams, 10/20Hz | 0.5-50m | LiDAR | Professional automotive |
| **USB 3.1** | **OAK-D Pro W** | $449 | 150°×110° ultra-wide FOV | 0.2-35m | Stereo Vision | Widest FOV |
| **USB 3.0** | **Astra 2** | €200-250 | 1600×1200 depth, IMU, sync | 0.6-8m | Structured Light | Best value USB 3.0 |

### 💻 Best SDK

| SDK | Manufacturer | Languages | Platforms | Key Features | Best Models | Downloads/Community |
|-----|--------------|-----------|-----------|--------------|-------------|---------------------|
| **DepthAI** | Luxonis (OAK) | Python, C++ | Win/Linux/macOS/ARM | **48 TOPS AI**, onboard inference, PyTorch/TF/ONNX, ROS/ROS2, custom pipelines | OAK-D Pro, OAK-4, OAK-D Lite | **2.5M+ downloads**, open-source |
| **RealSense 2.0** | Intel | Python, C++, C#, Node.js | Win/Linux/macOS | **Largest ecosystem**, Unity/Unreal, ROS/ROS2, best docs, proven | D455, D435i, D555 PoE, L515 | **Largest community** |
| **ZED SDK** | Stereolabs | Python, C++, C#, Unity | Win/Linux | **Neural depth**, spatial AI, positional tracking, object/body detection, extreme conditions | ZED 2i, ZED X, ZED 2 | Strong, professional |
| **Orbbec SDK** | Orbbec | Python, C++, C | Win/Linux | **Azure Kinect compatible**, TouchDesigner ready, multi-device sync, OpenNI | Femto Bolt/Mega, Astra 2, Gemini 2 | Growing, TD integration ✅ |
| **Azure Kinect SDK** | Microsoft | Python, C++, C# | Win/Linux | 7-mic array, body tracking, cognitive services (discontinued) | Azure Kinect DK, Femto Bolt/Mega (compatible) | Large, maintained by Orbbec |
| **Industrial SDKs** | Various | C++, C | Win/Linux | GigE Vision, GenICam, high precision, factory automation | Basler, Lucid, Zivid, Photoneo | Industry standard |

## 📊 Specifications

### Intel RealSense

| Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV (H×V) | IMU | Price (€) | Notes |
|-------|------------|---------------------|-------------------|---------|-------|--------------|-----------|-----|-----------|-------|
| **D405** | Stereo Vision | 1280×720 | 1280×720 | 90 fps | 0.07-0.5m | USB-C 3.1 | 87°×58° | ❌ | €415 | Close-range, OV9782 |
| **D415** | Stereo Vision | **1280×720** | **1920×1080** | 90 fps | 0.3-10m | USB-C 3.0 | 65°×40° | ❌ | €372 | Narrow FOV, rolling shutter |
| **D435** | Stereo Vision | **1280×720** | **1920×1080** | 90 fps | 0.3-10m | USB-C 3.1 | 86°×57° | ❌ | €456 | Wide FOV, rolling shutter |
| **D435i** | Stereo Vision | **1280×720** | **1920×1080** | 90 fps | 0.3-10m | USB-C 3.1 | 86°×57° | ✅ | €468 | D435 + 6-DoF IMU |
| **D435if** | Stereo Vision | **1280×720** | **1920×1080** | 90 fps | 0.3-10m | USB-C 3.1 | 86°×57° | ✅ | €567 | IR pass filter + IMU |
| **D455** | Stereo Vision | **1280×720** | **1280×720** | 90 fps | 0.4-6m | USB-C 3.1 | 86°×57° | ✅ | €588 | **Global shutter, best outdoor** |
| **D455f** | Stereo Vision | **1280×720** | **1280×720** | 90 fps | 0.4-6m | USB-C 3.1 | 86°×57° | ✅ | €612 | D455 + IR pass filter |
| **D456** | Stereo Vision | **1280×720** | **1280×720** | 90 fps | 0.4-10m | USB-C 3.1 | 86°×57° | ✅ | €678 | 3 sensors, extended range |
| **D457** | Stereo Vision | **1280×720** | **1280×720** | 90 fps | 0.4-6m | **GMSL/FAKRA** | 86°×57° | ✅ | €690 | **IP65, automotive** |
| **D555 PoE** | Stereo Vision | **1280×720** | **1280×720** | 90 fps | 0.4-6m | **GigE PoE** | 86°×57° | ✅ | €720 | **Vision SoC V5, IP65, industrial** |
| **L515** | LiDAR (dToF) | **1024×768** | **1920×1080** | 30 fps | 0.25-9m | USB-C 3.1 | 70°×55° | ❌ | €450+ | ±5mm accuracy, discontinued |

### Luxonis OAK

| Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV (H×V) | IMU | Price ($) | Notes |
|-------|------------|---------------------|-------------------|---------|-------|--------------|-----------|-----|-----------|-------|
| **OAK-D Lite** | Stereo Vision | **1280×800** | **4K (3840×2160)** | 60 fps | 0.2-35m | USB-C 3.1 | 127°×80° | ❌ | $150 | Budget, Myriad X AI |
| **OAK-D** | Stereo Vision | **1280×800** | **4K (3840×2160)** | 60 fps | 0.2-35m | USB-C 3.1 | 127°×80° | ✅ | $299 | **48 TOPS AI, onboard CV** |
| **OAK-D Pro** | Stereo Vision | **1280×800** | **12MP (4K)** | 60 fps | 0.2-35m | USB-C 3.1 | 127°×80° | ✅ | $399 | **Laser dot, night vision** |
| **OAK-D Pro PoE** | Stereo Vision | **1280×800** | **12MP (4K)** | 60 fps | 0.2-35m | **PoE (802.3af)** | 127°×80° | ✅ | $499 | **Native PoE, no USB** |
| **OAK-D Pro W** | Stereo Vision | **1280×800** | **12MP (4K)** | 60 fps | 0.2-35m | USB-C 3.1 | **150°×110°** | ✅ | $449 | **Ultra-wide FOV** |
| **OAK-4** | Stereo + Multi | **1280×800** | **48MP** | 60 fps | 0.2-35m | USB-C / PoE | 127°×80° | ✅ | $599+ | **Self-healing, 4 cameras** |

**Key Features:**
- All models include Myriad X VPU (48 TOPS AI processing)
-All OAK: Myriad X VPU (48 TOPS AI), onboard CV/ML, PyTorch/TensorFlow/ONNX support*

### Orbbec - Structured Light (Astrasolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV (H×V) | IMU | Price (€) | Notes |
|-------|------------|---------------------|-------------------|---------|-------|--------------|-----------|-----|-----------|-------|
| **Astra 2** | Structured Light | **1600×1200** | **1920×1080** | 30 fps | 0.6-8m | **USB 3.0 Type-C** | Depth: 58.2°×45.2° / RGB: 74.7°×46.2° | ✅ | €200-250 | **Orbbec ASIC, 241g, multi-camera sync** |
| Astra+ | Structured Light | **640×480** | 640×480 | 30 fps | 0.6-8m | USB 2.0 | 60°×49.5° | ❌ | €150 | Legacy, VGA RGB |
| Astra Mini Pro | Structured Light | **640×480** | 1280×960 | 30 fps | 0.35-2.5m | USB 2.0 | 60°×49.5° | ❌ | €200 | Compact, short range |
| Astra Embedded S | Structured Light | **640×480** | 1280×960 | 30 fps | 0.6-8m | USB 2.0 | 60°×49.5° | ❌ | - | Legacy, embedded |

#### Stereo Vision (Gemini Series)

| Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV (H×V) | IMU | Price (€) | Notes |
|-------|------------|---------------------|-------------------|---------|-------|--------------|-----------|-----|-----------|-------|
| **Gemini 2** | Stereo Vision | **640×400** | **1920×1080** | 30 fps | 0.5-5m | USB 3.0 | 67°×45° | ❌ | €200-250 | Good value |
| **Gemini 305** | Stereo Vision | **640×400** | **1920×1080** | 30 fps | **0.04-1m** | USB 3.0 | 67°×45° | ✅ | €300+ | **4cm ultra-close, 65g** |
| **Gemini 305g** | Stereo Vision | **640×400** | **1920×1080** | 30 fps | 0.04-1m | USB 3.0 | 67°×45° | ✅ | €320+ | Gemini 305 variant |
| **Gemini 335** | Stereo Vision | **640×400** | **1920×1080** | 30 fps | 0.15-5m | USB 3.0 | 67°×45° | ❌ | €250-300 | Binocular + structured light |
| G Orbbec - Stereo Vision (Gemini*640×400** | **1920×1080** | 30 fps | 0.15-5m | USB 3.0 | 67°×45° | ❌ | €260-310 | Long-range variant |
| Gemini 335Lg | Stereo Vision | **640×400** | **1920×1080** | 30 fps | 0.15-5m | USB 3.0 | 67°×45° | ✅ | €280-330 | Long-range + global shutter |
| Gemini 336 | Stereo Vision | **640×400** | **1920×1080** | 30 fps | 0.15-5m | USB 3.0 | 67°×45° | ❌ | €270-320 | Enhanced Gemini 335 |

#### ToF (Time-of-Flight) Series

| Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV (H×V) | IMU | Price (€) | Notes |
|-------|------------|---------------------|-------------------|---------|-------|--------------|-----------|-----|-----------|-------|
| **Femto Bolt** | iToF | **1024×1024** | **1920×1080** | 30 fps | 0.25-5.46m | USB 3.0 | 75°/120° NFOV/WFOV | ✅ | €300-400 | **Azure Kinect compatible SDK** |
| **Femto Mega** | iToF | **1024×1024** | **1920×1080** | 30 fps | 0.4-5.5m | **USB 3.0 / GigE PoE** | 75°/120° NFOV/WFOV | ✅ | €350-450 | **PoE support, dual interface** |
| **Femto Mega I** | iToF | **1024×1024** | **1920×1080** | 30 fps | 0.4-5.5m | USB 3.0 / GigE PoE | 75°/120° NFOV/WFOV | ✅ | €400-500 | Enhanced version |
| Femto W | iToF | **640×576** | 1920×1080 | 30 fps | 0.3-5m | USB 3.0 | 120° WFOV | ❌ | €250 | Legacy, wide FOV |
| F Orbbec - ToF (Time-of-Flight)920×1080 | 30 fps | 0.3-5m | USB 3.0 | 75° NFOV | ❌ | €200 | Legacy |

### Stereolabs ZED

| Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV (H×V) | IMU | Price (€) | Notes |
|-------|------------|---------------------|-------------------|---------|-------|--------------|-----------|-----|-----------|-------|
| **ZED 2** | Stereo Vision | **2208×1242** | **2208×1242** | **60 fps** | 0.5-20m | USB 3.0 | 110°×70° | ✅ | €450 | **Spatial AI SDK, robust** |
| **ZED 2i** | Stereo Vision | **2208×1242** | **2208×1242** | **60 fps** | 0.5-20m | USB 3.0 | 110°×70° | ✅ | €550 | **Industrial, global shutter** |
| **ZED X** | Stereo Vision | **2208×1242** | **2208×1242** | **120 fps** | 0.5-20m | **USB 3.1 / GMSL2** | 110°×70° | ✅ | €750 | **Highest FPS, GMSL option** |
| ZED Mini | Stereo Vision | **1344×376** | 1344×376 | 60 fps | 0.3-15m | USB 3.0 | 90°×60° | ✅ | €350 | Compact, AR/VR |

**Key Features:**
- Spatial AI SDK with neural depth
-All ZED: Spatial AI SDK, neural depth, positional tracking, object/body detection, works in extreme conditions (60kmph, 45°C)* Microsoft Azure Kinect

| Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV (H×V) | IMU | Price (€) | Notes |
|-------|------------|---------------------|-------------------|---------|-------|--------------|-----------|-----|-----------|-------|
| **Azure Kinect DK** | iToF | **1024×1024** | **3840×2160 (4K)** | 30 fps | 0.5-5.46m | USB 3.0 | 75°/120° NFOV/WFOV | ✅ | €500 | **7 mics, discontinued 2023** |

**Note:** Replaced by Orbbec Femto Bolt/Mega with compatible SDK

---

### Industrial Depth Cameras

| Brand | Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV | Price (€) | Notes |
|-------|-------|------------|---------------------|-------------------|---------|-------|--------------|-----|-----------|-------|
| **Basler** | blaze-101 | iToF | **640×480** | Optional RGB | 30 fps | 0.3-10m | **GigE / USB 3.0** | 71°×55° | €1,000-1,500 | Compact industrial |
|Note: Replaced by Orbbec Femto Bolt/Mega with compatible SDK*

### Industrial

### LiDAR Cameras

| Brand | Model | Type | Points/sec | Max FPS | Range | Connectivity | FOV | Price (€) | Notes |
|-------|-------|------|------------|---------|-------|--------------|-----|-----------|-------|
| **Livox** | Mid-360 | LiDAR | 100K pts/sec | 10 Hz | 0.5-40m | Ethernet | 360°×59° | €500-600 | 360° horizontal |
| **Ouster** | OS0/OS1 | LiDAR | Up to 2048 beams | 10/20 Hz | 0.5-50m | **Ethernet** | 360° | €3,000-15,000 | Professional automotive |
| **Velodyne** | VLP-16 | LiDAR | 16 channels | 5-20 Hz | 100m | **Ethernet** | 360°×30° | €4,000-8,000 | Classic automotive |
| **RoboSense** | RS-LiDAR-M1 | LiDAR | 625K pts/sec | 10 Hz | 200m | Ethernet | 120°×25° | €3,000+ | MEMS solid-state |

### LiDARComparison

| Technology | Depth Accuracy | Range | Outdoor Performance | Low Light | Response Time | Power | Cost | Best Use Case |
|------------|---------------|-------|-------------------|-----------|---------------|-------|------|---------------|
| **Stereo Vision** | cm | Good | ✅ Excellent | ❌ Weak | Medium | Low | 💰 Low | Outdoor robots, navigation |
| **Structured Light** | µm-cm | Limited | ❌ Weak | ✅ Good | Slow | Medium | 💰💰 Medium | Indoor scanning, faces |
| **iToF** | mm-cm | Scalable | ⚠️ Fair | ✅ Good | Very Fast | Medium | 💰💰 Medium | Indoor robots, gesture |
| **dToF/LiDAR** | mm-cm | Scalable | ⚠️ Fair | ✅ Good | Fast | Medium-High | 💰💰💰 High | Precision mapping, long range |

---

## 🔑 Techall Value
1. **OAK-D Pro** ($399) - AI chip + 4K RGB + laser dot + IMU
2. **Orbbec Femto Bolt** (€300-400) - Azure Kinect compatible, ToF
3. **Intel D435i** (€468) - Proven ecosystem, IMU, wide FOV

### 💰 Best Budget
1. **OAK-D Lite** ($150) - Unbeatable AI + 4K RGB
2. **Orbbec Astra 2** (€200-250) - **1600×1200 depth**, Full HD RGB, USB 3.0, IMU
3. **Gemini 2** (€200-250) - USB 3.0, good value

### 🌐 Best PoE (Power over Ethernet)
## 📋 Best By Category

**🏆 Overall Value:** OAK-D Pro ($399) • Femto Bolt (€300-400) • D435i (€468)
**💰 Budget:** OAK-D Lite ($150) • Astra 2 (€200-250, 1600×1200 depth!) • Gemini 2 (€200-250)
### ☀️ Best Outdoor Performance
1. **ZED 2i** - Proven at 60kmph in 45°C heat (Reddit verified)
2. **Intel D455/D455f** - Global shutter, designed for outdoor
3. **Intel D435i** - Wide FOV, good in varied lighting

### 🤖 Best for Robotics/AMR
**Based on Reddit Community (r/robotics):**
1. **ZED 2i** - Most robust, works in extreme conditions
2. **Intel D455** - Reliable, global shutter, good value
3. **Orbbec Femto Bolt** - Great indoors (avoid strong sunlight)
4. **OAK-D Pro** - Built-in AI, good for feature-rich environments

### 📐 Highest Resolution
**Depth:**
1. **ZED 2/2i/X** - 2208×1242 (highest)
2. **Orbbec Astra 2** - 1600×1200 (best structured light)
3. **Lucid Helios2** - 1456×1088
4. **Azure Kinect / Femto Series** - 1024×1024

**RGB:**
1. **Azure Kinect** - 4K (3840×2160)
2. **OAK-D Pro** - 12MP (4K)
3. **ZED 2/2i/X** - 2208×1242

### 🔬 Best Close-Range
1. **Orbbec Gemini 305** - **4cm minimum** (revolutionary!)
2. **Intel D405** - 7cm minimum
3. **Astra Mini Pro** - 35cm minimum

### 🏭 Best Industrial
1. **Intel D555 PoE** (€720) - IP65, PoE, Vision SoC
2. **Intel D457** (€690) - GMSL/FAKRA, IP65, automotive
3. **Zivid Two M130** (€10,000+) - Professional 3D scanning
4. **Basler blaze-101** (€1,000-1,500) - Compact industrial ToF

### 🎨 Best for Creative/TouchDesigner
1. **Orbbec Femto Bolt** (€300-400) - Native SDK, point cloud ready
2. **Intel D455** (€588) - High FPS, excellent SDK
3. **OAK-D Pro** (€399) - Built-in AI, Python SDK
4. **ZED 2** (€450) - Spatial AI SDK

---

## ⚠️ Important Notes from Community (Reddit r/robotics)

### ✅ Recommendations
- **ZED 2i**: "Most robust and reliable depth camera. Works in 45°C heat at 60kmph" ✅
- **Intel D455**: "Global shutter makes it best RealSense for outdoor use" ✅
- **Orbbec Femto Bolt/Mega**: "Much superior to listed options, uses Azure Kinect technology" ✅
- **OAK-D Pro**: "Great when you need onboard AI processing" ✅

### ❌ Avoid
- **Intel D415 for moving robots**: "Rolling shutter causes issues on mobile platforms" ❌
- **Femto Bolt/Mega outdoors**: "Becomes quite bad in strong sunlight" ⚠️
- **OAK-D in low-texture environments**: "Depth can be temperamental without good features" ⚠️

---

## 🔌 Connectivity Summary

### USB 2.0
- Orbbec Astra series (Astra+, Astra Mini Pro, Astra Embedded S)
Community Notes (Reddit r/robotics)
**✅ Recommended:** ZED 2i (60kmph/45°C proven) • D455 (best outdoor) • Femto Bolt/Mega (Azure tech, indoors) • OAK-D Pro (AI onboard)
**❌ Avoid:** D415 (rolling shutter issues on mobile platforms) • Femto outdoors (bad in sunlight) • OAK-D (needs texture-rich environments)*Orbbec Femto Mega / Mega I** ✅
- Zivid Two M130
- Photoneo PhoXi 3D
- Industrial LiDAR (Ouster, Velodyne, etc.)

### GMSL / GMSL2 (Automotive)
- **Intel D457** (GMSL/FAKRA)
- **ZED X** (GMSL2 option)

### GigE (Gigabit Ethernet)
- Basler blaze-101
- Lucid Helios2
- Photoneo PhoXi 3D
- Zivid series
**USB 2.0:** Astra+, Mini Pro, Embedded S
**USB 3.0/3.1:** RealSense (all), OAK (all USB), Astra 2, Gemini/Femto, ZED, Azure Kinect, Basler blaze-101
**PoE:** D555 PoE • OAK-D Pro PoE/OAK-4 • Femto Mega/Mega I • Zivid • Photoneo • Industrial LiDAR
**GMSL/GMSL2:** D457 (GMSL/FAKRA) • ZED X (GMSL2)
**GigE:** Basler, Lucid, Photoneo, Zivid, Industrial camerasest:** Orbbec Femto Bolt (€300-400) - Fast ToF  
**Alternative:** OAK-D Pro ($399) - AI gestures

### Outdoor Mapping / Survey
**Long range:** Ouster/Velodyne LiDAR (€3,000+)  
**Medium range:** ZED X (€750) - 120fps  
**Budget:** D455 (€588)

### Wearable / Drone
**Ultra-light:** Gemini 305 (65g, €300+)  
**Compact:** ZED Mini (€350)  
**AI onboard:** OAK-D Lite ($150)

### Industrial Inspection
**PoE:** D555 PoE (€720) or Basler blaze-101 (€1,000)  
**High precision:** Zivid (€10,000+)  
**Automotive:** D457 GMSL (€690)

### Creative / Art / TouchDesigner
**Best SDK:** Femto Bolt (€300-400) - you have integration!  
**Alternative:** D455 (€588) or OAK-D Pro ($399)  
**Multi-camera:** ZED 2 (€450) - robust

---

## 📦 What's in Your Workspace

Based on your `CKTDOrbbec` project:
- ✅ You have Orbbec SDK v2.6.3 installed
- ✅ You have `pyorbbecsdk` integration for TouchDesigner
- ✅ Your integrGuide
**AMR/AGV:** ZED 2i/D455 (€550-588) • Budget: OAK-D Lite ($150)/Gemini 2 (€200) • Industrial: D555 PoE (€720)
**Outdoor:** ZED 2i (€550) • D455 (€588) • Avoid: Femto (sunlight issues)
**Indoor Robotics:** Femto Bolt (€300-400) • OAK-D Pro ($399) • Astra 2 (€200, 1600×1200!)
**Robotic Arms:** Gemini 305 (€300+, 4cm!) • D405 (€415, 7cm) • Zivid (€10k+, precision)
**3D Scanning:** Zivid (€10k+) • L515 (€450+) • D455 (€588)
**Gesture/HMI:** Femto Bolt (€300-400) • OAK-D Pro ($399)
**Outdoor Mapping:** Ouster/Velodyne (€3k+) • ZED X (€750, 120fps) • D455 (€588)
**Wearable/Drone:** Gemini 305 (65g) • ZED Mini (€350) • OAK-D Lite ($150)
**Industrial:** D555 PoE (€720) • Basler (€1k) • Zivid (€10k+) • D457 GMSL (€690)
**TouchDesigner:** Femto Bolt (€300-400, SDK ready!) • D455 (€588) • OAK-D Pro ($399) • ZED 2 (€450)

## 🎯 Quick Decision Matrix

**Budget < €200:**
→ OAK-D Lite ($150) or Astra 2 (€200)

**Need PoE:**
→ OAK-D Pro PoE ($499) or D555 PoE (€720)

**Need highest FPS:**
→ ZED X (120fps, €750)

**Need outdoor robustness:**
→ ZED 2i (€550) or D455 (€588)

**Need close range (<10cm):**
→ Gemini 305 (4cm, €300+)

**Need highest depth resolution:**
→ ZED series (2208×1242)

**Need highest RGB resolution:**
→ Azure Kinect (4K) or OAK-D Pro (12MP)

**Need onboard AI:**
→ OAK-D Pro ($399) or OAK-4 ($599+)

**Already have TouchDesigner setup:**
→ Orbbec Femto Bolt (€300-400) ✅

**Need industrial/IP65:**
→ D555 PoE (€720) or D457 (€690)

---

## 📞 Your Setup (CKTDOrbbec)
✅ Orbbec SDK v2.6.3 • pyorbbecsdk for TouchDesigner • Supports: Femto/Gemini/Astra
**Recommended:** Femto Bolt (€300-400, SDK ready!) • Femto Mega (€350-450, PoE) • D455 (€588, RealSense SDK)

## 🛒 Where to Buy
**Europe:** Generation Robots (RealSense) • Orbbec Official • Luxonis Shop
**Online:** Amazon (verify seller) • Alibaba (bulk) • Official storesntel RealSense L515 discontinued in 2023
- Azure Kinect DK discontinued in 2023 (replaced by Orbbec Femto)
- Always verify latest specs on manufacturer websites before purchase
Support
**RealSense 2.0:** Python/C++/C#/Node.js • Win/Linux/macOS • ROS/ROS2 • Unity/Unreal
**Orbbec 2.6.3:** Python/C++/C • Win/Linux • ROS/ROS2 • TouchDesigner (your integration!)
**Luxonis DepthAI:** Python/C++ • Win/Linux/macOS/ARM • ROS/ROS2 • PyTorch/TensorFlow/ONNX • Onboard inference
**ZED SDK:** Python/C++/C#/Unity • Win/Linux • ROS/ROS2 • Unity/Unreal • Spatial AI/Neural depth
**<€200:** OAK-D Lite ($150) • Astra 2 (€200, 1600×1200 depth!)
**PoE:** OAK-D Pro PoE ($499) • D555 PoE (€720)
**Max FPS:** ZED X (120fps, €750)
**Outdoor:** ZED 2i (€550) • D455 (€588)
**Close <10cm:** Gemini 305 (4cm, €300+)
**Max Depth Res:** ZED (2208×1242)
**Max RGB Res:** Azure Kinect (4K) • OAK-D Pro (12MP)
**Onboard AI:** OAK-D Pro ($399) • OAK-4 ($599+)
**TouchDesigner ready:** Femto Bolt (€300-400) ✅
**Industrial/IP65:** D555 PoE (€720) • D457 (€690)Support
**Tech:** Intel ([intel.com/realsense](https://www.intel.com/realsense)) • Orbbec (business@orbbec.com) • Luxonis (support@luxonis.com, [forum](https://discuss.luxonis.com/)) • Stereolabs (support@stereolabs.com)
**Community:** Reddit (r/robotics, r/computervision) • ROS Discourse ([discourse.ros.org](https://discourse.ros.org)) • GitHub (official repos)

---
**Document:** CraftKontrol - Arnaud Cassone © Artcraft Visuals | **Verified:** Jan 17, 2026
**Notes:** Prices approximate • Specs from official sources • Reddit feedback 2024-2026 • L515 discontinued 2023 • Azure Kinect discontinued 2023 (replaced by Orbbec Femto) • Always verify latest specs on manufacturer websites