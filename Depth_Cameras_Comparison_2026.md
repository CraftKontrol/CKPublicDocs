# 🎥 Complete Depth Camera Comparison 2026

**Last Updated:** January 17, 2026  
**Sources:** Generation Robots, Reddit r/robotics, Luxonis, e-con Systems, Orbbec

---

## 📊 Complete Specifications Table

### Intel RealSense Series

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

---

### Luxonis OAK Series

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
- Onboard CV/ML pipelines
- Custom DepthAI API
- Support for PyTorch, TensorFlow, ONNX

---

### Orbbec Series

#### Structured Light (Astra Series)

| Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV (H×V) | IMU | Price (€) | Notes |
|-------|------------|---------------------|-------------------|---------|-------|--------------|-----------|-----|-----------|-------|
| **Astra 2** | Structured Light | **640×480** | **1920×1080** | 30 fps | 0.4-8m | USB 2.0 | 60°×49.5° | ❌ | €200-250 | **Current model, Full HD RGB** |
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
| Gemini 335L | Stereo Vision | **640×400** | **1920×1080** | 30 fps | 0.15-5m | USB 3.0 | 67°×45° | ❌ | €260-310 | Long-range variant |
| Gemini 335Lg | Stereo Vision | **640×400** | **1920×1080** | 30 fps | 0.15-5m | USB 3.0 | 67°×45° | ✅ | €280-330 | Long-range + global shutter |
| Gemini 336 | Stereo Vision | **640×400** | **1920×1080** | 30 fps | 0.15-5m | USB 3.0 | 67°×45° | ❌ | €270-320 | Enhanced Gemini 335 |

#### ToF (Time-of-Flight) Series

| Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV (H×V) | IMU | Price (€) | Notes |
|-------|------------|---------------------|-------------------|---------|-------|--------------|-----------|-----|-----------|-------|
| **Femto Bolt** | iToF | **1024×1024** | **1920×1080** | 30 fps | 0.25-5.46m | USB 3.0 | 75°/120° NFOV/WFOV | ✅ | €300-400 | **Azure Kinect compatible SDK** |
| **Femto Mega** | iToF | **1024×1024** | **1920×1080** | 30 fps | 0.4-5.5m | **USB 3.0 / GigE PoE** | 75°/120° NFOV/WFOV | ✅ | €350-450 | **PoE support, dual interface** |
| **Femto Mega I** | iToF | **1024×1024** | **1920×1080** | 30 fps | 0.4-5.5m | USB 3.0 / GigE PoE | 75°/120° NFOV/WFOV | ✅ | €400-500 | Enhanced version |
| Femto W | iToF | **640×576** | 1920×1080 | 30 fps | 0.3-5m | USB 3.0 | 120° WFOV | ❌ | €250 | Legacy, wide FOV |
| Femto | iToF | **640×576** | 1920×1080 | 30 fps | 0.3-5m | USB 3.0 | 75° NFOV | ❌ | €200 | Legacy |

---

### Stereolabs ZED Series

| Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV (H×V) | IMU | Price (€) | Notes |
|-------|------------|---------------------|-------------------|---------|-------|--------------|-----------|-----|-----------|-------|
| **ZED 2** | Stereo Vision | **2208×1242** | **2208×1242** | **60 fps** | 0.5-20m | USB 3.0 | 110°×70° | ✅ | €450 | **Spatial AI SDK, robust** |
| **ZED 2i** | Stereo Vision | **2208×1242** | **2208×1242** | **60 fps** | 0.5-20m | USB 3.0 | 110°×70° | ✅ | €550 | **Industrial, global shutter** |
| **ZED X** | Stereo Vision | **2208×1242** | **2208×1242** | **120 fps** | 0.5-20m | **USB 3.1 / GMSL2** | 110°×70° | ✅ | €750 | **Highest FPS, GMSL option** |
| ZED Mini | Stereo Vision | **1344×376** | 1344×376 | 60 fps | 0.3-15m | USB 3.0 | 90°×60° | ✅ | €350 | Compact, AR/VR |

**Key Features:**
- Spatial AI SDK with neural depth
- Positional tracking
- Object detection
- Body tracking
- Works in extreme conditions (tested at 60kmph, 45°C)

---

### Microsoft Azure Kinect

| Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV (H×V) | IMU | Price (€) | Notes |
|-------|------------|---------------------|-------------------|---------|-------|--------------|-----------|-----|-----------|-------|
| **Azure Kinect DK** | iToF | **1024×1024** | **3840×2160 (4K)** | 30 fps | 0.5-5.46m | USB 3.0 | 75°/120° NFOV/WFOV | ✅ | €500 | **7 mics, discontinued 2023** |

