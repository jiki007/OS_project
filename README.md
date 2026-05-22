# OS_project 🐧

A collection of 5 automation scenarios implemented in Google Colab 
running on an Ubuntu-based environment, built for the Operating Systems course.

---

## 📂 Repository Structure
├── Chatbot.ipynb              # Scenario 1 - Process Automation Chatbot with OS Commands
├── CronJobScheduler.ipynb     # Scenario 2 - Cron Job Scheduler Simulator
├── FileOrganization.ipynb     # Scenario 3 - Intelligent File Organization & Backup
├── PackageManager.ipynb       # Scenario 4 - Automated Package & Dependency Manager
├── SmartHome.ipynb            # Scenario 5 - Smart Home Sensor Automation System
└── README.md

---

## 🚀 Scenarios

### 1. 🤖 Process Automation Chatbot with OS Commands
An interactive chatbot that accepts natural language commands and executes
real Ubuntu shell commands, logging all interactions and visualizing usage patterns.

**Key Features:**
- Natural language command parsing
- Real Ubuntu commands (`df`, `ps aux`, `top`, `free -h`, `uptime`, `uname`, `ip`, `who`)
- 9 supported commands: disk space, processes, CPU, memory, uptime, OS info, network, users, kill process
- Command frequency bar chart and command timeline chart
- Interactive mode and demo mode

**Ubuntu Concepts:** Shell commands, process management, system monitoring, `subprocess`

---

### 2. ⏰ Cron Job Scheduler Simulator with Visual Logs
Simulates Ubuntu's cron job scheduling system by running 5 real Ubuntu
commands automatically at defined intervals and visualizing execution history.

**Key Features:**
- 5 scheduled jobs: Log Rotation, Disk Cleanup, Memory Check, Uptime Check, Backup
- Real Ubuntu commands (`df -h`, `free -h`, `uptime`, `echo`)
- Gantt chart showing job execution timeline
- Success vs failure bar chart
- Job execution frequency and average duration charts
- Full execution log table

**Ubuntu Concepts:** Cron jobs, process scheduling, task automation

---

### 3. 📁 Intelligent File Organization & Backup Automation
Simulates a messy Ubuntu file system and automates sorting, organizing,
backing up, and cleaning up files.

**Key Features:**
- Generates 30 random files with mixed extensions in a messy folder
- Auto-organizes files into categories (documents, images, videos, audio, code, archives)
- Before/after visualizations showing the difference
- Timestamped backup of organized folder
- Cleanup automation that removes original messy files
- Full organization log table

**Ubuntu Concepts:** File system management, backup automation, directory operations

---

### 4. 📦 Automated Package & Dependency Manager Simulator
Simulates Ubuntu's `apt` package manager by automating the installation,
removal, and updating of software packages with full dependency resolution.

**Key Features:**
- Repository of 15 real Ubuntu packages with realistic versions and sizes
- Recursive dependency resolution (like real `apt`)
- Install, remove, and update operations with conflict detection
- Dependency tree network graph visualization
- Storage usage charts (bar + pie)
- Full operation log table

**Ubuntu Concepts:** Package management, dependency resolution, `apt`

---

### 5. 🏠 Smart Home Sensor Automation System
Simulates a smart home IoT environment with 5 sensors that generate
real-time data and trigger automated responses when thresholds are exceeded.

**Key Features:**
- 5 sensors: Temperature, Humidity, Motion, CO2, Light
- Automation rules that trigger actions (fan, heater, blinds, lights, ventilation)
- Real-time sensor timeline charts with threshold lines and alert highlights
- Automation events dashboard
- Statistics summary (min, max, average per sensor)
- Full automation event log

**Ubuntu Concepts:** Process automation, real-time monitoring, event-driven systems

---

## 🛠️ How to Run

1. Open [Google Colab](https://colab.research.google.com/)
2. Upload the `.ipynb` file for the scenario you want to run
3. Run each cell **top to bottom** in order
4. Each notebook is fully self-contained

---

## 📦 Dependencies

All dependencies are installed automatically inside each notebook:

| Library | Used In |
|---------|---------|
| `matplotlib` | All scenarios (visualizations) |
| `networkx` | Scenario 4 (dependency tree graph) |
| `numpy` | Scenario 5 (sensor data) |
| `subprocess` | Scenarios 2 & 1 (Ubuntu commands) |
| `shutil` | Scenario 3 (file operations) |
