---
layout: about
title: About
permalink: /
subtitle: BSc in Computer Science, City University of Hong Kong (Graduated) <br> Incoming ECE MEng Student (Specialized in Software Engineering and Intelligent Systems), University of Alberta (Fall 2026)

profile:
  align: right
  image: shuai.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Taken during my trip to Sapporo, Japan.</p>

selected_papers: false 
social: true # Enabled for professors to easily view your GitHub/Email

announcements:
  enabled: false 
  scrollable: true 
  limit: 5 

latest_posts:
  enabled: false
---

## **About Me**

I am an incoming **ECE MEng (Master of Engineering)** student at the **University of Alberta** (Starting Fall 2026). I recently graduated with a **Bachelor of Science in Computer Science** from the **City University of Hong Kong (CityU)** in June 2026.

With a rigorous foundation in theoretical computer science, top-tier programming capabilities, and strong mathematical intuition, **my ultimate goal is to pursue a Ph.D.** I aspire to contribute to next-generation intelligent systems, focusing on **Robot Learning, Continual/Representation Learning**, and **Efficient AI Software Systems**. 

I am actively seeking **Research Assistant (RA) positions**, collaborative research projects, or software-driven AI development opportunities for the upcoming semesters at UAlberta & Amii.

---

## **Research Interests**

I am eager to bridge the gap between algorithmic theory and practical deployment in the following areas:
* **Robot Learning & Agile Locomotion:** Coupling deep reinforcement learning (DRL) with structural or biological priors (e.g., CPG) for complex robotic systems.
* **Representation & Continual Learning:** Investigating sample-efficient learning, state representation abstraction, and robust adaptation in dynamic, non-stationary environments.
* **AI Systems & Software Engineering:** Building highly optimized, full-stack software architectures, high-throughput pipelines, and efficient communication protocols for AI/Robotics deployment.

---

## **Featured Project**

### Hybrid Legged Locomotion: Integrating CPG with Deep Reinforcement Learning for an 18-DOF Hexapod
*Individual Contributor | Final Year Project at CityU CS (Grade: **A-**)*

<div class="row justify-content-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/hexapod_demo.gif' | relative_url }}" alt="Hexapod Locomotion Demo">
    </div>
</div>
<br>

To overcome the sample inefficiency and unstable local minima of training high-dimensional systems from scratch, this research engineered an end-to-end hybrid framework coupling **Hopf-oscillator-based Central Pattern Generators (CPG)** with a **Deep Reinforcement Learning (DRL)** agent (observing a 29-dimensional state space). 

#### **Key Achievements & Metrics**
* **[Convergence Optimization]:** Accelerated reward convergence significantly compared to model-free RL baselines by injecting structural biological priors.
* **[Energy Efficiency]:** Generated highly symmetrical, steady tripod gaits, lowering mechanical transport costs by **XX%**.
* **[Curriculum Learning]:** Formulated a multi-stage curriculum pipeline to progressively train the agent from flat surfaces to complex fields with physical obstacles.
* **[Sim-to-Real Bottleneck Solution]:** Successfully deployed the policy onto bare-metal hardware under a strict **9600-baud serial bottleneck**. Engineered a custom 40-byte bidirectional binary communication protocol, achieving **10 Hz real-time closed-loop control** via onboard IMU feedback.

*Key Tech: PyTorch, Reinforcement Learning, Robot Locomotion, C++, Arduino, Sim-to-Real.*
`[Code & Demo Video Link coming soon]`

---

## **Academic & Core Strengths**

Instead of just running AI models, I back my research with a solid mathematical and software engineering foundation:
* **Mathematical Rigor:** Achieved **A+** in *Enhanced Calculus & Linear Algebra*, and **A** in *Computational Probability Modeling*.
* **Algorithmic Mastery:** Active **Core Team Member in ICPC** (Nanjing & Shenyang Regionals), specializing in graph theory, dynamic programming, and complex network optimization.
* **Coding Excellence:** Secured **A+** in both *Introductory and Advanced Computer Programming* modules, alongside an **A** in *Software Engineering Practice*.

---
<!-- 
## Industrial Experience (AI & Full-Stack Systems)

### **Nanjing Liandi Information Systems | Software Development Engineer Intern**
*Shanghai, China | July 2025 - August 2025*
* Developed an **AI-based meeting record processing system** features audio transcription, automated summary generation, and knowledge base management.
* Architected microservices using the **Dify workflow engine, FastAPI, SQLAlchemy**, and **Next.js**, while integrating local APIs for **Whisper and PyAnnote** models.
* Engineered comprehensive test suites utilizing condition and path coverage metrics on Ubuntu systems via SSH.

