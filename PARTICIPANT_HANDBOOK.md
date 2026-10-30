# Participant Handbook

**FGCU Quantum Hackathon 2026 | Qiskit Fall Fest 2026**

**Hackathon work period: October 30, 2026, 1:30 p.m. – November 6, 2026, 8:00 a.m.**

**All times are Eastern Time (America/New_York).**

---

## Contents

- [0. Quick start](#0-quick-start)
- [1. About the event](#1-about-the-event)
- [2. Project guide](#2-project-guide)
- [3. Participation and teamwork](#3-participation-and-teamwork)
- [4. IBM Quantum Platform account](#4-ibm-quantum-platform-account)
- [5. Get Qiskit running](#5-get-qiskit-running)
- [6. GitHub and final submission](#6-github-and-final-submission)
- [7. Learning resources](#7-learning-resources)
- [8. Event schedule](#8-event-schedule)
- [9. Troubleshooting](#9-troubleshooting)
- [10. Support and community](#10-support-and-community)
- [11. Accessibility hardware and cost](#11-accessibility-hardware-and-cost)
- [12. Frequently asked questions](#12-frequently-asked-questions)
- [Appendix A. Glossary](#appendix-a-quantum-computing-glossary)
- [Appendix B. Checklist](#appendix-b-preparation-and-submission-checklist)
- [Appendix C. Use-Case Canvas](#appendix-c-use-case-canvas)

---

## 0. Quick start

The **FGCU Quantum Hackathon** starts on **October 30, 2026, at 1:30 p.m.** Final submissions are due on **November 6, 2026, at 8:00 a.m. Eastern Time**.

Teams consist of **2–4 students**. Students from all majors and experience levels are welcome. No prior quantum computing experience is required. Teams combine problem framing, quantum computing, technical development, evaluation, and communication according to their project needs.

**Before kickoff:**

- [ ] Register through [Deepstation.ai](https://deepstation.ai) using <https://tinyurl.com/fgcu-quantum>. If prompted, enter **QUANTUMEAGLE**.
- [ ] Join the [event chat](https://discord.gg/uN6WDVuXw).
- [ ] Create an IBM Quantum Platform account (§4) and a GitHub account (§6).
- [ ] Read §2 and §3, and bring an initial problem or application idea.
- [ ] If you will implement circuits or code, review §5 and test your environment.

**Before the submission deadline:** upload a **project video of no more than 15 minutes** and submit your **GitHub project repository link** through **Deepstation.ai**. See §6.4 for details. A GitHub repository or pull request alone does not complete your submission.

---

## 1. About the event

Qiskit Fall Fest is a worldwide, student-led series of quantum computing events run in partnership with IBM Quantum. Hosts on campuses and in communities around the world run their own hackathons, workshops, and challenges under one banner during the autumn.

The **2026 theme is "a decade of quantum on the cloud"**: it marks ten years since IBM put the world's first open-access quantum computer on the internet. Ten years ago, running a circuit on real quantum hardware meant knowing someone in a lab. Today you do it from a browser tab, for free, in about four minutes. That shift is the entire reason this event can exist, and it's a useful thing to keep in mind when you're deciding how ambitious to be.

Florida Gulf Coast University (FGCU) is running the **FGCU Quantum Hackathon** as part of that lineup.

Official IBM announcement: <https://www.ibm.com/quantum/blog/qiskit-fall-fest-2026>

---

## 2. Project guide

A hackathon project should explore how quantum computing could address a specific problem. You are not expected to prove quantum advantage during the event. Keep claims proportional to the evidence you produce.

A strong Qiskit Fall Fest project is one of these:

1. **A mapped problem.** Take a real problem from a real industry, show precisely how it becomes something a quantum computer could work on (a QUBO, a Hamiltonian, a kernel), run it small on hardware or simulator, and be honest about what would need to change to make it matter. This is where having someone with experience in the relevant field is helpful. 
2. **A benchmark or comparison.** Run the same problem classically and quantumly at small scale. Show where the crossover *might* be and what's blocking it.
3. **A useful tool.** Build a visualizer, a translator from application data into a circuit, a teaching aid, or another tool that makes quantum work easier. Show how it serves a specific application or audience within your project.
4. **An analysis.** A rigorous, sourced assessment of where quantum does or doesn't fit in a specific sector, with the technical claims actually checked against what current hardware can do.

Projects may emphasize implementation, comparison, tools, or analysis, but each must explain the problem, quantum approach, evidence, and limitations. Build the project through collaboration across your team. See §3 for suggested roles.

**Judging criteria:** consult the rubric and scoring information provided by the organizers on [Deepstation.ai](https://deepstation.ai). Explain the relevance of your problem, your quantum approach and technical evidence, and the limitations of your results. The submitted video and GitHub project are the final materials for evaluation; the closing ceremony sharing presentations do not affect final scores.

### 2.1 Connecting an idea to a useful project

A quantum method is useful to a project only when it addresses a clearly defined problem. A portfolio model may need transaction costs; a routing model may need vehicle capacity or working-hour limits; a healthcare model may need privacy and resource constraints.

Define who faces the problem, what a useful result would look like, and which assumptions your model makes. Use the **Use-Case Canvas in Appendix C** to organize the idea before or during team formation.

### 2.2 Three starting points for quantum applications

| Pattern | What to explore | Example problems | What to evaluate |
|---|---|---|---|
| Optimization | Choosing among many combinations under constraints | Scheduling, routing, resource allocation, portfolio construction | Problem size, constraints, solution quality, and a classical baseline |
| Simulation | Representing a quantum system such as a molecule or material | Chemistry, catalysts, batteries, materials | Model assumptions, system size, and the limits of the demonstration |
| Learning and data | Using quantum circuits in a data analysis or learning workflow | Classification, anomaly detection, risk scoring | Data preparation, comparison methods, prediction quality, and resource costs |

These patterns help you choose a method. A well-supported conclusion that a quantum approach does not fit a problem can also be a useful project outcome.

Start with three ideas:

- **Problem structure matters:** explain why the selected method is relevant.
- **Evidence has limits:** a small experiment does not by itself establish a practical advantage.
- **Workflows can be hybrid:** explain what the classical and quantum parts each do.

### 2.3 Industry and application examples

Use these examples to develop your own question, constraints, and evaluation plan. They are suggested topics, not required assignments.

**Financial services**: portfolio rebalancing under transaction costs and regulatory capital constraints | derivative pricing with path-dependent payoffs | collateral optimization across netting sets | fraud detection on sparse labelled data | credit risk with correlated defaults

**Logistics and supply chain**: multi-depot vehicle routing with driver-hours regulations | container loading and stowage | warehouse slotting under seasonal demand | resilient network design under disruption scenarios | last-mile consolidation

**Energy and utilities**: unit commitment across a mixed generation fleet | grid stability classification | optimal placement of storage on a distribution network | battery electrolyte chemistry | demand response scheduling across heterogeneous loads

**Pharma and healthcare**: protein-ligand binding affinity | reaction pathway analysis for synthesis planning | clinical trial site selection and patient allocation | operating theatre and staff scheduling | molecular property prediction with scarce data

**Manufacturing and materials**: catalyst discovery | production line sequencing with changeover costs | alloy and composite property prediction | predictive maintenance scheduling under spare-parts constraints | high-temperature superconductor screening

**Telecommunications**: spectrum allocation | network topology under redundancy requirements | antenna placement and beamforming | traffic routing under QoS constraints | post-quantum cryptography migration planning

**Agriculture and food**: crop rotation planning under soil, water, and market constraints | cold chain routing | fertilizer chemistry and nitrogen fixation catalysis | yield prediction from sparse sensor data

**Public sector and policy**: emergency service positioning | public transport network design | vaccine and resource distribution under equity constraints | infrastructure investment sequencing | post-quantum cryptography readiness across government systems

**Insurance**: catastrophe risk modelling with correlated events | reinsurance portfolio structuring | claims triage | pricing in thin-data segments

**Aerospace and defence**: trajectory optimization | satellite constellation scheduling and tasking | structural and materials design | sensor fusion under uncertainty

#### Optional Southwest Florida starting points

You may explore problems such as post-hurricane resource distribution, emergency vehicle or drone routing, hospital staff scheduling, water and agricultural resource allocation, or cybersecurity anomaly detection. These are examples, not required topics. Choose a small instance that your team can model, evaluate, and explain during the hackathon.

### 2.4 Making claims that your evidence supports

**Choose an appropriate scope.** A small demonstration can be a useful project when the problem, method, and limits are clear. Explain how its scale differs from a realistic application.

**Distinguish simulation and hardware.** State where each result came from, how the experiment was configured, and which uncertainties remain.

**Use meaningful comparisons.** A result on one small instance does not establish quantum advantage. Explain the classical baseline and the evidence needed for any claimed improvement.

**Check security claims carefully.** Distinguish quantum algorithms, quantum key distribution, and post-quantum cryptography. Explain the threat model and assumptions relevant to your project rather than making predictions about when encryption will fail.

**State assumptions about future use.** Identify what would need to change for the approach to become useful, without treating a vendor roadmap or a projected benefit as a demonstrated result.

**Report negative findings honestly.** If a quantum method does not fit your problem, explain the analysis and evidence that led to that conclusion.

---

## 3. Participation and teamwork

Students from **all majors and experience levels** can contribute. No prior quantum computing knowledge is required.

- **Computing, software engineering, and mathematics:** implement algorithms, develop tools, test circuits, and analyze results.
- **Business, finance, and operations:** identify decision problems, define constraints, and assess practical value.
- **Engineering, science, healthcare, and agriculture:** connect methods to models, data, and realistic requirements.
- **Policy, law, and social sciences:** examine governance, privacy, feasibility, and implications for users.
- **Design, communication, and other fields:** develop explanations, visualizations, demos, and clear project materials.
- **Beginners:** research the problem, explore Composer, read notebooks, document experiments, and ask questions.

These examples do not limit your role. A student from any major may learn the technical tools, and a programmer may lead problem framing or communication.

Not every team member needs to install Python. Team members doing implementation should review §5; others can contribute through research, circuit exploration in Composer, evaluation, documentation, and presentation.

Choose roles according to your team's strengths and learning goals. A team of **2–4 students** does not need a different person for every role below.

### Problem Lead

Define the problem, intended users, and practical constraints. Check whether modelling assumptions are appropriate.

*Contribution:* a clear use-case description in `USE-CASE.md` or the README.

### Problem Framer

Translate the use case into variables, constraints, objectives, and a manageable experiment. Work with teammates on the quantum formulation.

*Contribution:* a problem model that explains what is represented and what is simplified.

### Quantum and Technical Developer

Implement Qiskit code or circuits, run simulations or hardware experiments, and build any supporting tools or visualizations. Connect the implementation to the use case.

*Contribution:* relevant source code, notebooks, experiment settings, results, and setup instructions in the team's GitHub repository.

### Evaluation and Feasibility Analyst

Interpret the outputs, compare with a classical approach where appropriate, and identify the gap between the demonstration and a realistic application.

*Contribution:* supporting evidence, results, and limitations, with assumptions stated clearly.

### Presentation and Demo Lead

Coordinate the story, visuals, video, and demonstration with the whole team. Ensure that claims match the evidence.

*Contribution:* a submitted project video **no longer than 15 minutes** and a separate **10-minute closing ceremony sharing presentation**, including a demo.

### Policy and Risk Analyst

Examine relevant privacy, security, ethical, regulatory, and operational constraints.

*Contribution:* a discussion of risks and limitations in `LIMITATIONS.md`, `USE-CASE.md`, or the README.

### Practical Value Reviewer

Ask who would use the result, what makes it useful, what assumptions it depends on, and what further work would be needed.

*Contribution:* questions and evidence that help the team refine its use case and conclusions.

Team members should work together throughout the hackathon, using the results of implementation, research, and evaluation to refine the project.

---

## 4. IBM Quantum Platform account

**Everyone creates an account. It takes about ten minutes and it is free.**

Your IBM Quantum account is what gives you (a) access to real quantum computers, (b) the full IBM Quantum Learning course library with in-browser code, and (c) the Composer, a drag-and-drop circuit editor that requires no coding at all.

### 4.1 Create the account

1. Go to <https://quantum.cloud.ibm.com/registration>
2. Sign up with an IBMid or a Google account. If you don't have an IBMid, the flow creates one for you.
3. You'll land on the IBM Quantum Platform dashboard.

> ⚠️ **Heads up on stale instructions.** IBM Quantum Platform moved to IBM Cloud, and the old `docs.quantum.ibm.com` platform was retired on 1 July 2025. If you find a blog post, a YouTube video, or a Fall Fest guide from a previous year that tells you to go to `quantum-computing.ibm.com`, or shows code with `channel="ibm_quantum"`, **it is out of date and will not work.** Use `quantum.cloud.ibm.com` and this handbook.

### 4.2 Create an instance

An *instance* is your allocation of quantum compute. Your account needs at least one.

1. Go to <https://quantum.cloud.ibm.com/instances>
2. Create an instance on the **Open Plan**.
3. Note that Open Plan instances can only be created in the **us-east** region. If your account switcher is set to `eu-de`, switch it.

### 4.3 Get your API key if you will access hardware through code

Team members using the hardware API should complete this step. Other team members can continue to §6 after reviewing the available tools.

1. From the dashboard at <https://quantum.cloud.ibm.com/>, create your API key.
2. **Copy it immediately to a password manager. It is shown once and never again.** It's a 44-character string.
3. Also copy your instance's **CRN** (Cloud Resource Name) from the Instances page — hover over the CRN and click the copy icon.

> Your API key is a credential. Do not paste it into a notebook you're going to commit to GitHub. Do not paste it in the event chat. §5.4 shows you how to store it properly. If you leak it, revoke it from the dashboard and make a new one.

### 4.4 Understand your quantum time budget

The Open Plan gives you **up to 10 minutes of QPU time per rolling 28-day window**, free. Monitor usage on the dashboard and on the [Workloads page](https://quantum.cloud.ibm.com/workloads).

Ten minutes sounds tiny. It is enormous. QPU time is measured in actual execution, and a typical small circuit run costs a couple of seconds. You can run hundreds of jobs. Teams almost never run out, but teams that leave a badly-parameterized loop running unattended absolutely do, so:

- **Develop against a simulator, submit to hardware only when the circuit is final.** (§5.5)
- Check the queue before you submit at 3am on deadline day.
- One person per team should own hardware submissions.

IBM also ran a limited-time promotion adding 180 extra minutes over 12 months for active Open Plan users ([details here](https://www.ibm.com/quantum/blog/open-plan-updates)). Check whether it's still available when you sign up — promotions change.

Full plan comparison: <https://quantum.cloud.ibm.com/docs/en/guides/plans-overview>

### 4.5 Classroom accounts (organizers)

If FGCU organizers want centralized management of participant access and work, IBM offers Classroom Accounts: <https://ibm.biz/classroom-account>. Apply well in advance.

---

## 5. Get Qiskit running

> **Use this section according to your role on the team.** Team members implementing circuits or code should complete the relevant setup. Members focusing on problem framing, analysis, or communication can explore the browser tools in §5.1 without a local installation.

We recommend **starting in the cloud** and only installing locally if you hit a reason to. Every hackathon loses hours to someone's broken conda environment. Don't be that hour.

### 5.1 Path A (recommended): browser, zero install

Three options, in order of how much we recommend them:

**IBM Quantum Learning (best starting point).** The course lessons at <https://quantum.cloud.ibm.com/learning> contain live code cells you run in the browser with your IBM Quantum account. Nothing to install, nothing to configure, and it's already wired to your account. Start with [Use a quantum computer today](https://quantum.cloud.ibm.com/learning/en/courses/use-a-qc-today).

**IBM Quantum Composer (zero code at all).** <https://quantum.cloud.ibm.com/composer> — drag gates onto a circuit, watch the state visualizations update live, run it. This is the single fastest way to build intuition for what a quantum circuit *is*. Recommended for all participants.

**Google Colab (for project work).** Free hosted Jupyter. Start any notebook with:

```python
!pip install qiskit qiskit-ibm-runtime matplotlib pylatexenc
```

Colab is the pragmatic choice for hackathon project work if you don't want to manage a local environment. Caveat: Colab sessions time out and lose state, so save to GitHub often, and don't hardcode your API key in a Colab notebook.

### 5.2 Path B: local install

Do this if you want a persistent environment, you're working offline, or you just prefer local tooling.

**Requirements:** Python 3.10 or later. (Qiskit 2.5.x supports 3.10 through 3.14.) 64-bit OS. Qiskit 2.x dropped 32-bit support entirely.

**macOS / Linux:**

```bash
# 1. Make a project folder and a virtual environment
mkdir fallfest && cd fallfest
python3 -m venv .venv
source .venv/bin/activate

# 2. Install everything in ONE pip command
pip install qiskit qiskit-ibm-runtime jupyter matplotlib pylatexenc numpy
```

**Windows (PowerShell):**

```powershell
mkdir fallfest; cd fallfest
python -m venv .venv
.venv\Scripts\Activate.ps1

pip install qiskit qiskit-ibm-runtime jupyter matplotlib pylatexenc numpy
```

Windows users on Git Bash: activate with `source .venv/scripts/activate` instead.

**Why these packages:**

| Package | What it's for |
|---|---|
| `qiskit` | The SDK itself: circuits, operators, transpiler, local simulators |
| `qiskit-ibm-runtime` | Talks to IBM's real quantum computers. Separate package. You need it. |
| `jupyter` | Notebooks |
| `matplotlib` + `pylatexenc` | Circuit diagrams and plots. Without `pylatexenc`, `circuit.draw('mpl')` fails with a confusing error. |

**Rules that will save you pain:**

1. **Always use a virtual environment.** Not optional. A polluted global Python is the #1 cause of hackathon environment failures.
2. **Install everything in a single `pip install` command.** Running pip repeatedly can produce an environment that resolves but is subtly broken.
3. **If you have an old Qiskit 0.x installation anywhere, do not try to upgrade it in place.** Make a fresh venv. Qiskit 1.0 changed the packaging structure and in-place upgrades from 0.x fail in ways that are genuinely hard to debug.

Official install guide: <https://quantum.cloud.ibm.com/docs/en/guides/install-qiskit>

### 5.3 Verify your install

Save this as `check_setup.py` and run it. It uses only the local simulator. No account needed, no QPU time consumed.

```python
"""Fall Fest environment check. Run: python check_setup.py"""
import sys

print(f"Python: {sys.version.split()[0]}")

import qiskit
print(f"Qiskit: {qiskit.__version__}")

try:
    import qiskit_ibm_runtime
    print(f"Runtime client: {qiskit_ibm_runtime.__version__}")
except ImportError:
    print("Runtime client: NOT INSTALLED  <-- run: pip install qiskit-ibm-runtime")

# Build a Bell state: two qubits, maximally entangled.
from qiskit import QuantumCircuit
from qiskit.primitives import StatevectorSampler

qc = QuantumCircuit(2)
qc.h(0)          # put qubit 0 into superposition
qc.cx(0, 1)      # entangle qubit 1 with qubit 0
qc.measure_all()

result = StatevectorSampler().run([qc], shots=1000).result()
counts = result[0].data.meas.get_counts()

print(f"Bell state counts: {counts}")
print("\nExpect roughly 500 '00' and 500 '11', and essentially no '01' or '10'.")
print("Those two outcomes being correlated and the other two being absent")
print("is entanglement. If you see that, your environment works.")
```

If that prints something like `{'00': 496, '11': 504}`, you are done. Go to §6.

### 5.4 Connect to real hardware for your project

Once, in a trusted environment (your own laptop, **not** a shared lab machine, **not** Colab):

```python
from qiskit_ibm_runtime import QiskitRuntimeService

QiskitRuntimeService.save_account(
    token="<your-44-character-API-key>",
    instance="<your-instance-CRN>",
    region="us-east",
    set_as_default=True,
)
```

This writes your credentials to a local config file. After that, every notebook just does:

```python
from qiskit_ibm_runtime import QiskitRuntimeService
service = QiskitRuntimeService()          # loads saved credentials
backend = service.least_busy(operational=True, simulator=False)
print(f"Using: {backend.name}")
```

On a shared or untrusted machine, don't save the account — pass the token explicitly each session, or follow the [untrusted environment guide](https://quantum.cloud.ibm.com/docs/en/guides/cloud-setup-untrusted).

The default channel is `ibm_quantum_platform` and you almost never need to specify it. Full detail: <https://quantum.cloud.ibm.com/docs/en/guides/initialize-account>

### 5.5 The one workflow rule

**Iterate on a simulator. Submit to hardware once.**

```python
# Local simulation — free, instant, unlimited
service = QiskitRuntimeService(channel="local")
```

Then switch to the real service only when your circuit is final. This is both a QPU-budget discipline and a sanity discipline: if your circuit is wrong, hardware noise will make the wrongness much harder to see.

Your first hardware run, step by step: <https://quantum.cloud.ibm.com/docs/en/guides/hello-world>

---

## 6. GitHub and final submission

**Every team needs a GitHub project repository.** Use it to collaborate on code, notebooks, use-case analysis, documentation, and slides. Team members can contribute according to their roles. Submit the repository link through Deepstation.ai together with your project video.

### 6.1 Create an account

1. Go to <https://github.com/signup>
2. Pick a username you'd be comfortable putting on a résumé. This is a public professional identity. `xX_quantum_slayer_Xx` will haunt you.
3. Verify your email address — GitHub blocks several actions until you do.
4. **Turn on two-factor authentication now**, at <https://github.com/settings/security>. GitHub requires 2FA for many contributors and it will interrupt you at the worst moment if you leave it. Use an authenticator app; save the recovery codes somewhere real.
5. Add a display name and a one-line bio. Judges and recruiters look at these.

**Students:** the [GitHub Student Developer Pack](https://education.github.com/pack) is free with a `.edu` address and includes Copilot and a pile of other tools. Apply now, not during the event, approval takes time.

### 6.2 Create your team project repository

1. Create a GitHub repository for your team project.
2. Invite your teammates as collaborators.
3. Add a README with the project title, team members, problem, approach, and instructions for reviewing or running the project.
4. Make sure the judges can access the repository by the submission deadline. If it is private, arrange reviewer access with the organizers in advance.

An invitation to an event GitHub organization or a pull request to a shared event repository is not required for final submission.

### 6.3 Suggested repository layout

The following is a suggested structure; adapt it to your project.

```text
your-team-project/
├── README.md                  ← project overview and run or review instructions
├── USE-CASE.md                ← problem and intended impact
├── notebooks/                 ← quantum experiments and analysis, if applicable
├── src/                       ← source code, if applicable
├── requirements.txt           ← dependencies, if applicable
├── results/                   ← figures, outputs, and supporting evidence
├── slides/                    ← optional presentation materials
└── LIMITATIONS.md             ← assumptions and limitations
```

### 6.4 Final submission through Deepstation.ai

**Deadline: November 6, 2026, at 8:00 a.m. Eastern Time.**

**Deepstation.ai is the only platform for final submissions.** Upload your video and submit your GitHub project link there by the deadline.

1. Open <https://tinyurl.com/fgcu-quantum> and sign in to [Deepstation.ai](https://deepstation.ai). If prompted for the event code, enter **QUANTUMEAGLE**.
2. Confirm your team and project information.
3. **Upload a project presentation video no longer than 15 minutes**, including any demo.
4. **Submit your GitHub project repository link.**
5. Complete the platform submission process and verify that the video and repository are accessible to the judges.

Creating a repository, pushing commits, or opening a GitHub pull request does not complete your final submission. Both the video and GitHub project link must be submitted through Deepstation.ai.

#### Project video content

Use the video to explain:

- **Motivation and problem:** what problem you address, who it affects, and why it matters.
- **Quantum approach:** how quantum computing fits the problem and what methods or tools you used.
- **Demo and results:** demonstrate the project or walk through the analysis, experiments, and outputs. Clearly distinguish simulation results from hardware results.
- **Evaluation and limitations:** explain what the evidence supports, any relevant classical comparison, and what remains unresolved.
- **Team contributions and next steps:** summarize what your team built or analyzed, what you learned, and potential improvements.

The **15-minute limit applies to the uploaded submission video**. The closing ceremony sharing presentation is a separate **10-minute presentation**, including a demo. See §8.

### 6.5 What belongs in your GitHub project

| Item | Requirement |
|---|---|
| `README.md` | Required: project title, team members, problem, quantum approach, results summary, and run or review instructions. |
| Source code or notebooks | Include all code and notebooks used in your project, where applicable. |
| Use-case analysis | Explain the use case, users, constraints, and intended impact in `USE-CASE.md` or the README. |
| Dependencies and setup | Include `requirements.txt` or equivalent setup instructions if the project contains code. |
| Results and supporting materials | Include the evidence needed to understand and review your conclusions. |
| Limitations | State assumptions and limitations in `LIMITATIONS.md` or the README. |
| Slides | Optional supporting material; slides do not replace the required video upload. |

Keep credentials and API keys out of the repository. Ensure that reviewers can follow your project without needing access to your personal accounts.

New to git? <https://docs.github.com/en/get-started>

---

## 7. Learning resources

Choose resources according to your role, available time, and project needs. You do not need to complete every course before the event. Start with an IBM Quantum account and Composer, review one or two relevant examples, and draft the Use-Case Canvas in Appendix C.

### Understanding the problem and its users

| Resource | Time | Why |
|---|---|---|
| [**Quantum business foundations**](https://quantum.cloud.ibm.com/learning/en/courses/quantum-business-foundations) | 3h | Built for exactly this audience. Ends in an exam and a Credly digital badge you can put on LinkedIn. **Start here.** |
| [**Designing and leading quantum projects**](https://quantum.cloud.ibm.com/learning/en/courses/designing-and-leading-quantum-projects) | 4h | For anyone who might actually have to sponsor or govern one of these. |
| [IBM Quantum Composer](https://quantum.cloud.ibm.com/composer) | 20 min | Play. Drag gates. No coding. Best intuition-per-minute available. |

### Quantum programming and technical development

| Resource | Time | Why |
|---|---|---|
| [**Use a quantum computer today**](https://quantum.cloud.ibm.com/learning/en/courses/use-a-qc-today) | 5h | The fastest on-ramp. IBM's own framing: *you don't need a physics degree or years of programming experience — if you can follow along with a notebook and click "Run," you're ready.* **Start here.** |
| [Basics of quantum information](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information) | 15h | John Watrous's course. The real foundation. Do the first two lessons before the event; finish it after. |
| [Quantum computing in practice](https://quantum.cloud.ibm.com/learning/en/courses/quantum-computing-in-practice) | 8h | 100+ qubit workloads and what actually works on today's hardware. |
| [Hello world guide](https://quantum.cloud.ibm.com/docs/en/guides/hello-world) | 30 min | Your first circuit on real hardware, end to end. |

### If you're going deep on a specific application

| Course | Time | For |
|---|---|---|
| [Variational algorithm design](https://quantum.cloud.ibm.com/learning/en/courses/variational-algorithm-design) | 8h | Optimization projects — the workhorse pattern |
| [Quantum machine learning](https://quantum.cloud.ibm.com/learning/en/courses/quantum-machine-learning) | 10h | Classification, kernels, feature maps |
| [Quantum chemistry with VQE](https://quantum.cloud.ibm.com/learning/en/courses/quantum-chem-with-vqe) | 5h | Molecules, materials, drug discovery |
| [Quantum diagonalization algorithms](https://quantum.cloud.ibm.com/learning/en/courses/quantum-diagonalization-algorithms) | 10h | VQE, Krylov, and the current state of the art |
| [Integrating quantum and HPC](https://quantum.cloud.ibm.com/learning/en/courses/integrating-quantum-and-high-performance-computing) | 6h | Hybrid workflows, realistic deployment |

Full catalog: <https://quantum.cloud.ibm.com/learning/en/courses>

### Notebooks

We've annotated the useful ones, including which are readable without running anything — in [`NOTEBOOK-CATALOG.md`](NOTEBOOK-CATALOG.md). Use it to identify examples relevant to your problem and your role.

---

## 8. Event schedule

**All times are Eastern Time (America/New_York).** The hackathon work period runs from **October 30, 2026, at 1:30 p.m.** to the final submission deadline on **November 6, 2026, at 8:00 a.m.**

**Venue for kickoff and the closing ceremony:** Sugden Resort & Hospitality Management Building, Room 114 (Sugden Hall), 10501 FGCU Blvd S, Fort Myers, FL 33965.

| Date | Time | Activity | Location |
|---|---|---|---|
| October 30, 2026 | 1:30–4:30 p.m. | Kickoff, quantum computing seminar, hackathon ideas, platform registration, judges introduction, and team formation | Sugden Hall, Room 114 |
| October 30–November 6, 2026 | During the hackathon work period | Team project development and collaboration | Team-arranged / online |
| November 6, 2026 | **8:00 a.m.** | **Final deadline: video of no more than 15 minutes and GitHub project link** | **Deepstation.ai** |
| November 6, 2026 | 8:00–11:30 a.m. | Judges review submitted projects and submit final scores | Online |
| November 6, 2026 | 1:30–3:00 p.m. | Team sharing presentations and demos, 10 minutes per team | Sugden Hall, Room 114 |
| November 6, 2026 | 3:00–3:30 p.m. | Judges reflections, evaluation criteria, and final scoring mechanism | Sugden Hall, Room 114 |
| November 6, 2026 | 3:30–4:00 p.m. | Awards ceremony: first, second, and third place; prizes, certificates, and trophies | Sugden Hall, Room 114 |
| November 6, 2026 | 4:00–4:15 p.m. | Closing remarks from the Department Chair and acknowledgments | Sugden Hall, Room 114 |

### Closing ceremony presentation and certificate requirement

Each team must prepare a **10-minute presentation, including a demo**, explaining its motivation, approach, results, and lessons learned. These presentations are for sharing and **do not affect final scores**.

All teams must present. Attendance and participation in this session are required to receive a **participation certificate**.

---

## 9. Troubleshooting

**`ModuleNotFoundError: No module named 'qiskit'`, but you definitely installed it.**
Your notebook kernel isn't the environment you installed into. Activate the venv *first*, then launch Jupyter from that same shell. If you're in Anaconda Navigator, use the "Applications on" dropdown to select your environment before launching.

**`ImportError` mentioning `qiskit-terra` or "invalid environment".**
You have Qiskit 0.x and 1.0+ colliding. This is not fixable in place. Delete the venv, make a new one, install once.

**Circuit drawing fails or renders as gibberish.**
`pip install pylatexenc matplotlib`, restart the kernel.

**`401 Unauthorized` when connecting to the service.**
Either the API key is wrong, or you're using a bearer token where the API key belongs. Regenerate the key from <https://quantum.cloud.ibm.com/> and re-run `save_account`.

**"No instance found" / can't see any QPUs.**
Check the region switcher at the top of the dashboard — Open Plan instances exist only in `us-east`. If you're looking at `eu-de`, you'll see nothing.

**Compilation errors during `pip install`.**
Your platform has no prebuilt wheel. Check you're on 64-bit Python 3.10+. Ask in the [event chat](https://discord.gg/uN6WDVuXw) before you start installing Rust toolchains.

**Jobs sitting in the queue forever.**
Normal at peak times — it's a shared fair-share queue. Use `service.least_busy(operational=True, simulator=False)` and check <https://quantum.cloud.ibm.com/computers>. Meanwhile, keep working against the local simulator.

**Code from a tutorial you found online just doesn't work.**
Check its date. Anything using `channel="ibm_quantum"`, `IBMQ.load_account()`, `execute()`, or `qiskit.Aer` predates the current API. See the warning in §4.1.

**Still stuck:** the [event chat](https://discord.gg/uN6WDVuXw), and post the actual error text, not "it doesn't work." Screenshots of terminals are harder to help with than pasted text.

---

## 10. Support and community

- **Registration and final submissions:** [Deepstation.ai](https://deepstation.ai) via <https://tinyurl.com/fgcu-quantum>; event code **QUANTUMEAGLE** if prompted.
- **Event chat:** <https://discord.gg/uN6WDVuXw>
- **Organizers:** contact the FGCU Quantum Hackathon organizing team through the event chat or during the in-person sessions.
- **Qiskit Slack:** <https://qisk.it/join-slack>, the global Qiskit community
- **Qiskit YouTube:** <https://www.youtube.com/qiskit>
- **Documentation:** <https://quantum.cloud.ibm.com/docs>
- **Quantum Computing Stack Exchange:** tag `qiskit`

Treat teammates, judges, and other participants respectfully. Raise conduct concerns with the FGCU organizing team.

---

## 11. Accessibility, hardware, and cost

- **No laptop?** Contact the organizing team before the event to discuss available options.
- **Weak laptop?** Everything in §5.1 runs in a browser. A Chromebook is sufficient.
- **Nothing here costs money.** Qiskit is open source (Apache 2.0). The IBM Quantum Open Plan is free. GitHub is free. If someone asks you to pay for something to participate, that's not us.
- **Accessibility needs:** contact the organizing team in advance to discuss accommodations.

---

## 12. Frequently asked questions

**Do I need to know Python?**  
Not every participant needs to code. Team members can contribute through problem framing, analysis, evaluation, documentation, and communication. Anyone interested can learn the technical tools and work with teammates on implementation.

**Do I need a team beforehand?**  
No. There is a team formation session at kickoff. Bring a problem idea or an initial Use-Case Canvas and discuss it with potential teammates. Teams consist of **2–4 students**.

**Can our project be a tool, visualizer, or platform?**  
Yes. Demonstrate how it addresses a problem or supports users for a specific application. Explain your technical contribution and its practical purpose.

**What if I do not understand a notebook or presentation?**  
Start with the problem statement, figures, and limitations. Ask teammates to explain the terms and assumptions. Use the introductory resources in the notebook catalog.

**What if our problem has no clear quantum use case?**  
A well-supported analysis of why a method is unsuitable can be a project outcome. Show the reasoning, comparisons, and limitations rather than relying on an unsupported conclusion.

**I am not a student. Can I participate?**  
The team format described in this guide is **2–4 students**. Contact the FGCU organizing team through the event chat to discuss other forms of involvement.

**Does the closing presentation affect our score?**  
No. It is a sharing session. Attendance and participation in that session are required to receive a participation certificate.

---

## Appendix A: Quantum computing glossary

You'll hear these on day one. You don't need to be able to derive any of them.

| Term | What it means when someone says it at this event |
|---|---|
| **Qubit** | The quantum unit of information. Unlike a bit, it can be in a combination of 0 and 1 until measured. |
| **Superposition** | That "combination of states" property. It's not "both at once" in any useful everyday sense, it's a weighted combination that produces probabilities on measurement. |
| **Entanglement** | Two or more qubits whose outcomes are correlated in ways no classical system can reproduce. It's the resource that makes quantum computing different. |
| **Circuit** | A quantum program. A sequence of operations (gates) on qubits. |
| **Gate** | One operation on one or more qubits. The building block. |
| **Shots** | How many times you run a circuit. Quantum results are probabilistic, so you run repeatedly and read the distribution. |
| **QPU** | Quantum Processing Unit: the actual quantum chip. |
| **Transpile** | Rewriting your circuit into the specific gates and connectivity a given QPU physically supports. |
| **Noise** | Real quantum hardware makes errors. Managing this is most of the engineering. |
| **Error mitigation** | Statistical techniques to recover a good answer from noisy runs. Different from error *correction*, which is a future, much bigger thing. |
| **QUBO** | Quadratic Unconstrained Binary Optimization: a standard way of writing an optimization problem that quantum optimizers can consume. If your problem can become a QUBO, it's in scope. |
| **Hamiltonian** | A mathematical description of a system's energy. Chemistry and physics problems are usually posed this way. |
| **VQE / QAOA** | The two most common hybrid quantum-classical algorithms. VQE for finding lowest-energy states; QAOA for optimization. |
| **Utility scale** | Circuits large enough that classical brute-force simulation gets hard — roughly 100+ qubits. Where the interesting current research lives. |

---

## Appendix B: Preparation and submission checklist

### Before kickoff on October 30, 2026, at 1:30 p.m.

**All participants**

- [ ] Register through <https://tinyurl.com/fgcu-quantum>; enter **QUANTUMEAGLE** if prompted.
- [ ] Join <https://discord.gg/vz6uTbtJzR>.
- [ ] Create an IBM Quantum Platform account (§4.1).
- [ ] Create a GitHub account and verify the email address (§6.1).
- [ ] Read §2 and §3 and bring a problem or application idea.
- [ ] Draft the Use-Case Canvas in Appendix C.
- [ ] Explore [IBM Quantum Composer](https://quantum.cloud.ibm.com/composer).

**Team members doing quantum programming or hardware experiments**

- [ ] Choose browser-based tooling (§5.1) or set up a local environment (§5.2).
- [ ] If using a local environment, run `check_setup.py` (§5.3).
- [ ] If using hardware through code, store the API key and CRN securely (§4.3).
- [ ] Test hardware access if needed (§5.4), allowing time for queues.
- [ ] Review the [hello world guide](https://quantum.cloud.ibm.com/docs/en/guides/hello-world).

**Team members focusing on problem framing, evaluation, or communication**

- [ ] Identify the intended users, constraints, and success measures.
- [ ] Draft a use-case description and explain the problem in 60 seconds.
- [ ] Select relevant resources from §7.
- [ ] Coordinate with teammates on implementation, analysis, and the demonstration.

### Before November 6, 2026, at 8:00 a.m. Eastern Time

- [ ] Complete the GitHub project repository and its README.
- [ ] Include relevant code, notebooks, setup instructions, analysis, results, and limitations.
- [ ] Record a project video **no longer than 15 minutes**, including any demo.
- [ ] **Upload the video to Deepstation.ai.**
- [ ] **Submit the GitHub project repository link through Deepstation.ai.**
- [ ] Verify that judges can access the video and repository.
- [ ] Complete the submission process before the deadline.

### For the November 6 closing ceremony

- [ ] Prepare a **10-minute team presentation**, including a demo.
- [ ] Attend and participate in the 1:30–3:00 p.m. team presentation session to qualify for a participation certificate.
- [ ] Remember that this sharing presentation does not affect final scores.

---

## Appendix C: Use-Case Canvas

Draft a one-page canvas before kickoff if possible. Bring it to team formation, then refine it with your teammates during the hackathon.

Copy this block into `USE-CASE.md` in your team GitHub repository, or incorporate it into the README. No shared event repository submission folder is required.

```markdown
# Use-Case Canvas

## 1. The problem
Write one paragraph for a reader unfamiliar with your field.
Use plain language and define any necessary technical terms.

## 2. Who has this problem
Be specific. Not "banks": "mid-size asset managers rebalancing
multi-asset portfolios monthly under UCITS constraints."

## 3. How it's solved today
What tool, what algorithm, how long does it take, how good is the answer?
This is your baseline. Without it you have no story.
If you don't know, that's your first research task.

## 4. What "better" is worth
Put a number on it. Currency, hours, lives, tonnes of CO2, error rate,
any unit, but a number. "It would be nice" is not an answer.

## 5. The quantum shape
Which of the three shapes is it? (Optimization / Simulation / Learning)
Why? What's the combinatorial explosion, the quantum system, or the
hidden structure?

## 6. The honest problem-size gap
How big is a real instance? How big can we run during the hackathon?
State both numbers. Explain the gap between the demonstration and a realistic application.

## 7. What would have to be true
For this to become useful beyond the demonstration, what would need
to change in hardware, algorithms, data, operations, or regulation?

## 8. What we will build or analyze during the hackathon
A tiny, concrete, achievable thing. Not the vision. The demo.
"We map a small routing instance to a QUBO, run a simulation,
compare with a classical solver, and test on hardware if feasible."

## 9. Why anyone should care
Three sentences. This becomes your opening slide.
```

---

*Found an error or a broken link? Let the FGCU organizing team know through the event chat.*
