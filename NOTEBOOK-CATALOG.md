# Notebook Catalog — FGCU Quantum Hackathon 2026

**Florida Gulf Coast University | Qiskit Fall Fest 2026**

**Hackathon work period:** October 30, 2026, at 1:30 p.m. – November 6, 2026, at 8:00 a.m.

**All times are Eastern Time (America/New_York).**

**Registration and submissions:** [Deepstation.ai](https://deepstation.ai) via <https://tinyurl.com/fgcu-quantum>. If prompted, enter **QUANTUMEAGLE**.

**Final deliverables:** upload a project video **no longer than 15 minutes** and submit your **GitHub project repository link** through Deepstation.ai by **November 6, 2026, at 8:00 a.m.** See §8 and the [Participant Handbook](PARTICIPANT_HANDBOOK.md).

This catalog brings together IBM Quantum Learning resources and examples hosted in the Qiskit documentation, including partner tutorials. The ratings describe how much coding is involved, so team members can choose resources suited to their experience and project roles. Use the examples as references for your own domain project and acknowledge any code or materials you adapt.

> **All FGCU teams participate in the Domain track.** Technical development, coding, tools, domain analysis, and communication are contributions within the same project. Sections 1, 2, and 4 support exploration and problem framing; sections 3 and 5 support implementation and experiments. Choose resources according to your role, rather than treating them as separate tracks.

---

## How to read the ratings

| | Means |
|---|---|
| 🟢 **No code** | Interactive or visual. Nothing to install, nothing to type. |
| 🟡 **Click Run** | A notebook you execute cell by cell. You read the explanations, press Run, look at the output. No editing required. |
| 🟠 **Read code** | Worth reading even if you don't write Python. Follow the narrative, skip the implementation. |
| 🔴 **Write code** | You will edit and debug code as part of your team's domain project. |

---

## 1. Start here — zero code required

**🟢 [IBM Quantum Composer](https://quantum.cloud.ibm.com/composer)**
Drag-and-drop circuit builder. Place gates on a circuit and watch the state visualizations respond in real time. Run it on real hardware with a button. *This is the single highest intuition-per-minute resource that exists and it requires nothing but a browser and an IBM Quantum account.* Twenty minutes here will make every subsequent conversation easier. It is useful for team members working on implementation as well as those framing the domain problem.

**🟢 [Superposition](https://quantum.cloud.ibm.com/learning/en/modules/quantum-mechanics/superposition-with-qiskit)**
A short teaching module on the property that makes quantum different. Explains *what superposition actually is*, which is not the "both at once" cliché you've heard.

**🟢 [Quantum teleportation](https://quantum.cloud.ibm.com/learning/en/modules/computer-science/quantum-teleportation)**
Despite the name, no matter is transported anywhere. This is about moving quantum *information*, and it's the most memorable demonstration of why entanglement is a resource rather than a curiosity.

**🟢 [Quantum key distribution](https://quantum.cloud.ibm.com/learning/en/modules/computer-science/quantum-key-distribution)**
Using quantum statistics to detect an eavesdropper. Directly relevant to anyone thinking about security and policy — and one of the few areas with genuine near-term deployment.

**🟢 [Uncertainty](https://quantum.cloud.ibm.com/learning/en/modules/quantum-mechanics/exploring-uncertainty-with-qiskit)**
Where measurement uncertainty comes from. Useful background for understanding why quantum results are probability distributions rather than answers.

Full module library: <https://quantum.cloud.ibm.com/learning/modules>

---

## 2. Domain and industry notebooks

**This is the section to read if you're bringing industry expertise.** These are end-to-end examples of quantum methods pointed at recognisable commercial problems. Several are built by quantum software companies rather than IBM, which makes them useful in a second way: you can see how the industry frames its own value proposition, and judge it.

Read them for *how the problem is set up* — what got simplified, what constraints were kept, what the comparison baseline was. That critical reading is exactly the skill your team will need from you.

### Finance

**🟠 [Dynamic portfolio optimization](https://quantum.cloud.ibm.com/docs/en/tutorials/global-data-quantum-optimizer)** *(Global Data Quantum)*
Multi-period portfolio construction as a quantum optimization problem. The most directly recognisable finance example in the catalog. Read the problem formulation section and ask yourself which real-world constraints are missing.

**🟠 [Solve the Market Split problem](https://quantum.cloud.ibm.com/docs/en/tutorials/solve-market-split-problem-with-iskay-quantum-optimizer)** *(Kipu Quantum)*
A classic hard combinatorial problem with direct commercial analogues in allocation and division.

### Energy and utilities

**🟠 [Hybrid quantum-enhanced ensemble classification — grid stability](https://quantum.cloud.ibm.com/docs/en/tutorials/sml-classification)**
A machine learning workflow applied to power grid stability. Good example of the hybrid pattern: classical does most of the work, quantum handles one piece.

### Chemistry, materials, and pharma

**🟠 [Dissociation PES curves with HiVQE](https://quantum.cloud.ibm.com/docs/en/tutorials/qunova-hivqe)** *(Qunova)*
Potential energy surfaces — the computation underneath reaction and binding prediction. This is the application category with the strongest theoretical case for quantum advantage.

**🟠 [Sample-based quantum diagonalization of a chemistry Hamiltonian](https://quantum.cloud.ibm.com/docs/en/tutorials/sample-based-quantum-diagonalization)**
One of the more current approaches to chemistry on near-term hardware.

**🟠 [Implicit solvent calculations](https://quantum.cloud.ibm.com/docs/en/tutorials/implicit-solvent-calculations)**
Modelling molecules in solution rather than in a vacuum — the step that makes chemistry simulation relevant to drug discovery rather than a physics exercise.

### Engineering and simulation

**🟠 [Model a flowing non-viscous fluid — QUICK-PDE](https://quantum.cloud.ibm.com/docs/en/tutorials/colibritd-pde)** *(ColibriTD)*
Partial differential equations, which underlie fluid dynamics, structural analysis, heat transfer, and a large fraction of engineering simulation.

**🟠 [Simulate neutron scattering in quantum materials](https://quantum.cloud.ibm.com/docs/en/tutorials/simulate-neutron-scattering)**
Materials characterisation. Relevant to anyone in advanced manufacturing or materials R&D.

### General optimization

**🟠 [Higher-order binary optimization](https://quantum.cloud.ibm.com/docs/en/tutorials/solve-higher-order-binary-optimization-problems-with-q-ctrls-optimization-solver)** *(Q-CTRL)*
A general-purpose optimization solver. Useful for seeing what shape a problem has to be in before it can be handed to one of these.

---

## 3. Core algorithms

Use these algorithms and workflows as technical components of your Domain track project. Team members can read the problem formulation and results even if they are not writing the code.

**🟡 [CHSH inequality](https://quantum.cloud.ibm.com/docs/en/tutorials/chsh-inequality)**
IBM's designated first tutorial, and a good choice: you run an experiment on a real quantum computer that demonstrates the universe is not classical. Nobel-prize physics, executed from your browser in about ten minutes. **If you run one notebook this whole event, run this one.**

**🟡 [Hello world / your first circuit on hardware](https://quantum.cloud.ibm.com/docs/en/guides/hello-world)**
The complete end-to-end loop: build, transpile, submit, retrieve, interpret. Every project you write will follow this skeleton.

**🟠 [Grover's algorithm](https://quantum.cloud.ibm.com/docs/en/tutorials/grovers-algorithm)**
Quantum search. The famous quadratic speedup. Read the introduction for a clear statement of what the speedup is and — importantly — what it isn't.

**🟠 [Shor's algorithm](https://quantum.cloud.ibm.com/docs/en/tutorials/shors-algorithm)**
Integer factoring. The one everybody has heard of because of cryptography. Read this before you say anything in public about quantum and encryption; the resource requirements section is the reality check.

**🔴 [Quantum approximate optimization algorithm (QAOA)](https://quantum.cloud.ibm.com/docs/en/tutorials/quantum-approximate-optimization-algorithm)**
A starting point for domain projects involving scheduling, routing, allocation, or another optimization problem.

**🔴 [Advanced techniques for QAOA](https://quantum.cloud.ibm.com/docs/en/tutorials/advanced-techniques-for-qaoa)** · **🔴 [Warm-start QAOA](https://quantum.cloud.ibm.com/docs/en/tutorials/warm-start-qaoa)**
Follow-ups for teams going deep on optimization.

**🔴 [Ground-state energy estimation with VQE](https://quantum.cloud.ibm.com/docs/en/tutorials/spin-chain-vqe)**
The variational pattern. The foundation for most chemistry and materials work.

**🔴 [Quantum kernel training](https://quantum.cloud.ibm.com/docs/en/tutorials/quantum-kernel-training)** · **🔴 [Projected quantum kernels](https://quantum.cloud.ibm.com/docs/en/tutorials/projected-quantum-kernels)**
Quantum machine learning. Consider these examples for domain projects involving classification, prediction, or quantum feature maps.

---

## 4. Reading a notebook when you can't read the code

A genuine skill, and one you can pick up in the next ten minutes. Notebooks alternate between prose cells and code cells. **The prose is the paper; the code is the appendix.**

**The method:**

1. **Read the title and opening section.** What problem, why it matters. Often this is all you need.
2. **Scroll straight to the plots and tables at the bottom.** The results. What did it produce and what's on the axes?
3. **Now go back and read only the prose cells.** Skip every grey code block entirely. Most well-written notebooks remain fully coherent this way — that's what the prose is for.
4. **Look for the numbers that matter to you:** How many qubits? How many shots? What was it compared against? How long did it take?
5. **Find the limitations paragraph.** Almost every honest notebook has one, usually near the end. This is frequently the most valuable content in the document.

**The four questions to ask of any notebook:**

- **How big was the problem, really?** Look for qubit counts and instance sizes. Compare mentally to what a real instance in your field would be. The gap is the story.
- **What was it compared to?** If there's no classical baseline, no claim about advantage can be supported, full stop.
- **What was simplified away?** Every notebook simplifies. Which of those simplifications would your industry find unacceptable?
- **What would it take to be useful?** Sometimes stated. Often it's the thing you can contribute by working it out.

If you can answer those four questions about a notebook, you understand it better than someone who ran every cell without thinking about it.

---

## 5. How to actually run these

Ranked by how likely you are to succeed on the first try.

| Method | Setup | Best for |
|---|---|---|
| **[IBM Quantum Learning](https://quantum.cloud.ibm.com/learning)** in-browser | None | Course lessons. Already connected to your account. |
| **[Google Colab](https://colab.research.google.com)** | One `pip` line | Everything else, if you don't want a local install |
| **Local Jupyter** | See [Participant Handbook](PARTICIPANT_HANDBOOK.md), §5.2 | Project work, offline work, persistent environments |

**Colab recipe.** Download the notebook (`.ipynb`) from the tutorial page, upload it to Colab, and add a new first cell:

```python
!pip install qiskit qiskit-ibm-runtime matplotlib pylatexenc
```

Run the cells in order, checking the outputs and understanding which cells submit jobs to hardware. Develop and debug on a simulator before using QPU time. Colab sessions time out and lose state, so save your work to GitHub. Never hardcode your IBM API key in a Colab notebook.

**Circuit drawings failing?** You're missing `pylatexenc`. Install it, restart the kernel.

**Everything failing on a tutorial you found elsewhere?** Check the date. Anything with `channel="ibm_quantum"`, `IBMQ.load_account()`, `execute()`, or `qiskit.Aer` predates the current API and will not run. See Handbook §4.1.

---

## 6. Picking by domain project

These are suggested starting points, not separate competition tracks. Select a domain problem first, then choose a method that fits it. A tool, visualizer, library, or platform should demonstrate its value through a specific domain use case.

| Your project is about... | Read these, in order |
|---|---|
| **Scheduling, routing, allocation** | Higher-order binary optimization → QAOA → Market Split → Advanced QAOA |
| **Finance and portfolios** | Dynamic portfolio optimization → QAOA → Market Split |
| **Chemistry, drugs, materials** | Dissociation PES curves → Sample-based diagonalization → Spin-chain VQE → Implicit solvent |
| **Classification and prediction** | Grid stability classification → Quantum kernel training → Projected quantum kernels |
| **Engineering simulation** | QUICK-PDE fluid → Neutron scattering |
| **Security, crypto, policy** | Quantum key distribution → Shor's algorithm → CHSH inequality |
| **"I want to understand what this is"** | Composer → Superposition → CHSH inequality → Teleportation |
| **"I want a hardware reality check"** | [Probabilistic error amplification](https://quantum.cloud.ibm.com/docs/en/tutorials/probabilistic-error-amplification) → [Repetition codes](https://quantum.cloud.ibm.com/docs/en/tutorials/repetition-codes) → [Real-time benchmarking](https://quantum.cloud.ibm.com/docs/en/tutorials/real-time-benchmarking-for-qubit-selection) |

---

## 7. Complete official sources

- **Tutorials:** <https://quantum.cloud.ibm.com/docs/en/tutorials>
- **Courses:** <https://quantum.cloud.ibm.com/learning/en/courses>
- **Teaching modules:** <https://quantum.cloud.ibm.com/learning/modules>
- **Guides and how-tos:** <https://quantum.cloud.ibm.com/docs/guides>
- **API reference:** <https://quantum.cloud.ibm.com/docs/api>
- **Qiskit YouTube:** <https://www.youtube.com/qiskit>

For any event-specific starter materials, follow the links provided by the FGCU organizers. Use the [Participant Handbook](PARTICIPANT_HANDBOOK.md) for FGCU event rules, team requirements, and submission instructions.

---

## 8. Turning a notebook into your FGCU project

A tutorial is a starting point. Explain what your team changed, why it fits your domain problem, and what the results show.

1. **Define the domain problem.** Identify the users, constraints, and a result that would be useful to them.
2. **Select and adapt an example.** Explain the quantum method and how the tutorial's assumptions relate to your use case. Cite the original tutorial and distinguish your team's contributions.
3. **Run and interpret the work.** Record the experiment settings and outputs. Clearly label simulator and hardware results, compare with a classical approach where appropriate, and state limitations.
4. **Prepare the GitHub project.** Include the README, relevant notebooks or source code, setup instructions, domain analysis, results, and limitations. Ensure that judges can access it.
5. **Complete the final submission through Deepstation.ai.** Upload the project video and submit the GitHub repository link by the deadline below.

### Final submission checklist

**Deadline: November 6, 2026, at 8:00 a.m. Eastern Time.**

- [ ] Prepare a project video **no longer than 15 minutes**, including any demo.
- [ ] Cover the motivation, domain problem, quantum approach, demo or analysis, results, limitations, and team contributions.
- [ ] **Upload the video to Deepstation.ai.**
- [ ] **Submit your GitHub project repository link through Deepstation.ai.**
- [ ] Verify that judges can access both the video and repository, and complete the submission process before the deadline.

**Deepstation.ai is the only platform for final submissions.** A GitHub repository or pull request alone does not complete your submission. Slides do not replace the video.

### Closing ceremony sharing presentation

The closing ceremony is on **November 6, 2026, from 1:30–4:15 p.m.**, at **Sugden Hall, Room 114**, 10501 FGCU Blvd S, Fort Myers, FL 33965.

Each team must prepare a **10-minute sharing presentation, including a demo**, for the **1:30–3:00 p.m.** presentation session. This is separate from the uploaded video of up to 15 minutes. The sharing presentation **does not affect final scores**, but attendance and participation in this session are required to receive a **participation certificate**.

---

*Found a useful resource or a broken link? Let the FGCU organizing team know through the event chat listed in the Participant Handbook.*
