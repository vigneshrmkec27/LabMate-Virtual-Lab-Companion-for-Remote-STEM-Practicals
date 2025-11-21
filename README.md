⭐ LabMate — Virtual Lab Companion for Remote STEM Practicals
Kaggle 5-Day Agents Intensive — Capstone Project (Track: Agents for Good)
🚀 Project Overview

LabMate transforms traditional STEM lab manuals into interactive, safe, virtual lab experiences.
Students upload a lab manual → Agents generate:

✔ Experiment steps

✔ Auto-generated simulation code

✔ Safety checks

✔ RC circuit simulation plot

✔ Auto-graded student report

✔ Memory-tracking of student performance

✔ A ChatAgent that answers questions from the manual

This solves the lack of physical lab access for many students.

🧠 Tech Used (Capstone Requirements Satisfied)
Requirement	Implemented?	How
Multi-Agent System	✔	Coordinator → Ingest → Experiment Generator → Safety → Simulator → Grader → Chat
Parallel / Sequential Agents	✔	Safety checks parallel logical grouping
Tools (Custom & Built-In)	✔	PDF loading tool, CodeGen tool, Simulation tool
Sessions & Memory	✔	MemoryBank storing student scores across labs
Context Engineering	✔	Manual chunking + structured ingestion
Observability	✔	Logging points in coordinator + agent stages
Evaluation	✔	Automated grading of simulation vs expected
Deployability Ready	✔	Modular structure, ready for Vertex AI Agent Engine
📦 Folder Structure
labmate/
├── README.md
├── writeup.md
├── demo.py
├── video_script.txt
├── evaluation_plan.md
├── submission_checklist.md
│
├── agents/
│   ├── coordinator.py
│   ├── ingest_agent.py
│   ├── experiment_generator_agent.py
│   ├── safety_agent.py
│   ├── simulator_agent.py
│   ├── grader_agent.py
│   └── chat_agent.py
│
├── tools/
│   ├── pdf_tool.py
│   ├── codegen_tool.py
│   └── simulator_tool.py
│
├── sample_data/
│   └── rc_lab_manual.txt
│
├── outputs/
│   ├── rc_charge.png  (generated at runtime)
│
└── docs/
    ├── architecture.png
    ├── storyboard.png

▶ How to Run Locally

Install Python 3.8+

Install dependencies:

pip install numpy matplotlib


Run:

python demo.py


Check:

outputs/rc_charge.png

console for safety checks + auto-grade


📊 Evaluation

Covered in evaluation_plan.md:

Simulation correctness

Grading rubric consistency

Student + TA usefulness scores

Observability metrics



Paste writeup.md content into Kaggle “project description” field.
Attach GitHub repo link + optional YouTube video.
