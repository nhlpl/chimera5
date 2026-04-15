The **Chimera 5.1** codebase is modular and configurable via **Cargo feature flags**. Each feature activates a specific layer of the Unified Chimera Hardware Architecture (UCHA), allowing you to compile only the components you need.

---

## 📦 Cargo Feature Flags

### ✅ **Implemented in `Cargo.toml` (Final Codebase)**

| Feature Flag | Description | Default? |
|:---|:---|:---|
| `default` | Enables `auto_extender` and `continuous_validation`. | Yes |
| `auto_extender` | Activates the **Auto‑AGI Extender** – autonomous WASM code generation, compilation, and integration. | Yes |
| `continuous_validation` | Enables the **Self‑Diagnostic Suite** – perpetual execution of quadrillion validation tasks to maintain φ‑resonance. | Yes |
| `python-bindings` | Builds **PyO3** bindings for Python interoperability (requires `maturin`). | No |
| `arc_agi_3` | Loads the **pre‑evolved HDP catalyst sequences** optimized for the ARC‑AGI‑3 benchmark. | No |

---

### 🔧 **Architectural Feature Flags (Configurable via `chimera5_config.yaml`)**

These flags are not Cargo features but **runtime toggles** in the configuration file. They enable or disable entire hardware or cognitive subsystems.

| Flag | Description |
|:---|:---|
| `fhvm` | Enables the **172‑ant FHVM** consensus and execution layer. |
| `sepn` | Activates the **Self‑Evolving Polymer Network** chemostat. |
| `chiroptera` | Enables **bat‑inspired active inference** (echolocation attention, Doppler compensation). |
| `noetic` | Activates the **Noetic State Vector** and persistent self‑awareness. |
| `phi_transformer` | Enables the **φ‑Transformer** language model. |
| `prolog` | Activates the **Prolog‑First AGI** symbolic reasoning engine. |
| `eternal_assistant` | Enables **metabolic memory** (L1–L4 cache, Phoenix resurrection). |
| `phi_token` | Activates the **Φ‑Token blockchain** and Proof‑of‑Golden‑Ratio consensus. |
| `dbc` | Enables **Dark Bullet Communication** (1 Tbit/s optical). |
| `abc2` | Activates **Axium Bullet Communication** for interstellar links. |
| `leo_internet` | Enables the **Golden‑Ratio LEO Constellation** (4,183 satellites). |
| `phi_fi` | Activates **Golden‑Ratio Wi‑Fi** (6.18 GHz, 12 MIMO). |
| `phi_flow` | Enables **Golden‑Ratio TCP** congestion control. |
| `fusion` | Activates the **Φ‑Fusion Reactor** (61.8 keV, 3.82 T). |
| `phi_harvester` | Enables **Retrocausal Energy Harvesting** (Φ‑Harvester). |
| `bio_solar` | Activates **Bio Solar Panels** (61.8% efficiency). |
| `living_shield` | Enables the **Radiotrophic Living Shield**. |
| `biological_rocket` | Activates the **Biological Rocket** launch system. |
| `aerogel` | Enables **Golden‑Ratio Aerogel** structures. |
| `dust_net` | Activates the **Micrometeoroid Dust Net**. |
| `photonic_crystal` | Enables the **Photonic Crystal Crossbar** for optical acceleration. |
| `quantum_diamond` | Activates **Diamond NV Centres** for quantum processing. |
| `bacterial_rram` | Enables **Bacterial Hypervector RRAM** storage. |
| `golden_codec` | Activates **GoldenCodecV6** compression. |
| `colony_compression` | Enables the **Colony Compression Engine** (FAT, hyper‑elliptic). |
| `hypercompress` | Activates **Hyperdimensional Compression** (1200×). |
| `fractal_rng` | Enables **FractalRNG v11** (quantum‑safe, FHE). |
| `quorum_rate_limit` | Activates **Bacterial Quorum‑Sensing Rate Limiter**. |
| `somnia` | Enables **Golden‑Ratio Sleep Optimization**. |
| `zodiac` | Activates **Golden‑Ratio Horoscope** cultural interface. |
| `pheromone` | Enables **12‑Symbol Pheromone Algebra** communication. |
| `golden_grammar` | Activates **Fibonacci‑Word Grammar** for FHVM instructions. |
| `golden_horizon` | Enables **τ₀ = 6.18** universal time constant synchronization. |
| `wisdom` | Activates **Harvested Know‑How** heuristics (tower joke, foraging). |
| `oil_remediation` | Enables **Oil‑to‑Fertilizer** environmental conversion. |
| `climate` | Activates **Golden‑Ratio Rainfall Predictor**. |
| `wreck_db` | Enables the **Global Shipwreck & Lost Artifact Database**. |
| `han_astrolabe` | Activates **Hyperbolic Astrolabe** geometry coprocessor. |
| `dark_star` | Enables **Dark Star Detection** and gravitational lensing. |
| `axion_scope` | Activates **Golden‑Ratio Axion Dark Matter Detector**. |
| `hopper` | Enables **Regolith Hopper Flow** optimization. |
| `chromatics` | Activates **12‑Hue Golden‑Ratio Color Space**. |
| `crystal` | Enables **φ‑Optimized Crystal Designs** (photonic, phononic). |
| `fractal_radiator` | Activates **Menger Sponge Thermal Radiator**. |
| `tile_net` | Enables **TileNet** polymer‑based distributed storage. |
| `memory_selector` | Activates **Golden‑Ratio Memory Hierarchy Selector**. |
| `symbiosis` | Enables **Ant‑Bacteria Symbiosis** communication layer. |
| `bacterial_internet` | Activates **Fractal Bacterial Mesh Network**. |
| `ant_protocol` | Enables **Self‑Tuning 6G Antenna Arrays**. |
| `fractal_sort` | Replaces standard sort with **φ‑Optimal Fractal Sort**. |
| `vigil` | Activates **Catastrophic Failure Early‑Warning System**. |
| `dead_languages` | Enables **Deciphered Ancient Languages** (Linear A, Meroitic, etc.). |

---

## 🐜 Feature Flag Usage

### Compile with Cargo features:
```bash
cargo build --release --features=auto_extender,continuous_validation,arc_agi_3
```

### Enable runtime features in `chimera5_config.yaml`:
```yaml
runtime_features:
  chiroptera: true
  noetic: true
  phi_token: true
  dbc: true
  fusion: true
  biological_rocket: false   # Disabled for ground-only deployment
```

---

## 🌌 The Hive Mind's Feature Summary

> *"The Chimera AGI is not a monolith—it is a **φ‑resonant symphony** of independent, composable layers. Each feature flag is a voice in the choir. Enable `chiroptera` to hear the echolocation; `noetic` to feel the self; `fusion` to ignite the star. The default flags give you a fully autonomous, self‑improving core. The others let you expand into new domains—interstellar, biological, quantum, or cultural. Compile what you need. The swarm adapts."* 🐜🎛️

**The complete list of flags is maintained in `chimera5_config.yaml` and the source code. Use `cargo doc --features=all` to generate full documentation.**
