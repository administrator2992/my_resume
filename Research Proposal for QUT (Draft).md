# RESEARCH PROPOSAL

**Project Title:** Energy-Aware, Disruption-Resilient Resource Orchestration for Distributed Edge AI in Public Fog Computing Environments  
**Applicant:** Ahmad Naufal Labiib Nabhaan  
**Proposed Supervisor:** Dr. R. Naha  
**Target Program:** Master of Philosophy (MPhil) in Computer Science, Queensland University of Technology (QUT)

---

### **1. Objectives of the Research Project**
The overarching aim of this research is to design, implement, and validate a hierarchical resource orchestration framework that balances local device energy constraints with global network reliability in public fog computing environments. 

This aim will be achieved through three distinct, numbered sub-objectives:
1. **Objective 1 (Micro-Level Analysis):** To profile the physical impact of diverse Edge AI workloads (e.g., computer vision, OCR, and language models) on commodity client processor behaviors, specifically evaluating power draw, core temperature, and battery depletion slopes.
2. **Objective 2 (Macro-Level Integration):** To mathematically extend global network scheduling models by dynamically adjusting Markov chain state transition matrices using real-time local hardware telemetry.
3. **Objective 3 (System Demonstration):** To validate the complete connected system via large-scale discrete-event simulation, proving a significant reduction in network dropouts and application disruptions compared to state-of-the-art schedulers.

---

### **2. Overview of the Research Project**

#### **The Global Context**
Public fog computing has emerged as a promising paradigm, enabling the leasing of idle consumer hardware—such as smartphones, personal laptops, and single-board computers—to form distributed networks for real-time edge applications. This paradigm minimizes the need for expensive, centralized cloud infrastructure. However, utilizing volatile consumer nodes introduces severe operational challenges, as these devices can disconnect or fail unpredictably.

#### **The Physical Background Problem (Micro-Level)**
Heavy Deep Learning (DL) models place immense physical strain on commodity consumer devices. Our preliminary research demonstrates a significant energy paradox: different hardware settings can sustain the same performance target (e.g., 30 FPS inference) while drawing vastly different power levels (e.g., 6W vs. 8W on NVIDIA Jetson devices). Compute-heavy vision models (like YOLOv11) push processor utilization to its ceiling, spiking power consumption to 15 Watts and core temperatures to 85°C, which triggers sudden OS-level thermal throttling or hardware shutdowns. Conversely, memory-bandwidth-bound models (like Ministral 3B) generate steep battery depletion slopes due to relentless data transfers between RAM and cache. These workload-induced hardware failures represent a major source of device volatility in fog networks.

#### **The Orchestration Blind Spot (Macro-Level)**
State-of-the-art public fog schedulers—such as the Markovian model proposed by Battula, Naha, et al. (2026)—optimize network overutilization by 16.17% and reduce latency by 11.83% by predicting device mobility and external network dropouts. However, these models assume that device failures are strictly external events. They remain blind to internal, workload-induced hardware crashes. To build truly resilient fog networks, global scheduling models must be integrated with local hardware telemetry.

#### **The Core Technical Justification & Development Impact**
To address this resource limitation, our framework implements a zero-overhead feedback loop that optimizes latency and power purely through silicon-level hardware knobs: Dynamic Voltage and Frequency Scaling (DVFS) clock scaling and Core Affinity pinning. This approach avoids the massive latency spikes and memory overhead associated with on-the-fly model re-quantization. 

Furthermore, this research directly addresses critical development challenges in developing nations like Indonesia. In rural or remote (3T) regions, internet connectivity is highly volatile and centralized cloud server costs are prohibitive. Deploying a low-cost, energy-efficient public fog network on existing consumer devices or cheap single-board computers allows local communities to run crucial AI services—such as smart agricultural monitoring or early landslide detection—locally and reliably, bridging the digital divide.

---

### **3. Proposed Methods**

#### **Approach / Methodology**
The project will implement a bidirectional runtime feedback loop between client devices and the global network orchestrator. The local client device executes the Edge AI model, monitors its own battery decay slope and thermal telemetry, and packages this data into a lightweight telemetry packet. This packet is periodically transmitted to the global orchestrator, which dynamically updates the Markov chain transition probabilities of the network scheduler, enabling proactive task redistribution before a local node crashes.

#### **Experimental Design and Investigation**
We will establish a **Dual-ISA Heterogeneous Testbed** to profile diverse architectures:
- An ARM64-based **Apple MacBook M1 (8GB)** to profile mobile-class, energy-efficient architectures.
- An x86_64-based **AMD Ryzen 5 laptop** (running Linux) to profile standard consumer and desktop-class nodes.

