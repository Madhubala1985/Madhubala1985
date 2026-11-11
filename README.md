# Hi, I'm Madhusudhan 👋

**AI / Machine Learning engineer.** I build learning systems end to end, from the research question to a
model running unattended in production, and I care most about the part many projects skip: proving that a
model actually works before trusting it.

- 🎓 Bachelor's thesis at **Johannes Kepler University Linz** (Institute for Pervasive Computing): continual learning in spiking neural networks
- 🧠 Built autonomous **market-intelligence models** that perceive, reason, abstain, and grade their own decisions on live data
- 🔬 Research interests: continual and federated learning, neuromorphic computing, time-series models, LLM evaluation
- 🌱 Open to **ML engineer, AI engineer, and research engineer** roles

---

## ⭐ Featured work

### 🧬 [Selective Plasticity for Continual Learning in Spiking Neural Networks](https://github.com/Madhubala1985/Decision-Guided-Continual-Learning-in-Spiking-Neural-Networks)
*Bachelor's thesis · PyTorch*
A per-sample decision module on top of Synaptic Intelligence decides whether each training sample should
*update*, *consolidate*, *protect*, or be *ignored* by a spiking network learning five tasks in sequence.
- **99.1% accuracy** on Split-MNIST with forgetting cut from 0.35 to **0.0015**
- Skips **29% of training samples** with no measurable loss in retention, saving ~20% of synaptic operations under an event-driven cost model
- LIF/ALIF neurons with surrogate gradients, a matched random-skip control, and three-seed statistics

### 🥇 [XAU Market Intelligence](https://github.com/Madhubala1985/xau-market-intelligence)
*Decision model for gold · 43k lines of Python · 906 tests*
A self-observing model that reads market structure, classifies regime, treats *no action* as a valid
decision, and keeps a journal it learns from offline.
- Pre-registered validation: causal replay, walk-forward k-fold, Bonferroni-corrected random controls, sealed holdout
- **Rigorous negative result:** no candidate signal beat a random-entry control, so the model correctly stayed flat. The one surviving effect ships as a macro-regime risk dial.

### 📈 [NSE Market Intelligence v2](https://github.com/Madhubala1985/nse-market-intelligence-v2)
*Autonomous model on live data · 92k lines · Oracle Cloud*
Ran every trading day against live market data: multi-timeframe context fusion, options analytics
(Greeks, IV surface, gamma exposure), shadow-model learning, and fail-closed execution behind 9 interlocks.
- Benchmarked an **LLM analyst (Claude)** and the **Kronos time-series foundation model** against the quantitative model on the same real data
- Diagnosed why a profitable-looking result came from a single day, and **kept real money disarmed** because the edge wasn't proven

### 🌐 [Few-Shot Federated Learning on CIFAR-10](https://github.com/Madhubala1985/Few-Short-Federated-Learning-Cifar-10)
*Empirical study · TensorFlow*
Prototype-based communication instead of gradient sharing for non-IID clients with only 5 labelled samples
per class, compared with centralized few-shot learning and FedAvg across backbones (InceptionV3, ResNet50).

### More projects
| Project | What it is |
|---|---|
| [NSE Market Intelligence v1](https://github.com/Madhubala1985/nse-market-intelligence-v1) | Event-driven perception pipeline, structure models and ML classifiers (foundation of v2) |
| [Energy Monitoring & Carbon Footprint](https://github.com/Madhubala1985/Energy-Monitoring-and-Carbon-Footprint-System) | CNN + LSTM energy forecasting from IoT sensor data, with emissions estimates |
| [Deep Learning Image Classification](https://github.com/Madhubala1985/Deep_Learning_Image_Classification) | 20-class CNN in PyTorch with augmentation, scheduling and early stopping |
| [Multi-Agent Swarm Simulator](https://github.com/Madhubala1985/Multi-agent-swarm-simulator) | Boids-style swarm behaviours plus PSO/ACO experiments |
| [APMC Farm Market](https://github.com/Madhubala1985/APMC_Farm_market) | Farm-to-market platform with live auctions (React, TypeScript, Supabase) |
| [Flask Task Manager](https://github.com/Madhubala1985/todo-flask-app) | Multi-user Flask app with authentication, per-user access control and a pytest suite |
| [Directory Scraper Planner](https://github.com/Madhubala1985/AI_Automated_Webscrapper) | React prototype for planning scraping and lead-generation workflows |

---

## 🛠️ Toolbox

**Machine learning:** PyTorch · TensorFlow/Keras · scikit-learn · NumPy · pandas · Matplotlib
**Methods:** continual learning · spiking neural networks · federated and few-shot learning · time-series forecasting · walk-forward validation · LLM and foundation-model evaluation
**Engineering:** Python 3.12 · asyncio · Pydantic · pytest · GitHub Actions · Redis · PostgreSQL/TimescaleDB
**Infrastructure:** Linux · Oracle Cloud · systemd · cron · Git
**Web:** React · TypeScript · Supabase · Flask

## 💡 How I work

- **Measure, don't assume.** Every model gets a baseline, a random control, and an out-of-sample test.
- **Report honestly.** A clear negative result is worth more than an overfit success.
- **Fail closed.** When a system can't confirm its own state, it stops instead of guessing.
- **Ship with tests.** My largest project carries 900+ unit tests.

---

<sub>Several projects were built with AI pair-programming (Claude Code). Market projects are research only, not financial advice.</sub>
