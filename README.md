# ⭐ LabMate — Virtual Lab Companion for Remote STEM Practicals  
### **Kaggle 5-Day Agents Intensive — Capstone Project**  
**Track:** Agents for Good (Education)

---

## 📌 Overview  
**LabMate** converts traditional engineering lab manuals into **interactive virtual lab experiences** using a fully modular **multi-agent system**.

Students upload a lab manual → Agents automatically generate:

- ✔ Structured experiment plan  
- ✔ Auto-generated simulation code  
- ✔ Safety analysis  
- ✔ A runnable RC simulation with plots  
- ✔ Auto-graded lab report  
- ✔ A memory-based student performance tracker  
- ✔ ChatAgent for Q&A with citations  

This opens lab access for students who lack physical lab facilities.

---

## 🧠 Core Features (Capstone Requirements Satisfied)

| Capstone Requirement | Implemented | Description |
|---------------------|-------------|-------------|
| **Multi-Agent System** | ✔ | Coordinator → IngestAgent → ExperimentGenerator → SafetyAgent → SimulatorAgent → GraderAgent → ChatAgent |
| **Tools (Custom)** | ✔ | PDF loader, CodeGen tool, Simulation tool |
| **Sessions & Memory** | ✔ | Student profile + score tracking |
| **Context Engineering** | ✔ | Manual chunking, structured parsing |
| **Observability** | ✔ | Logging & structured agent tracing |
| **Agent Evaluation** | ✔ | Grading against expected simulation metrics |
| **Deployment-Ready** | ✔ | Modular design suitable for Vertex AI Agent Engine |

---

## 🗂️ Project Structure

labmate/
├── README.md ← You are here
├── writeup.md ← Kaggle submission content
├── demo.py ← Full end-to-end demo runner
├── video_script.txt ← For 3-min demo video
├── evaluation_plan.md
├── submission_checklist.md
│
├── agents/
│ ├── coordinator.py
│ ├── ingest_agent.py
│ ├── experiment_generator_agent.py
│ ├── safety_agent.py
│ ├── simulator_agent.py
│ ├── grader_agent.py
│ └── chat_agent.py
│
├── tools/
│ ├── pdf_tool.py
│ ├── codegen_tool.py
│ └── simulator_tool.py
│
├── sample_data/
│ └── rc_lab_manual.txt ← Example manual for testing
│
├── outputs/ ← Generated plots + reports (auto-created)
│ └── rc_charge.png (created after running demo)
│
└── docs/
├── architecture.png
└── storyboard.png



---

## 🚀 Quick Start (Run Locally)

### **1. Install Requirements**
```bash
pip install numpy matplotlib

2. Run Demo
python demo.py

3. View Outputs

After running, check:

outputs/rc_charge.png → RC circuit simulation plot

Terminal output → safety results + grading + memory snapshot

🧪 What the Demo Produces

The demo simulates an RC circuit lab and generates:

A clean experiment specification

Auto-generated simulation code

Safety warnings (if any)

A capacitor charging plot (saved in outputs folder)

Auto-graded performance with feedback

Student learning memory updated

🎯 Why LabMate Matters

Brings STEM labs to students who cannot attend physical laboratories

Automates experiment explanation, simulation & grading

Helps teachers reduce grading time

Encourages equitable access to engineering education

🎓 Pedagogical Value

LabMate enables:

Remote learners to perform hands-on experiments

Self-paced practice with immediate feedback

Better exam preparation through auto-grading

Teacher analytics (future extension)