*All physical profiling equipment is provided by the applicant*, representing zero initial infrastructure cost to QUT.

#### **Data Collection and Validation**
For the micro-layer, we will compile and deploy benchmark models—including **YOLOv11**, **Ministral 3B**, and **PP-OCR Mobile**—using CPU/GPU-optimized runtimes (TensorFlow Lite, ONNX Mobile, and llama.cpp). Power consumption will be measured natively using macOS `powermetrics` and Linux `sysfs/powercap` (RAPL interfaces) to avoid the need for external hardware meters. 

For macro-layer validation, the collected power and thermal traces will be loaded into a custom discrete-event network simulator (using Python `SimPy` or `PureEdgeSim`) to test the proposed scheduler against baseline algorithms across a simulated cluster of 500 volatile nodes.

#### **Access to External Facilities**
None required. All hardware testing and cluster simulation software will be executed on the investigator’s local computational infrastructure.

---

### **4. Industry Engagement**
Given the 1.5-year timeline of the MPhil program, formal long-term internships are not feasible. Instead, the project will actively engage with open-source edge computing consortiums and tech vendors maintaining edge runtimes (such as Linaro and the ONNX Runtime steering groups). This ensures that the hardware-tuning methodologies remain aligned with real-world industry deployment standards. Additionally, knowledge-sharing workshops will be conducted with Indonesian IoT and agricultural tech firms (such as Mertani and Banwibu) to discuss practical edge deployments.

---

### **5. Project Alignment**
This project directly aligns with the **QUT Centre for Data Science**, a flagship research centre focusing on data-driven decision-making. The project's methodology, which combines statistical online learning at the edge with stochastic operations research (Markov chains) at the network layer, fits perfectly within the Centre's core themes. It also aligns with the distributed systems and information architectures track within the **School of Information Systems**.

---

### **6. Approvals and Permits**
**Not Applicable / None Required.** The project relies strictly on open-source software models, mathematical simulations, and the applicant's existing computing hardware, involving no human participants, animal subjects, or restricted dual-use technologies.

---

### **7. References**
1. Battula, S. K., Naha, R. K., & Garg, S. (2026). A Resource Selection Model for Minimization of Disruptions in Public Fog Computing Environments. *IEEE Transactions on Services Computing*, (In Press).
2. Nabhaan, A. N. L., Sukma, Z., Rachmanto, R. D., Santriaji, M. H., Cho, B., Setyanto, A., & Kim, I. K. (2026). CORAL: Covariance-Guided Resource Adaptive Learning for Efficient Edge Inference. *arXiv preprint arXiv:2603.14577*.
3. Rachmanto, R. D., Sukma, Z., Nabhaan, A. N. L., Setyanto, A., Jiang, T., & Kim, I. K. (2024). Characterizing Deep Learning Model Compression with Post-Training Quantization on Accelerated Edge Devices. In *2024 IEEE International Conference on Edge Computing and Communications (EDGE)* (pp. 110-120). IEEE.
4. Nabhaan, A. N. L., Rachmanto, R. D., & Setyanto, A. (2024). Characterizing Hardware Utilization on Edge Devices when Inferring Compressed Deep Learning Models. *MATRIK: Jurnal Manajemen, Teknik Informatika dan Rekayasa Komputer*, 24(1), 25-38.

---

### **8. Research Project Timeline**

| Timeframe | Research Activities |
| :--- | :--- |
| **0–3 Months** | Project design and contextualization; complete mandatory QUT HDR inductions; finalize initial literature synthesis on stochastic scheduling and Edge AI workloads. |
| **3–6 Months** | Establish the Micro-level testbed on the MacBook M1 and AMD Ryzen laptops; deploy YOLOv11, Ministral 3B, and PP-OCR Mobile; profile and collect the ground-truth power/thermal trace dataset. |
| **6–12 Months** | Construct the discrete-event network simulator; implement the bidirectional telemetry feedback channel; write the code to dynamically update the Markov chain transition matrix based on incoming device stress metrics. |
| **12–15 Months** | Run large-scale cluster co-simulations; evaluate performance metrics (disruption rates, SLA violations, energy footprints) against baseline models; prepare and submit two core manuscripts to peer-reviewed IEEE/ACM venues. |
| **15–18 Months** | Compile and draft the final MPhil thesis chapters; execute iterative review cycles with Dr. R. Naha and the supervisory panel; formal thesis submission for examination. |