### **Spark Technology Innovation Limited | Software Development Engineer Intern**
*Hong Kong, China | August 2024 - May 2025*
* Designed the database architecture and backend systems for an enterprise WeChat mini-program managing real-time warehouse logistics, permission structures, and data analysis.
* Conducted system-wide testing, drafted comprehensive user manuals, and handled post-launch debugging and updates.

--- -->

## **Technical Skills**

* **Programming:** Python, C++, JavaScript, Java, MATLAB, SQL, HTML/CSS
* **AI & Robotics:** PyTorch, TensorFlow, ROS/ROS2, OpenCV, OpenAI Gym
* **Software & Systems:** FastAPI, Next.js, PostgreSQL, Linux/Ubuntu (SSH), Git, Docker, Microservice Architecture
* **Embedded & Hardware:** Arduino, Embedded C/C++, Serial Communication Protocols

---

If you are a professor at UAlberta or Amii searching for a graduate student with a rock-solid CS engineering background, exceptional algorithmic skills, and a passion for turning learning theory into deployed reality, please feel free to reach out via email!


<!-- ---
layout: about
title: about
permalink: /
subtitle: Bachelor of Science in Computer Science, City University of Hong Kong <br> Incoming ECE MEng Student, University of Alberta

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Taken during my trip to Sapporo, Japan.</p>

selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

## About Me


I am an incoming **ECE MEng (Master of Engineering)** student at the **University of Alberta** (Starting Fall 2026). Prior to this, I graduated with a **Bachelor's degree in Computer Science** from the **City University of Hong Kong (CityU)**. 

With a solid foundational background in Computer Science and a strong passion for intelligent systems, **my ultimate goal is to pursue a Ph.D.** where I can contribute to next-generation robotic control, automation, or human-robot interaction. By bridging my CS coding expertise with ECE hardware-software integration, I am actively seeking research opportunities, specialized projects (**ECE 910**), or Research Assistant (RA) positions for the upcoming semesters.

I am an incoming **ECE MEng (Master of Engineering)** student at the **University of Alberta**, starting in Fall 2026. Prior to this, I completed my Bachelor's degree at **City University of Hong Kong (CityU)**. 

Driven by a strong passion for robotics and intelligent systems, **my ultimate goal is to pursue a Ph.D.** where I can contribute to next-generation robotic control, automation, or human-robot interaction. I am actively seeking research opportunities, specialized projects (**ECE 910**), or Research Assistant (RA) positions for the upcoming semesters.

---

## Technical Skills

* **Programming Languages:** Python, C++, MATLAB, SQL
* **Robotics & AI Frameworks:** ROS / ROS2, PyTorch, OpenCV, Gazebo
* **Hardware & Embedded:** Embedded C, FPGA, PCB Design (Altium Designer/KiCad)
* **Developer Tools:** Git, Docker (on x86_64/AMD64 platforms), Linux/Ubuntu

---

## Research & Project Experience

### [Project Name 1: e.g., Autonomous Mobile Robot Navigation]
*Development Lead | CityU Graduation Project / Competition* * Developed a ROS-based autonomous navigation pipeline for a differential drive robot using LiDAR and IMU fusion.
* Implemented and optimized SLAM algorithms (Gmapping/Cartographer) and path planning (A* and DWA), reducing navigation error by 15%.
* *Key Tech:* C++, ROS, Linux, LiDAR.

### [Project Name 2: e.g., Embedded Control System for Robotic Arm]
*Hardware & Firmware Engineer | Course Project / Internship*
* Designed a 4-layer PCB for a robotic arm joint controller and programmed STM32 microcontrollers using FreeRTOS.
* Implemented PID control loops for precise motor position and velocity control.
* *Key Tech:* Embedded C, STM32, Altium Designer, PID Control.

---

## Research Interests

I am eager to dive deeper into the following areas at UAlberta:
1.  **Robotic Perception and Manipulation:** Combining computer vision and deep learning for robust robot control.
2.  **Intelligent Control & Reinforcement Learning:** Applying RL to autonomous systems and mobile robots.
3.  **Bio-inspired or Medical Robotics:** Exploring human-machine interfaces and assistive robotic devices.

If you are a professor at UAlberta ECE looking for a highly motivated student with strong engineering and coding skills to help "build things" or collaborate on research via **ECE 910**, please feel free to drop me an email! -->