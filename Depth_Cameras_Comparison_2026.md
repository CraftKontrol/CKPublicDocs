# Depth Camera Comparison 2026
**Updated:** Jan 17, 2026 | **Author:** Arnaud Cassone © Artcraft Visuals


Comprehensive comparison of depth cameras for robotics and computer vision applications.

## Complete Comparison - All Cameras
*Sorted by: Depth Resolution → Connectivity (Ethernet first) → Price*

| Model | Depth Resolution | Color Resolution | FPS | Range | FOV | Stereo | Connectivity | Price | Usage | Provider | TD Compatible |
|-------|-----------------|------------------|-----|-------|-----|--------|--------------|-------|-------|----------|---------------|
| [ZED 2](https://www.stereolabs.com/en-fr/products/zed-2) | 2208x1242 (2.7MP) | 4416x2484 (4K) | 15/30/60 | 0.2-20m | H110° V70° | Yes (Stereo) | USB 3.0 | ~$400-600 | General robotics | Stereolabs | Community support |
| [ZED X](https://www.stereolabs.com/en-fr/products/zed-x) | 1920x1200 (2.3MP) | 1920x1200 GS or 3840x2160 4K HDR | 15/30/60 | 1-20m | N:H80° V52° W:H110° V80° | Yes (Stereo) | GMSL2 | ~$600-900 | Industrial robotics | Stereolabs | Community support |
| [ZED X One](https://www.stereolabs.com/en-fr/products/zed-x-one) | 1920x1200 (2.3MP) | 1920x1200 GS @60 or 3840x2160 4K @15 | 15/30/60/120 | Custom | N:H80° V52° W:H110° V80° F:H195° V115° | Monocular/Custom | GMSL2/MIPI | €280-€380 | Multi-camera systems | Stereolabs | Community support |
| [OAK 4 D](https://shop.luxonis.com/products/oak-4-d?variant=46428694446303) | 1920x1200 | 48MP | 60 depth | 0.7-12m | H110° V80° | Yes | USB3 & PoE | $849 | Advanced edge AI | Luxonis | Community support |
| [Astra 2](https://www.orbbec.com/products/structured-light-camera/astra-2/) | 1600x1200 | 1920x1080 | 30 | 0.6-8m | H58° V45° | No (Structured Light) | USB 3.0 Type-C | ~$200-300 | Indoor scanning | Orbbec | Yes (SDK available) |
| [Gemini 435LE](https://www.orbbec.com/gemini-435le/) | High density | 1920x1080 | 30 | 0.3-20m | H90° V65° | Yes (Stereo) | Ethernet PoE | ~$400-500 | Long-range industrial | Orbbec | Yes (SDK available) |
| [Gemini 345LG](https://www.orbbec.com/gemini-345lg/) | 1280x960 | 1920x1080 | 30 | 0.3-10m | W:H104° V87° S:H91° V78° | Yes (Stereo) | GMSL2/USB 3.0 | ~$400-500 | Outdoor robotics | Orbbec | Yes (SDK available) |
| [Gemini 335LE](https://www.orbbec.com/gemini-335le/) | 1280x800 | 1920x1080 | 30 | 0.26-3m | H90° V65° | Yes (Active/Passive) | Ethernet PoE | ~$300-400 | Industrial AMR | Orbbec | Yes (SDK available) |
| [OAK-D W PoE](https://shop.luxonis.com/products/oak-d-w-poe?variant=44043279302879) | 1280x800 | 4K@30, 1080p@60 (12MP IMX378) | 30 depth, 60 RGB | 0.4-6m | H150° (stereo) H120° (RGB) | Yes | Ethernet PoE | $549 | Wide FOV robotics | Luxonis | Community support |
| [Femto Mega I](https://www.orbbec.com/products/tof-camera/femto-mega-i/) | 1024x1024@15, 640x576@30 | 3840x2160@25 | 10-30 | 0.25-5.46m | W:H120° V120° N:H75° V65° | No (ToF) | Ethernet M12 PoE | ~$700-900 | Industrial IP65 | Orbbec | Yes (SDK available) |
| [Femto Mega](https://www.orbbec.com/products/tof-camera/femto-mega/) | 1024x1024@15, 640x576@30 | 3840x2160@25 | 15-30 | 0.25-5.46m | W:H120° V120° N:H75° V65° | No (ToF) | USB 3.0/Ethernet PoE | ~$500-600 | Industrial w/ Jetson Nano | Orbbec | Yes (SDK available) |
| [D457](https://www.intel.fr/content/www/fr/fr/products/sku/230571/intel-realsense-depth-camera-d457/specifications.html) | 1280x720 | RGB supported | up to 90 | 0.6-6m | H87° V58° | Yes (Stereo) | GMSL/FAKRA | N/A | Automotive/industrial | Intel | Yes |
| [D456](https://www.intel.fr/content/www/fr/fr/products/sku/236331/intel-realsense-depth-camera-d456/specifications.html) | 1280x720 | RGB supported | up to 90 | 0.6-6m | H86° V57° | Yes (Stereo) | USB 3.1 | N/A | General purpose | Intel | Yes |
| [D455F](https://www.intel.fr/content/www/fr/fr/products/sku/233193/intel-realsense-depth-camera-d455f/specifications.html) | 1280x720 | RGB supported | up to 90 | 0.6-6m | H86° V57° | Yes (Stereo) | USB 3.1 | N/A | General purpose | Intel | Yes |
| [D435iF](https://www.intel.fr/content/www/fr/fr/products/sku/233194/intel-realsense-depth-camera-d435if/specifications.html) | 1280x720 | RGB supported | N/A | 0.3-3m | H87° V58° | Yes (Active Stereo) | USB 3 Type-C | N/A | Short/mid-range | Intel | Yes |
| [Gemini 335](https://www.orbbec.com/products/stereo-vision-camera/gemini-335/) | 1280x800 | 1920x1080 | 30 | 0.26-3m | H90° V65° | Yes (Active/Passive) | USB 3.0 Type-C | ~$200-300 | AMR, robotics | Orbbec | Yes (SDK available) |
| [Gemini 215](https://www.orbbec.com/products/stereo-vision-camera/gemini-215/) | 1280x800 | 1920x1080 | 30 | 0.15-0.7m | H63° V46° | Yes (Active Stereo) | USB 3.0 | ~$150-250 | Short-range scanning | Orbbec | Yes (SDK available) |
| [OAK-D W](https://shop.luxonis.com/products/oak-d-w?variant=43905772519647) | 1280x800 | 4K@30, 1080p@60 (12MP IMX378) | 30 depth, 60 RGB | 0.4-6m | H150° (stereo) H120° (RGB) | Yes | USB-C | $399 | Wide FOV robotics | Luxonis | Community support |
| [Femto Bolt](https://www.orbbec.com/products/tof-camera/femto-bolt/) | 1024x1024@15, 640x576@30 | 3840x2160@30 | 15-30 | 0.25-5.46m | W:H120° V120° N:H75° V65° | No (ToF) | USB 3.2 Type-C | ~$400-500 | Azure Kinect replacement | Orbbec | Yes (SDK available) |
| [Azure Kinect DK](https://azure.microsoft.com/fr-fr/products/kinect-dk) | 1024x1024@15, 640x576@30 | 3840x2160 (12MP) | 15-30 | 0.25-5.46m | W:H120° V120° N:H75° V65° | No (ToF) | USB 3 | ~$400 (discontinued) | Body tracking, spatial AI | Microsoft | Yes (legacy support) |
| [Astra Series](https://www.orbbec.com/products/structured-light-camera/astra-series/) | 640x480 | 640x480 or 1920x1080 | 30 | 0.4-8m | H58° V46° | No (Structured Light) | USB 2.0 Type-A | ~$100-200 | Budget indoor | Orbbec | Yes (OpenNI SDK) |

---

## Detailed Specifications by Manufacturer

### Intel RealSense Series

| Model | Depth Resolution | Color Resolution | FPS | Range | FOV | Stereo | Connectivity | Price | Usage | Provider | TD Compatible |
|-------|-----------------|------------------|-----|-------|-----|--------|--------------|-------|-------|----------|---------------|
| [D456](https://www.intel.fr/content/www/fr/fr/products/sku/236331/intel-realsense-depth-camera-d456/specifications.html) | 1280x720 | RGB supported | up to 90 | 0.6m - 6m | H86° V57° | Yes (Stereo) | USB 3.1 | N/A | General purpose | Intel | Yes |
| [D455F](https://www.intel.fr/content/www/fr/fr/products/sku/233193/intel-realsense-depth-camera-d455f/specifications.html) | 1280x720 | RGB supported | up to 90 | 0.6m - 6m | H86° V57° | Yes (Stereo) | USB 3.1 | N/A | General purpose | Intel | Yes |
| [D435iF](https://www.intel.fr/content/www/fr/fr/products/sku/233194/intel-realsense-depth-camera-d435if/specifications.html) | 1280x720 | RGB supported | N/A | 0.3m - 3m | H87° V58° | Yes (Active Stereo) | USB 3 Type-C | N/A | Short/mid-range | Intel | Yes |
| [D457](https://www.intel.fr/content/www/fr/fr/products/sku/230571/intel-realsense-depth-camera-d457/specifications.html) | 1280x720 | RGB supported | up to 90 | 0.6m - 6m | H87° V58° ±3 | Yes (Stereo) | GMSL/FAKRA | N/A | Automotive/industrial | Intel | Yes |

## Luxonis OAK Series

| Model | Depth Resolution | Color Resolution | FPS | Range | FOV | Stereo | Connectivity | Price | Usage | Provider | TD Compatible |
|-------|-----------------|------------------|-----|-------|-----|--------|--------------|-------|-------|----------|---------------|
| [OAK-D W PoE](https://shop.luxonis.com/products/oak-d-w-poe?variant=44043279302879) | 1280x800 | 4K@30, 1080p@60 (12MP IMX378) | 30 depth, 60 RGB | 0.4m - 6m | Stereo: H150° V?, RGB: H120° | Yes | Ethernet PoE | $549 | Wide FOV robotics | Luxonis | Community support |
| [OAK-D W](https://shop.luxonis.com/products/oak-d-w?variant=43905772519647) | 1280x800 | 4K@30, 1080p@60 (12MP IMX378) | 30 depth, 60 RGB | 0.4m - 6m | Stereo: H150° V?, RGB: H120° | Yes | USB-C | $399 | Wide FOV robotics | Luxonis | Community support |
| [OAK 4 D](https://shop.luxonis.com/products/oak-4-d?variant=46428694446303) | 1920x1200 | 48MP | 60 depth | 0.7m - 12m | Baseline: 75mm | Yes | USB3 & PoE | $849 | Advanced edge AI | Luxonis | Community support |

## Orbbec Gemini Series (Stereo Vision)

| Model | Depth Resolution | Color Resolution | FPS | Range | FOV | Stereo | Connectivity | Price | Usage | Provider | TD Compatible |
|-------|-----------------|------------------|-----|-------|-----|--------|--------------|-------|-------|----------|---------------|
| [Gemini 335](https://www.orbbec.com/products/stereo-vision-camera/gemini-335/) | 1280x800 | 1920x1080 | 30 | 0.10-20m+ (optimal: 0.26-3m) | Depth: H90° V65°, RGB: H86° V55° | Yes (Active/Passive) | USB 3.0 Type-C | ~$200-300 | AMR, robotics | Orbbec | Yes (SDK available) |
| [Gemini 335LE](https://www.orbbec.com/gemini-335le/) | 1280x800 | 1920x1080 | 30 | 0.26-3m optimal | Depth: H90° V65°, RGB: H86° V55° | Yes (Active/Passive) | Ethernet PoE | ~$300-400 | Industrial AMR | Orbbec | Yes (SDK available) |
| [Gemini 345LG](https://www.orbbec.com/gemini-345lg/) | 1280x960 | 1920x1080 | 30 | 0.3-10m (ideal: 0.3-6m) | Wide: H104° V87°, Standard: H91° V78° | Yes (Stereo) | GMSL2/USB 3.0 | ~$400-500 | Outdoor robotics | Orbbec | Yes (SDK available) |
| [Gemini 435LE](https://www.orbbec.com/gemini-435le/) | High density | 1920x1080 | 30 | Up to 20m | N/A | Yes (Stereo) | Ethernet PoE | ~$400-500 | Long-range industrial | Orbbec | Yes (SDK available) |
| [Gemini 215](https://www.orbbec.com/products/stereo-vision-camera/gemini-215/) | 1280x800 | 1920x1080 | 30 | 0.15-0.70m (ideal: 0.2-0.5m) | H63.5° V45.6° | Yes (Active Stereo) | USB 3.0 | ~$150-250 | Short-range scanning | Orbbec | Yes (SDK available) |

## Orbbec Femto Series (ToF)

| Model | Depth Resolution | Color Resolution | FPS | Range | FOV | Stereo | Connectivity | Price | Usage | Provider | TD Compatible |
|-------|-----------------|------------------|-----|-------|-----|--------|--------------|-------|-------|----------|---------------|
| [Femto Bolt](https://www.orbbec.com/products/tof-camera/femto-bolt/) | 1024x1024@15, 640x576@30 | 3840x2160@30 | 15-30 | 0.25-5.46m | WFOV: H120° V120°, NFOV: H75° V65° | No (ToF) | USB 3.2 Type-C | ~$400-500 | Azure Kinect replacement | Orbbec | Yes (SDK available) |
| [Femto Mega](https://www.orbbec.com/products/tof-camera/femto-mega/) | 1024x1024@15, 640x576@30 | 3840x2160@25 | 15-30 | 0.25-5.46m | WFOV: H120° V120°, NFOV: H75° V65° | No (ToF) | USB 3.0/Ethernet PoE | ~$500-600 | Industrial w/ Jetson Nano | Orbbec | Yes (SDK available) |
| [Femto Mega I](https://www.orbbec.com/products/tof-camera/femto-mega-i/) | 1024x1024@15, 640x576@30 | 3840x2160@25 | 10-30 | 0.25-5.46m | WFOV: H120° V120°, NFOV: H75° V65° | No (ToF) | Ethernet M12 PoE | ~$700-900 | Industrial IP65 | Orbbec | Yes (SDK available) |

## Orbbec Astra Series (Structured Light)

| Model | Depth Resolution | Color Resolution | FPS | Range | FOV | Stereo | Connectivity | Price | Usage | Provider | TD Compatible |
|-------|-----------------|------------------|-----|-------|-----|--------|--------------|-------|-------|----------|---------------|
| [Astra Series](https://www.orbbec.com/products/structured-light-camera/astra-series/) | 640x480 | 640x480 or 1920x1080 | 30 | 0.6-8m (S: 0.4-2m) | H58.4° V45.5° | No (Structured Light) | USB 2.0 Type-A | ~$100-200 | Budget indoor | Orbbec | Yes (OpenNI SDK) |
| [Astra 2](https://www.orbbec.com/products/structured-light-camera/astra-2/) | 1600x1200 | 1920x1080 | 30 | 0.6-8m | H58.2° V45.2° | No (Structured Light) | USB 3.0 Type-C | ~$200-300 | Indoor scanning | Orbbec | Yes (SDK available) |

## Stereolabs ZED Series

| Model | Depth Resolution | Color Resolution | FPS | Range | FOV | Stereo | Connectivity | Price | Usage | Provider | TD Compatible |
|-------|-----------------|------------------|-----|-------|-----|--------|--------------|-------|-------|----------|---------------|
| [ZED X](https://www.stereolabs.com/en-fr/products/zed-x) | 1920x1200 (2.3MP) | 1920x1200 GS or 3840x2160 4K HDR | 15/30/60 | Long range | GS Narrow: H80° V52°, Wide: H110° V80° | Yes (Stereo) | GMSL2 | ~$600-900 | Industrial robotics | Stereolabs | Community support |
| [ZED X One](https://www.stereolabs.com/en-fr/products/zed-x-one) | 1920x1200 (2.3MP) | 1920x1200 GS @60 or 3840x2160 4K @15 | 15/30/60/120 | Custom baseline | Narrow: H80° V52°, Wide: H110° V80°, Fisheye: H195° V115° | Monocular/Custom | GMSL2/MIPI | €280-€380 | Multi-camera systems | Stereolabs | Community support |
| [ZED 2](https://www.stereolabs.com/en-fr/products/zed-2) | 2208x1242 (2.7MP) | 4416x2484 (4K) | 15/30/60 | 0.2m - 20m | H110° V70° | Yes (Stereo) | USB 3.0 | ~$400-600 | General robotics | Stereolabs | Community support |

## Microsoft Azure Kinect

| Model | Depth Resolution | Color Resolution | FPS | Range | FOV | Stereo | Connectivity | Price | Usage | Provider | TD Compatible |
|-------|-----------------|------------------|-----|-------|-----|--------|--------------|-------|-------|----------|---------------|
| [Azure Kinect DK](https://azure.microsoft.com/fr-fr/products/kinect-dk) | 1024x1024@15, 640x576@30 | 3840x2160 (12MP) | 15-30 | 0.25-5.46m | WFOV: H120° V120°, NFOV: H75° V65° | No (ToF) | USB 3 | ~$400 (discontinued) | Body tracking, spatial AI | Microsoft | Yes (legacy support) |

---

## Key Features Summary

### Technology Types
- **Stereo Vision**: Intel RealSense, Orbbec Gemini, Luxonis OAK, Stereolabs ZED
- **Time of Flight (ToF)**: Orbbec Femto, Azure Kinect
- **Structured Light**: Orbbec Astra

### Connectivity Options
- **USB-C/USB 3.0**: Most models for plug-and-play
- **Ethernet PoE**: Industrial models (Gemini 335LE, 435LE, Femto Mega I, OAK-D W PoE)
- **GMSL2**: Automotive/industrial (D457, Gemini 345LG, ZED X series)

### Price Ranges
- **Budget** ($100-200): Astra Series
- **Mid-range** ($200-400): Gemini 335, OAK-D W, D-series
- **Premium** ($400-900): Femto series, ZED X, OAK 4 D

### TouchDesigner Compatibility
- **Native Support**: Intel RealSense, Orbbec (via SDK)
- **Community Support**: Luxonis OAK, Stereolabs ZED
- **Legacy Support**: Azure Kinect

### Best Use Cases
- **AMR/Robotics**: Gemini 335/335LE, OAK-D W, ZED X
- **Outdoor/Industrial**: Gemini 345LG, 435LE, Femto Mega I, D457
- **Body Tracking**: Azure Kinect, Femto Bolt
- **Wide FOV**: OAK-D W (150°), Femto WFOV (120°)
- **Long Range**: Gemini 435LE (up to 20m), ZED X
- **Short Range/Scanning**: Gemini 215 (0.15-0.7m)

---

*Last updated: January 2026*
*Prices are approximate and may vary by region and distributor*