**Note:** Replaced by Orbbec Femto Bolt/Mega with compatible SDK

---

### Industrial Depth Cameras

| Brand | Model | Technology | Max Depth Resolution | Max RGB Resolution | Max FPS | Range | Connectivity | FOV | Price (€) | Notes |
|-------|-------|------------|---------------------|-------------------|---------|-------|--------------|-----|-----------|-------|
| **Basler** | blaze-101 | iToF | **640×480** | Optional RGB | 30 fps | 0.3-10m | **GigE / USB 3.0** | 71°×55° | €1,000-1,500 | Compact industrial |
| **Lucid** | Helios2 | iToF | **1456×1088** | N/A | 24 fps | 0.3-10m | **GigE / USB 3.1** | Varies | €1,500-3,000 | Sony DepthSense, industrial |
| **Photoneo** | PhoXi 3D M | Structured Light | **1032×772** | N/A | 15 fps | 0.2-3m | **GigE** | Varies | €5,000+ | Industrial inspection |
| **Zivid** | Two M130 | Structured Light | **1920×1200** | **1920×1200** | 10 fps | 0.3-1.3m | **GigE PoE** | 43°×33° | €10,000+ | Professional 3D scanning |

---

### LiDAR Cameras

| Brand | Model | Type | Points/sec | Max FPS | Range | Connectivity | FOV | Price (€) | Notes |
|-------|-------|------|------------|---------|-------|--------------|-----|-----------|-------|
| **Livox** | Mid-360 | LiDAR | 100K pts/sec | 10 Hz | 0.5-40m | Ethernet | 360°×59° | €500-600 | 360° horizontal |
| **Ouster** | OS0/OS1 | LiDAR | Up to 2048 beams | 10/20 Hz | 0.5-50m | **Ethernet** | 360° | €3,000-15,000 | Professional automotive |
| **Velodyne** | VLP-16 | LiDAR | 16 channels | 5-20 Hz | 100m | **Ethernet** | 360°×30° | €4,000-8,000 | Classic automotive |
| **RoboSense** | RS-LiDAR-M1 | LiDAR | 625K pts/sec | 10 Hz | 200m | Ethernet | 120°×25° | €3,000+ | MEMS solid-state |

---

## 🔑 Technology Comparison

| Technology | Depth Accuracy | Range | Outdoor Performance | Low Light | Response Time | Power | Cost | Best Use Case |
|------------|---------------|-------|-------------------|-----------|---------------|-------|------|---------------|
| **Stereo Vision** | cm | Good | ✅ Excellent | ❌ Weak | Medium | Low | 💰 Low | Outdoor robots, navigation |
| **Structured Light** | µm-cm | Limited | ❌ Weak | ✅ Good | Slow | Medium | 💰💰 Medium | Indoor scanning, faces |
| **iToF** | mm-cm | Scalable | ⚠️ Fair | ✅ Good | Very Fast | Medium | 💰💰 Medium | Indoor robots, gesture |
| **dToF/LiDAR** | mm-cm | Scalable | ⚠️ Fair | ✅ Good | Fast | Medium-High | 💰💰💰 High | Precision mapping, long range |

---

## 📋 Best By Category

### 🏆 Best Overall Value
1. **OAK-D Pro** ($399) - AI chip + 4K RGB + laser dot + IMU
2. **Orbbec Femto Bolt** (€300-400) - Azure Kinect compatible, ToF
3. **Intel D435i** (€468) - Proven ecosystem, IMU, wide FOV

### 💰 Best Budget
1. **OAK-D Lite** ($150) - Unbeatable AI + 4K RGB
2. **Orbbec Astra 2** (€200-250) - Full HD RGB, USB 2.0
3. **Gemini 2** (€200-250) - USB 3.0, good value

### 🌐 Best PoE (Power over Ethernet)
1. **Intel D555 PoE** (€720) - Vision SoC V5, IP65, industrial-grade
2. **OAK-D Pro PoE** ($499) - 48 TOPS AI, no USB needed
3. **Orbbec Femto Mega** (€350-450) - Dual interface (USB/PoE)
4. **Zivid Two M130** (€10,000+) - Professional 3D scanning

### 🚀 Highest FPS
1. **ZED X** - 120 fps (stereo depth)
2. **Intel D455/D435i/D415** - 90 fps (stereo depth)
3. **OAK-D Series** - 60 fps (stereo depth + AI)

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
2. **Lucid Helios2** - 1456×1088
3. **Azure Kinect / Femto Series** - 1024×1024

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
- Orbbec Astra series (2, +, Mini Pro, Embedded S)

