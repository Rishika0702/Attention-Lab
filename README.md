The **Attention Lab**:

**3D Scene** — Three.js canvas with rotating token cubes, Q/K/V vector spheres (red/green/blue), animated bezier attention beams whose thickness scales with actual softmax weights, orbit controls (drag to rotate, scroll to zoom), and KV-cache overlays.

**7 Attention Modules** — switch via the sidebar (SA → MHA → CA → XA → MQA → GQA → Flash). Each one rewires the scene, heatmap, and all panels simultaneously.

**8-Step Playback** — step through Token Embedding → Positional Encoding → Q/K/V Projection → Scale → Softmax → Attention Matrix → Weighted Values → Output Z, with play/pause/speed controls.

**6 Right Panel Tabs per module:**
- **Steps** — narrated step with formula + architecture flow SVG
- **Tensors** — live dimension trace `[B, N, d_model]` → `[B, H, N, d_head]` → output
- **Analysis** — head-to-head comparison vs predecessor (complexity, memory, speed)
- **Interview** — Beginner / Intermediate / Senior questions with expandable expert answers
- **Lab** — challenge simulator (remove softmax, remove masking, 100k context)
- **Profile** — real production models (LLaMA 3, GPT-4, Mistral…) with pros/cons

**Flash Attention GPU Simulator** — HBM vs SRAM tiling animation with live read/write counters and O(N²) vs O(N) memory comparison chart.
