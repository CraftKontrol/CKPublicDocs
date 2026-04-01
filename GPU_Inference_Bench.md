# GPU Diffusion Inference Benchmark 2026
**Updated:** April 1, 2026 | **Author:** Arnaud Cassone © Artcraft Visuals


Comprehensive comparison of Nvidia GPUs for diffusion model inference (Stable Diffusion 1.5 / SDXL / FLUX), covering consumer GeForce and professional RTX (ex-Quadro) series.


## Top Picks:
- **Maximum raw performance** — RTX 5090 (32GB GDDR7, native FP4, #1 content creation score)
- **Best value high-end** — RTX 4090 (24GB, proven, dominant TensorRT performance)
- **Professional / ECC / large VRAM** — RTX 6000 Ada (48GB ECC, vGPU-ready, comparable SD speed to RTX 4090)
- **Mid-range sweet spot** — RTX 4080 Super (16GB, strong TensorRT gains, ~$999)
- **Budget / large VRAM** — RTX 4060 Ti 16GB (16GB VRAM at entry price, good for SDXL)

## To evaluate:
- RTX 5090 with FP4 via TensorRT (Nvidia claims up to 3× RTX 4090 for AI workloads with FP4)
- Multi-card NVLink on pro RTX (RTX 6000 Ada supports NVLink for 96GB VRAM pool — not available on GeForce)
- RTX PRO 6000 Blackwell (announced 2025, 96GB next-gen pro GPU — not yet broadly available)

## Key factors for diffusion inference:
- **VRAM** : 8GB minimum for SD 1.5, 16–24GB for SDXL/FLUX fp16, 48GB for full fp32 batch / large models
- **Memory Bandwidth** : Directly drives denoising step throughput
- **Tensor Cores** : FP8 (Ada/Ampere) or FP4+FP8 (Blackwell) — critical for TensorRT acceleration
- **CUDA / TensorRT ecosystem** : Nvidia-exclusive; massive software advantage over AMD
- **ECC memory** : Pro cards only — required for unattended production use

## Software implementations (Puget Systems SD benchmark, July 2023):
- **Automatic1111 + xFormers** — NVIDIA-optimized, highest baseline for RTX cards
- **TensorRT extension** — avg 2.75× over base A1111, ~2× over xFormers (RTX 4090: ~57 it/s with TensorRT)
- **SHARK** — AMD-preferred; RTX cards run ~30% slower on SHARK than A1111


---


## Complete Comparison — All GPUs
*Sorted by: Performance Tier → VRAM | Tom's HW score: composite content creation (SD 1.5/XL + Blender + MLPerf + SPECworkstation), relative to RTX 5090 = 100%*

| <sub><sup>Model</sup></sub> | <sub><sup>Series</sup></sub> | <sub><sup>VRAM</sup></sub> | <sub><sup>Mem BW</sup></sub> | <sub><sup>FP32 TF</sup></sub> | <sub><sup>Tensor Perf</sup></sub> | <sub><sup>TDP</sup></sub> | <sub><sup>MSRP</sup></sub> | <sub><sup>TH Content Creation %</sup></sub> | <sub><sup>SD A1111+xF (it/s)</sup></sub> | <sub><sup>Best use</sup></sub> |
|-------|--------|------|--------|--------|-----------|-----|------|---------|--------|--------|
| <sub><sup>[RTX 5090](https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5090/)</sup></sub> | <sub><sup>Blackwell GB202</sup></sub> | <sub><sup>32GB GDDR7</sup></sub> | <sub><sup>1792 GB/s</sup></sub> | <sub><sup>104.8 TF</sup></sub> | <sub><sup>FP16: 838 TF / FP4: 3352 TF</sup></sub> | <sub><sup>575W</sup></sub> | <sub><sup>$1,999</sup></sub> | <sub><sup>**100%** (862.8)</sup></sub> | <sub><sup>N/A *</sup></sub> | <sub><sup>Maximum throughput, large batch, FP4 TensorRT</sup></sub> |
| <sub><sup>[RTX 4090](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4090/)</sup></sub> | <sub><sup>Ada AD102</sup></sub> | <sub><sup>24GB GDDR6X</sup></sub> | <sub><sup>1008 GB/s</sup></sub> | <sub><sup>82.6 TF</sup></sub> | <sub><sup>FP16: 661 TF / FP8: 1321 TF</sup></sub> | <sub><sup>450W</sup></sub> | <sub><sup>$1,599</sup></sub> | <sub><sup>**78.9%** (681.0)</sup></sub> | <sub><sup>21.04 it/s</sup></sub> | <sub><sup>Best proven single-card for diffusion, TensorRT king</sup></sub> |
| <sub><sup>[RTX 5080](https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5080/)</sup></sub> | <sub><sup>Blackwell GB203</sup></sub> | <sub><sup>16GB GDDR7</sup></sub> | <sub><sup>690 GB/s</sup></sub> | <sub><sup>~56 TF</sup></sub> | <sub><sup>FP4 support</sup></sub> | <sub><sup>360W</sup></sub> | <sub><sup>$999</sup></sub> | <sub><sup>**69.8%** (601.9)</sup></sub> | <sub><sup>N/A *</sup></sub> | <sub><sup>Current-gen, good SDXL, limited VRAM at 16GB</sup></sub> |
| <sub><sup>[RTX 4080 Super](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4080-super/)</sup></sub> | <sub><sup>Ada AD103</sup></sub> | <sub><sup>16GB GDDR6X</sup></sub> | <sub><sup>736 GB/s</sup></sub> | <sub><sup>~52 TF</sup></sub> | <sub><sup>FP8 support</sup></sub> | <sub><sup>320W</sup></sub> | <sub><sup>$999</sup></sub> | <sub><sup>**65.6%** (565.7)</sup></sub> | <sub><sup>~19–20 it/s †</sup></sub> | <sub><sup>Best value at $999 tier, proven TensorRT</sup></sub> |
| <sub><sup>[RTX 4080](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4080/)</sup></sub> | <sub><sup>Ada AD103</sup></sub> | <sub><sup>16GB GDDR6X</sup></sub> | <sub><sup>717 GB/s</sup></sub> | <sub><sup>~49 TF</sup></sub> | <sub><sup>FP8 support</sup></sub> | <sub><sup>320W</sup></sub> | <sub><sup>$1,199</sup></sub> | <sub><sup>**63.5%** (547.8)</sup></sub> | <sub><sup>19.41 it/s</sup></sub> | <sub><sup>Solid 16GB Ada, strong TensorRT gains (~2.6× base)</sup></sub> |
| <sub><sup>RTX 6000 Ada</sup></sub> | <sub><sup>Ada AD102 Pro</sup></sub> | <sub><sup>48GB GDDR6 ECC</sup></sub> | <sub><sup>960 GB/s</sup></sub> | <sub><sup>91.1 TF</sup></sub> | <sub><sup>FP8: 1457 AI TOPS</sup></sub> | <sub><sup>300W</sup></sub> | <sub><sup>~$6,800</sup></sub> | <sub><sup>N/A ‡</sup></sub> | <sub><sup>**21.11 it/s**</sup></sub> | <sub><sup>Pro / large model / no VRAM limit / ECC / vGPU</sup></sub> |
| <sub><sup>[RTX 5070 Ti](https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5070-ti/)</sup></sub> | <sub><sup>Blackwell GB203</sup></sub> | <sub><sup>16GB GDDR7</sup></sub> | <sub><sup>896 GB/s</sup></sub> | <sub><sup>~44 TF</sup></sub> | <sub><sup>FP4 support</sup></sub> | <sub><sup>300W</sup></sub> | <sub><sup>$749</sup></sub> | <sub><sup>**63.4%** (547.3)</sup></sub> | <sub><sup>N/A *</sup></sub> | <sub><sup>Current-gen mid-high, good BW at lower TDP than 5080</sup></sub> |
| <sub><sup>[RTX 4070 Ti Super](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4070-ti-super/)</sup></sub> | <sub><sup>Ada AD103</sup></sub> | <sub><sup>16GB GDDR6X</sup></sub> | <sub><sup>672 GB/s</sup></sub> | <sub><sup>~44 TF</sup></sub> | <sub><sup>FP8 support</sup></sub> | <sub><sup>285W</sup></sub> | <sub><sup>$799</sup></sub> | <sub><sup>**56.2%** (485.1)</sup></sub> | <sub><sup>~18 it/s †</sup></sub> | <sub><sup>16GB @ $799, good SDXL throughput</sup></sub> |
| <sub><sup>[RTX A6000](https://www.nvidia.com/en-us/design-visualization/rtx-a6000/)</sup></sub> | <sub><sup>Ampere Pro</sup></sub> | <sub><sup>48GB GDDR6 ECC</sup></sub> | <sub><sup>768 GB/s</sup></sub> | <sub><sup>38.7 TF</sup></sub> | <sub><sup>3rd-gen Tensor</sup></sub> | <sub><sup>300W</sup></sub> | <sub><sup>~$4,650</sup></sub> | <sub><sup>N/A ‡</sup></sub> | <sub><sup>**19.09 it/s**</sup></sub> | <sub><sup>Pro / large VRAM / confirmed ECC stability</sup></sub> |
| <sub><sup>[RTX 4070 Ti](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4070-ti/)</sup></sub> | <sub><sup>Ada AD104</sup></sub> | <sub><sup>12GB GDDR6X</sup></sub> | <sub><sup>504 GB/s</sup></sub> | <sub><sup>~40 TF</sup></sub> | <sub><sup>FP8 support</sup></sub> | <sub><sup>285W</sup></sub> | <sub><sup>$799</sup></sub> | <sub><sup>**53.5%** (461.8)</sup></sub> | <sub><sup>17.65 it/s</sup></sub> | <sub><sup>Strong mid-range, 12GB limits FLUX fp16</sup></sub> |
| <sub><sup>[RTX 5070](https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5070/)</sup></sub> | <sub><sup>Blackwell GB205</sup></sub> | <sub><sup>12GB GDDR7</sup></sub> | <sub><sup>672 GB/s</sup></sub> | <sub><sup>~31 TF</sup></sub> | <sub><sup>FP4 support</sup></sub> | <sub><sup>250W</sup></sub> | <sub><sup>$549</sup></sub> | <sub><sup>**51.9%** (447.7)</sup></sub> | <sub><sup>N/A *</sup></sub> | <sub><sup>Efficient current-gen, VRAM limits large models</sup></sub> |
| <sub><sup>[RTX 4070 Super](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4070-super/)</sup></sub> | <sub><sup>Ada AD104</sup></sub> | <sub><sup>12GB GDDR6X</sup></sub> | <sub><sup>504 GB/s</sup></sub> | <sub><sup>~35 TF</sup></sub> | <sub><sup>FP8 support</sup></sub> | <sub><sup>220W</sup></sub> | <sub><sup>$599</sup></sub> | <sub><sup>**50.7%** (437.3)</sup></sub> | <sub><sup>~16 it/s †</sup></sub> | <sub><sup>Efficient Ada, good price/perf at 12GB</sup></sub> |
| <sub><sup>[RTX 4070](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4070/)</sup></sub> | <sub><sup>Ada AD104</sup></sub> | <sub><sup>12GB GDDR6X</sup></sub> | <sub><sup>504 GB/s</sup></sub> | <sub><sup>~29 TF</sup></sub> | <sub><sup>FP8 support</sup></sub> | <sub><sup>200W</sup></sub> | <sub><sup>$549</sup></sub> | <sub><sup>**44.2%** (381.0)</sup></sub> | <sub><sup>16.02 it/s</sup></sub> | <sub><sup>Entry high-end, 12GB boundary for SDXL</sup></sub> |
| <sub><sup>RTX A5000</sup></sub> | <sub><sup>Ampere Pro</sup></sub> | <sub><sup>24GB GDDR6 ECC</sup></sub> | <sub><sup>768 GB/s</sup></sub> | <sub><sup>27.8 TF</sup></sub> | <sub><sup>3rd-gen Tensor</sup></sub> | <sub><sup>230W</sup></sub> | <sub><sup>~$2,500</sup></sub> | <sub><sup>N/A ‡</sup></sub> | <sub><sup>**15.3 it/s**</sup></sub> | <sub><sup>Pro 24GB ECC, silent workstation operation</sup></sub> |
| <sub><sup>[RTX 5060 Ti 16GB](https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5060-ti/)</sup></sub> | <sub><sup>Blackwell GB206</sup></sub> | <sub><sup>16GB GDDR7</sup></sub> | <sub><sup>448 GB/s</sup></sub> | <sub><sup>~24 TF</sup></sub> | <sub><sup>FP4 support</sup></sub> | <sub><sup>180W</sup></sub> | <sub><sup>$429</sup></sub> | <sub><sup>**40.1%** (346.2)</sup></sub> | <sub><sup>N/A *</sup></sub> | <sub><sup>Best budget pick for SDXL (16GB VRAM)</sup></sub> |
| <sub><sup>[RTX 4060 Ti 16GB](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4060-ti/)</sup></sub> | <sub><sup>Ada AD106</sup></sub> | <sub><sup>16GB GDDR6</sup></sub> | <sub><sup>288 GB/s</sup></sub> | <sub><sup>~22 TF</sup></sub> | <sub><sup>FP8 support</sup></sub> | <sub><sup>160W</sup></sub> | <sub><sup>$499</sup></sub> | <sub><sup>**33.9%** (292.1)</sup></sub> | <sub><sup>12.32 it/s †</sup></sub> | <sub><sup>Budget 16GB VRAM, low bandwidth bottleneck</sup></sub> |
| <sub><sup>RTX 3090</sup></sub> | <sub><sup>Ampere GA102</sup></sub> | <sub><sup>24GB GDDR6X</sup></sub> | <sub><sup>936 GB/s</sup></sub> | <sub><sup>35.6 TF</sup></sub> | <sub><sup>3rd-gen Tensor</sup></sub> | <sub><sup>350W</sup></sub> | <sub><sup>~$700 used</sup></sub> | <sub><sup>N/A ‡</sup></sub> | <sub><sup>**16.66 it/s**</sup></sub> | <sub><sup>Used market 24GB option, high BW, aging arch</sup></sub> |
| <sub><sup>RTX 3060 Ti</sup></sub> | <sub><sup>Ampere GA104</sup></sub> | <sub><sup>8GB GDDR6</sup></sub> | <sub><sup>448 GB/s</sup></sub> | <sub><sup>16.2 TF</sup></sub> | <sub><sup>3rd-gen Tensor</sup></sub> | <sub><sup>200W</sup></sub> | <sub><sup>~$250 used</sup></sub> | <sub><sup>N/A ‡</sup></sub> | <sub><sup>**8.62 it/s**</sup></sub> | <sub><sup>Entry point, VRAM too limited for SDXL</sup></sub> |

*\* RTX 50 series not yet included in Puget Systems SD benchmark suite (Blackwell launched Jan 2025)*
*† Estimated from close-spec card benchmarks, same Puget Systems test conditions*
*‡ Not included in Tom's Hardware consumer GPU hierarchy test suite*

---


## Detailed Specifications by Category

### NVIDIA GeForce RTX 50 Series — Blackwell

| <sub><sup>Model</sup></sub> | <sub><sup>GPU Die</sup></sub> | <sub><sup>CUDA Cores</sup></sub> | <sub><sup>VRAM</sup></sub> | <sub><sup>Mem BW</sup></sub> | <sub><sup>FP32 TF</sup></sub> | <sub><sup>FP16 TF</sup></sub> | <sub><sup>FP4 TF</sup></sub> | <sub><sup>TDP</sup></sub> | <sub><sup>MSRP</sup></sub> | <sub><sup>TH CC%</sup></sub> |
|-------|--------|--------|------|--------|--------|--------|--------|-----|------|------|
| <sub><sup>[RTX 5090](https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5090/)</sup></sub> | <sub><sup>GB202</sup></sub> | <sub><sup>21,760</sup></sub> | <sub><sup>32GB GDDR7 @28Gbps 512-bit</sup></sub> | <sub><sup>1792 GB/s</sup></sub> | <sub><sup>104.8 TF</sup></sub> | <sub><sup>838 TF</sup></sub> | <sub><sup>3352 TF</sup></sub> | <sub><sup>575W</sup></sub> | <sub><sup>$1,999</sup></sub> | <sub><sup>**100%** (862.8)</sup></sub> |
| <sub><sup>[RTX 5080](https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5080/)</sup></sub> | <sub><sup>GB203</sup></sub> | <sub><sup>10,752</sup></sub> | <sub><sup>16GB GDDR7 @30Gbps</sup></sub> | <sub><sup>690 GB/s</sup></sub> | <sub><sup>~56 TF</sup></sub> | <sub><sup>—</sup></sub> | <sub><sup>yes</sup></sub> | <sub><sup>360W</sup></sub> | <sub><sup>$999</sup></sub> | <sub><sup>**69.8%** (601.9)</sup></sub> |
| <sub><sup>[RTX 5070 Ti](https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5070-ti/)</sup></sub> | <sub><sup>GB203</sup></sub> | <sub><sup>8,960</sup></sub> | <sub><sup>16GB GDDR7 @28Gbps 256-bit</sup></sub> | <sub><sup>896 GB/s</sup></sub> | <sub><sup>~44 TF</sup></sub> | <sub><sup>—</sup></sub> | <sub><sup>yes</sup></sub> | <sub><sup>300W</sup></sub> | <sub><sup>$749</sup></sub> | <sub><sup>**63.4%** (547.3)</sup></sub> |
| <sub><sup>[RTX 5070](https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5070/)</sup></sub> | <sub><sup>GB205</sup></sub> | <sub><sup>6,144</sup></sub> | <sub><sup>12GB GDDR7 @28Gbps 192-bit</sup></sub> | <sub><sup>672 GB/s</sup></sub> | <sub><sup>~31 TF</sup></sub> | <sub><sup>—</sup></sub> | <sub><sup>yes</sup></sub> | <sub><sup>250W</sup></sub> | <sub><sup>$549</sup></sub> | <sub><sup>**51.9%** (447.7)</sup></sub> |
| <sub><sup>[RTX 5060 Ti 16GB](https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5060-ti/)</sup></sub> | <sub><sup>GB206</sup></sub> | <sub><sup>4,608</sup></sub> | <sub><sup>16GB GDDR7 @28Gbps 128-bit</sup></sub> | <sub><sup>448 GB/s</sup></sub> | <sub><sup>~24 TF</sup></sub> | <sub><sup>—</sup></sub> | <sub><sup>yes</sup></sub> | <sub><sup>180W</sup></sub> | <sub><sup>$429</sup></sub> | <sub><sup>**40.1%** (346.2)</sup></sub> |

**Notes — Blackwell RTX 50:**
- Native FP4 precision is a Blackwell-exclusive feature enabling up to 3× higher AI throughput vs Ada FP8 per Nvidia.
- RTX 5090 has 33% more SMs, 33% more VRAM, and 78% more memory bandwidth than the RTX 4090.
- In Tom's Hardware's content creation test suite (which includes Stable Diffusion 1.5/XL), the RTX 5090 scores 26.7% higher than the RTX 4090.

---

### NVIDIA GeForce RTX 40 Series — Ada Lovelace

| <sub><sup>Model</sup></sub> | <sub><sup>GPU Die</sup></sub> | <sub><sup>CUDA Cores</sup></sub> | <sub><sup>VRAM</sup></sub> | <sub><sup>Mem BW</sup></sub> | <sub><sup>FP32 TF</sup></sub> | <sub><sup>FP16 TF</sup></sub> | <sub><sup>FP8 TF</sup></sub> | <sub><sup>TDP</sup></sub> | <sub><sup>MSRP</sup></sub> | <sub><sup>SD A1111 it/s</sup></sub> |
|-------|--------|--------|------|--------|--------|--------|--------|-----|------|------|
| <sub><sup>[RTX 4090](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4090/)</sup></sub> | <sub><sup>AD102</sup></sub> | <sub><sup>16,384</sup></sub> | <sub><sup>24GB GDDR6X @21Gbps 384-bit</sup></sub> | <sub><sup>1008 GB/s</sup></sub> | <sub><sup>82.6 TF</sup></sub> | <sub><sup>661 TF</sup></sub> | <sub><sup>1321 TF</sup></sub> | <sub><sup>450W</sup></sub> | <sub><sup>$1,599</sup></sub> | <sub><sup>**21.04 it/s** / ~57 it/s TensorRT</sup></sub> |
| <sub><sup>[RTX 4080 Super](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4080-super/)</sup></sub> | <sub><sup>AD103</sup></sub> | <sub><sup>10,240</sup></sub> | <sub><sup>16GB GDDR6X @23Gbps 256-bit</sup></sub> | <sub><sup>736 GB/s</sup></sub> | <sub><sup>~52 TF</sup></sub> | <sub><sup>—</sup></sub> | <sub><sup>yes</sup></sub> | <sub><sup>320W</sup></sub> | <sub><sup>$999</sup></sub> | <sub><sup>~19–20 it/s †</sup></sub> |
| <sub><sup>[RTX 4080](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4080/)</sup></sub> | <sub><sup>AD103</sup></sub> | <sub><sup>9,728</sup></sub> | <sub><sup>16GB GDDR6X @22.4Gbps 256-bit</sup></sub> | <sub><sup>717 GB/s</sup></sub> | <sub><sup>~49 TF</sup></sub> | <sub><sup>—</sup></sub> | <sub><sup>yes</sup></sub> | <sub><sup>320W</sup></sub> | <sub><sup>$1,199</sup></sub> | <sub><sup>**19.41 it/s** / ~50 it/s TensorRT</sup></sub> |
| <sub><sup>[RTX 4070 Ti Super](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4070-ti-super/)</sup></sub> | <sub><sup>AD103</sup></sub> | <sub><sup>8,448</sup></sub> | <sub><sup>16GB GDDR6X @21Gbps 256-bit</sup></sub> | <sub><sup>672 GB/s</sup></sub> | <sub><sup>~44 TF</sup></sub> | <sub><sup>—</sup></sub> | <sub><sup>yes</sup></sub> | <sub><sup>285W</sup></sub> | <sub><sup>$799</sup></sub> | <sub><sup>~18 it/s †</sup></sub> |
| <sub><sup>[RTX 4070 Ti](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4070-ti/)</sup></sub> | <sub><sup>AD104</sup></sub> | <sub><sup>7,680</sup></sub> | <sub><sup>12GB GDDR6X @21Gbps 192-bit</sup></sub> | <sub><sup>504 GB/s</sup></sub> | <sub><sup>~40 TF</sup></sub> | <sub><sup>—</sup></sub> | <sub><sup>yes</sup></sub> | <sub><sup>285W</sup></sub> | <sub><sup>$799</sup></sub> | <sub><sup>**17.65 it/s**</sup></sub> |
| <sub><sup>[RTX 4070 Super](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4070-super/)</sup></sub> | <sub><sup>AD104</sup></sub> | <sub><sup>7,168</sup></sub> | <sub><sup>12GB GDDR6X @21Gbps 192-bit</sup></sub> | <sub><sup>504 GB/s</sup></sub> | <sub><sup>~35 TF</sup></sub> | <sub><sup>—</sup></sub> | <sub><sup>yes</sup></sub> | <sub><sup>220W</sup></sub> | <sub><sup>$599</sup></sub> | <sub><sup>~16 it/s †</sup></sub> |
| <sub><sup>[RTX 4070](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4070/)</sup></sub> | <sub><sup>AD104</sup></sub> | <sub><sup>5,888</sup></sub> | <sub><sup>12GB GDDR6X @21Gbps 192-bit</sup></sub> | <sub><sup>504 GB/s</sup></sub> | <sub><sup>~29 TF</sup></sub> | <sub><sup>—</sup></sub> | <sub><sup>yes</sup></sub> | <sub><sup>200W</sup></sub> | <sub><sup>$549</sup></sub> | <sub><sup>**16.02 it/s**</sup></sub> |
| <sub><sup>[RTX 4060 Ti 16GB](https://www.nvidia.com/en-us/geforce/graphics-cards/40-series/rtx-4060-ti/)</sup></sub> | <sub><sup>AD106</sup></sub> | <sub><sup>4,352</sup></sub> | <sub><sup>16GB GDDR6 @18Gbps 128-bit</sup></sub> | <sub><sup>288 GB/s</sup></sub> | <sub><sup>~22 TF</sup></sub> | <sub><sup>—</sup></sub> | <sub><sup>yes</sup></sub> | <sub><sup>160W</sup></sub> | <sub><sup>$499</sup></sub> | <sub><sup>**12.32 it/s** (8GB variant)</sup></sub> |

**Notes — Ada Lovelace RTX 40:**
- With TensorRT extension: RTX 4090 averages 2.75× baseline A1111 (~57 it/s), RTX 4080 averages 2.6× (~50 it/s).
- RTX 4060 Ti 16GB variant has notably narrow 128-bit bus (288 GB/s), creating a bandwidth bottleneck despite sufficient VRAM.
- Ada's FP8 Tensor Cores are the current standard for TensorRT-accelerated inference.

---

### NVIDIA RTX Professional Series (ex-Quadro) — Ada & Ampere

| <sub><sup>Model</sup></sub> | <sub><sup>Generation</sup></sub> | <sub><sup>CUDA Cores</sup></sub> | <sub><sup>VRAM</sup></sub> | <sub><sup>Mem BW</sup></sub> | <sub><sup>FP32 TF</sup></sub> | <sub><sup>AI TOPS</sup></sub> | <sub><sup>TDP</sup></sub> | <sub><sup>MSRP</sup></sub> | <sub><sup>SD A1111 it/s</sup></sub> | <sub><sup>Notes</sup></sub> |
|-------|--------|--------|------|--------|--------|--------|-----|------|------|------|
| <sub><sup>[RTX 6000 Ada](https://www.nvidia.com/en-us/design-visualization/rtx-6000/)</sup></sub> | <sub><sup>Ada Lovelace</sup></sub> | <sub><sup>18,176</sup></sub> | <sub><sup>48GB GDDR6 ECC</sup></sub> | <sub><sup>960 GB/s</sup></sub> | <sub><sup>91.1 TF</sup></sub> | <sub><sup>1457 AI TOPS (FP8)</sup></sub> | <sub><sup>300W</sup></sub> | <sub><sup>~$6,800</sup></sub> | <sub><sup>**21.11 it/s**</sup></sub> | <sub><sup>Top pro single-card, NVLink-ready, vGPU support</sup></sub> |
| <sub><sup>[RTX A6000](https://www.nvidia.com/en-us/design-visualization/rtx-a6000/)</sup></sub> | <sub><sup>Ampere</sup></sub> | <sub><sup>10,752</sup></sub> | <sub><sup>48GB GDDR6 ECC</sup></sub> | <sub><sup>768 GB/s</sup></sub> | <sub><sup>38.7 TF</sup></sub> | <sub><sup>3rd-gen Tensor</sup></sub> | <sub><sup>300W</sup></sub> | <sub><sup>~$4,650</sup></sub> | <sub><sup>**19.09 it/s**</sup></sub> | <sub><sup>48GB ECC at lower cost, NVLink-ready</sup></sub> |
| <sub><sup>[RTX A5000](https://www.nvidia.com/en-us/design-visualization/rtx-a5000/)</sup></sub> | <sub><sup>Ampere</sup></sub> | <sub><sup>8,192</sup></sub> | <sub><sup>24GB GDDR6 ECC</sup></sub> | <sub><sup>768 GB/s</sup></sub> | <sub><sup>27.8 TF</sup></sub> | <sub><sup>3rd-gen Tensor</sup></sub> | <sub><sup>230W</sup></sub> | <sub><sup>~$2,500</sup></sub> | <sub><sup>**15.3 it/s**</sup></sub> | <sub><sup>Pro 24GB, quiet, ECC, NVLink optional</sup></sub> |

**Notes — Professional RTX:**
- RTX 6000 Ada SD performance (21.11 it/s) is on par with RTX 4090 (21.04 it/s) despite similar CUDA count advantage via higher FP8 Tensor headroom and 2× VRAM.
- Notable: RTX A5000 at 24GB has **3× more iterations/sec than the AMD Radeon PRO W7800 at 32GB** under Automatic1111.
- RTX 6000 Ada vs RTX A6000: ~10.5% faster in SD at 1.47× the price — marginal gain for pure diffusion.
- NVLink on pro cards enables 2× RTX A6000 = 96GB pool (vs consumer GeForce which has no NVLink support).
- ECC memory prevents silent bit errors — recommended for unattended / production inference pipelines.

---


## TensorRT Performance Multipliers (Automatic1111, Puget Systems Oct 2023)

| <sub><sup>GPU</sup></sub> | <sub><sup>Base A1111 (it/s)</sup></sub> | <sub><sup>+ xFormers (it/s)</sup></sub> | <sub><sup>+ TensorRT extension (it/s)</sup></sub> | <sub><sup>Gain vs base</sup></sub> | <sub><sup>Gain vs xFormers</sup></sub> |
|-------|--------|--------|--------|--------|--------|
| <sub><sup>RTX 4090 (Ryzen platform)</sup></sub> | <sub><sup>~22</sup></sub> | <sub><sup>~33</sup></sub> | <sub><sup>~51</sup></sub> | <sub><sup>**~2.3×**</sup></sub> | <sub><sup>~1.7×</sup></sub> |
| <sub><sup>RTX 4090 (Threadripper PRO)</sup></sub> | <sub><sup>~15</sup></sub> | <sub><sup>~21</sup></sub> | <sub><sup>~51</sup></sub> | <sub><sup>**~3.4×**</sup></sub> | <sub><sup>~2.6×</sup></sub> |
| <sub><sup>RTX 4080 (Ryzen platform)</sup></sub> | <sub><sup>~20</sup></sub> | <sub><sup>~29</sup></sub> | <sub><sup>~50</sup></sub> | <sub><sup>**~2.5×**</sup></sub> | <sub><sup>~1.75×</sup></sub> |
| <sub><sup>RTX 4080 (Threadripper PRO)</sup></sub> | <sub><sup>~18</sup></sub> | <sub><sup>~24</sup></sub> | <sub><sup>~50</sup></sub> | <sub><sup>**~2.8×**</sup></sub> | <sub><sup>~2.1×</sup></sub> |

*Ten 512×512 images at 50 steps generates in ~10 seconds on RTX 4090 + TensorRT = ~1 image/sec.*


---


## Key Findings

- **Nvidia dominates diffusion inference** across all implementations and price points. With Automatic1111 + TensorRT, NVIDIA RTX 4080 runs ~2.2× faster than AMD Radeon RX 7900 XTX (best-optimized AMD result with Olive/SHARK).
- **Memory bandwidth is the primary bottleneck** for step latency. RTX 4060 Ti 16GB's narrow 128-bit bus (288 GB/s) is significantly slower than RTX 4070 (504 GB/s) despite similar compute.
- **VRAM threshold**: 12GB handles SD 1.5 comfortably. 16GB is recommended for SDXL and FLUX.1 in fp16. 24–48GB for fp32, large batches, or model fine-tuning.
- **RTX 6000 Ada matches RTX 4090 in SD speed** (21.11 vs 21.04 it/s) while offering 48GB ECC, vGPU, NVLink — making it the pro standard for unattended pipelines.
- **RTX 5090 FP4 advantage**: Nvidia claims up to 3× faster AI inference vs RTX 4090 using FP4 + TensorRT. Tom's HW content creation composite (includes SD) places it 26.7% ahead of RTX 4090 in a mixed workload score.
- **TensorRT adds ~2.75× vs base A1111** on average across RTX 40-series (confirmed Puget Systems Oct 2023). Setup takes ~15 minutes.

---


## VRAM Guide

| <sub><sup>VRAM</sup></sub> | <sub><sup>SD 1.5</sup></sub> | <sub><sup>SDXL fp16</sup></sub> | <sub><sup>FLUX.1 fp16</sup></sub> | <sub><sup>FLUX.1 fp8</sup></sub> | <sub><sup>Fine-tuning LoRA</sup></sub> |
|------|--------|--------|--------|--------|--------|
| <sub><sup>8 GB</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>⚠️ with offload</sup></sub> | <sub><sup>❌</sup></sub> | <sub><sup>⚠️ with offload</sup></sub> | <sub><sup>⚠️ limited batch</sup></sub> |
| <sub><sup>12 GB</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>⚠️ with offload</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅ small batch</sup></sub> |
| <sub><sup>16 GB</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅</sup></sub> |
| <sub><sup>24 GB</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅ large batch</sup></sub> |
| <sub><sup>48 GB</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅</sup></sub> | <sub><sup>✅ + fp32</sup></sub> | <sub><sup>✅ full batch / multi-model</sup></sub> |

---


## Sources

1. **Tom's Hardware GPU Benchmarks Hierarchy 2026** — Content creation rankings (SD 1.5/XL, Blender, MLPerf Client 0.5, SPECworkstation 4.0), January 2026 update
   https://www.tomshardware.com/reviews/gpu-hierarchy,4388.html

2. **Tom's Hardware — Nvidia GeForce RTX 5090 Founders Edition Review** — FP32/FP16/FP4 specs, architecture comparison table (Jan 23, 2025)
   https://www.tomshardware.com/pc-components/gpus/nvidia-geforce-rtx-5090-review

3. **Puget Systems — Stable Diffusion Performance: NVIDIA GeForce vs AMD Radeon** — A1111 + xFormers it/s benchmarks for RTX 40/30 series (July 31, 2023)
   https://www.pugetsystems.com/labs/articles/stable-diffusion-performance-nvidia-geforce-vs-amd-radeon/

4. **Puget Systems — Stable Diffusion Performance: NVIDIA RTX vs Radeon PRO** — RTX 6000 Ada, A6000, A5000 SD benchmarks (July 31, 2023)
   https://www.pugetsystems.com/labs/articles/stable-diffusion-performance-professional-gpus/

5. **Puget Systems — NVIDIA TensorRT Extension for Stable Diffusion Performance Analysis** — TensorRT multipliers on RTX 4090 and RTX 4080 (Oct 31, 2023)
   https://www.pugetsystems.com/labs/articles/nvidia-tensorrt-extension-for-stable-diffusion-performance-analysis/

6. **Nvidia — RTX 6000 Ada Generation Product Page** — Official specs: 91.1 TFLOPS FP32, 1457 AI TOPS FP8, 48GB GDDR6, 300W
   https://www.nvidia.com/en-us/design-visualization/rtx-6000/

7. **VideoCardz — NVIDIA GeForce RTX 5090/5080 Spec Table** — Confirmed RTX 50 series CUDA counts, memory speed, TDP, and MSRP (Jan 2025)
   https://videocardz.com/newz/nvidia-geforce-rtx-5090-reviews-go-live-january-24-rtx-5080-on-january-30


---

*Last updated: April 2026*
*Prices are approximate and vary by region, retailer, and market conditions*
*SD A1111 it/s benchmarks from Puget Systems are geometrical mean over SD 1.5 prompts at 512×512*