### USB 3.0 / 3.1 Type-C
- Intel RealSense (D405, D415, D435, D435i, D435if, D455, D455f, D456, L515)
- Luxonis OAK series (all USB models)
- Orbbec Gemini series, Femto series (USB models)
- Stereolabs ZED (2, 2i, Mini)
- Azure Kinect DK
- Basler blaze-101 (dual)

### PoE (Power over Ethernet)
- **Intel D555 PoE** ✅
- **Luxonis OAK-D Pro PoE, OAK-4** ✅
- **Orbbec Femto Mega / Mega I** ✅
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
- Industrial cameras

---

## 💡 Use Case Recommendations

### Mobile Robots (AMR/AGV)
**Primary:** ZED 2i (€550) or Intel D455 (€588)  
**Budget:** OAK-D Lite ($150) or Gemini 2 (€200)  
**Industrial:** D555 PoE (€720)

### Outdoor Vehicles
**Best:** ZED 2i (€550) - proven at 60kmph  
**Alternative:** Intel D455 (€588) - global shutter  
**Avoid:** Femto series in direct sunlight

### Indoor Robotics
**Best:** Orbbec Femto Bolt (€300-400) - ToF, fast  
**Alternative:** OAK-D Pro ($399) - AI onboard  
**Budget:** Astra 2 (€200) or OAK-D Lite ($150)

### Robotic Arms / Pick & Place
**Close range:** Gemini 305 (€300+) - 4cm minimum  
**Medium range:** D405 (€415) - 7cm minimum  
**Precision:** Zivid Two M130 (€10,000+)

### 3D Scanning / Metrology
**Professional:** Zivid Two M130 (€10,000+)  
**Mid-range:** Intel L515 (€450+) - LiDAR  
**Budget:** D455 (€588) + post-processing

### Gesture Recognition / HMI
**Best:** Orbbec Femto Bolt (€300-400) - Fast ToF  
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
- ✅ Your integration supports: Femto series, Gemini series, Astra series

**Recommended for your workflow:**
1. **Orbbec Femto Bolt** (€300-400) - Already have SDK integration!
2. **Orbbec Femto Mega** (€350-450) - Same SDK + PoE option
3. **Intel D455** (€588) - High FPS alternative with RealSense SDK

---

## 🛒 Where to Buy

### Europe
- **Generation Robots** (France) - RealSense specialist
- **Orbbec Official** - Direct from manufacturer
- **Luxonis Shop** - Direct OAK cameras

### Online
- Amazon (verify seller)
- Alibaba (bulk/OEM)
- Official manufacturer stores

---

## 📚 SDK & Software Support

### Intel RealSense SDK 2.0
- Languages: Python, C++, C#, Node.js
- Platforms: Windows, Linux, macOS
- ROS/ROS2: ✅ Full support
- Unity/Unreal: ✅

### Orbbec SDK 2.6.3
- Languages: Python, C++, C
- Platforms: Windows, Linux
- ROS/ROS2: ✅ Support
- TouchDesigner: ✅ (your integration)

### Luxonis DepthAI
- Languages: Python, C++
- Platforms: Windows, Linux, macOS, ARM
- ROS/ROS2: ✅ Support
- ML Frameworks: PyTorch, TensorFlow, ONNX
- Edge AI: ✅ Onboard inference

### Stereolabs ZED SDK
- Languages: Python, C++, C#, Unity
- Platforms: Windows, Linux
- ROS/ROS2: ✅ Full support
- Unity/Unreal: ✅
- AI: Spatial AI, Neural depth

---

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

## 📞 Contact Information

### Technical Support
- **Intel RealSense**: [Intel Support](https://www.intel.com/realsense)
- **Orbbec**: business@orbbec.com
- **Luxonis**: support@luxonis.com, [Forum](https://discuss.luxonis.com/)
- **Stereolabs**: support@stereolabs.com

### Community
- **Reddit**: r/robotics, r/computervision
- **ROS Discourse**: [discourse.ros.org](https://discourse.ros.org)
- **GitHub**: Each manufacturer has official repos

---

**Document prepared by:** CraftKontrol - Arnaud Cassone / Artcraft Visuals  
**Sources verified:** January 17, 2026  
**Next update:** Check manufacturer websites for latest models

---

## 📝 Notes

- Prices are approximate and vary by region/distributor
- All specifications verified from official sources and retailer listings
- Community feedback from Reddit r/robotics (2024-2026)
- Intel RealSense L515 discontinued in 2023
- Azure Kinect DK discontinued in 2023 (replaced by Orbbec Femto)
- Always verify latest specs on manufacturer websites before purchase
