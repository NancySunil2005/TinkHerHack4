
AI-POWERED PEDESTRIAN TRAFFIC SYSTEM 🎯

## Basic Details

### Team Name: CODEALCHEMY

### Team Members
- Member 1: NANCY SUNIL - AMAL JYOTHI COLLEGE OF ENGINEERING AUTONOMOUS
- Member 2: NANDANA RAKESH KRISHNAN - AMAL JYOTHI COLLEGE OF ENGINEERING AUTONOMOUS


### Project Description
https://acrobat.adobe.com/id/urn:aaid:sc:AP:b2412f0d-cd8c-49c3-bcb4-936811709f26

### The Problem statement
Traditional traffic signals operate on fixed timers and do not adapt to real-time pedestrian and vehicle density. This leads to inefficient traffic flow and increased safety risks, especially in school zones where pedestrian safety is critical.


### The Solution
We developed an AI-powered adaptive traffic signal system that uses YOLOv8 object detection to analyze real-time pedestrian and vehicle density and dynamically adjust signal timing, with enhanced safety prioritization in school zones and inclusive override mechanisms.

---

## Technical Details
The system uses Python for developing the application and OpenCV for processing camera images and videos. 
Using computer vision and the YOLO (You Only Look Once) algorithm, the system detects pedestrians and vehicles in real time. This helps analyze traffic conditions and adjust signal timing automatically for better traffic flow.

### Technologies/Components Used

**For Software:**
- Languages used: PYTHON
- Libraries used:Ultralytics (YOLOv8) for AI-based object detection, OpenCV for image processing and signal visualization, and NumPy for numerical operations.
- Tools used: VS Code for development, Git & GitHub for version control and project management, and Command Prompt for running the application.



## Features

List the key features of your project:
- Feature 1: AI-Based Object Detection – Uses YOLOv8 to detect pedestrians and vehicles from traffic images in real time.
- Feature 2: Density-Based Adaptive Signal Control – Compares pedestrian and vehicle counts to dynamically switch between WALK and VEHICLE GO signals
- Feature 3: School Zone Priority Mode – Applies higher pedestrian weighting and extends crossing duration to 15 seconds for improved safety.
- Feature 4: Inclusive Override Mechanism – Activates WALK signal with extended crossing time when a vulnerable pedestrian is detected.

---

## Implementation 

### For Software:

#### Installation
```bash
# Clone the repository
git clone https://github.com/nancysunil/Tink-Her-Hack-4.0.git
cd Tink-Her-Hack-4.0

# Install required dependencies
pip install -r requirements.txt
```

#### Run
```bash
[Run commands - e.g., npm start, python app.py]
```

### For Hardware:

#### Components Required
[List all components needed with specifications]

#### Circuit Setup
[Explain how to set up the circuit]

---

## Project Documentation

### For Software:

#### Screenshots (Add at least 3)
<img width="1198" height="652" alt="image" src="https://github.com/user-attachments/assets/cf754fd1-c782-4e05-95f5-85780095a5e4" />
The image shows a typical urban intersection with vehicles approaching from different directions and pedestrians crossing at marked crosswalks. It represents a real-world traffic scenario where both vehicle flow and pedestrian movement need to be managed safely and efficiently

<img width="1196" height="650" alt="image" src="https://github.com/user-attachments/assets/9c222afb-c1a1-466b-98af-bde6d7f6610b" />
The image demonstrates real-time object detection using YOLOv8, where pedestrians and vehicles are identified and visually marked with bounding boxes.

<img width="1192" height="658" alt="image" src="https://github.com/user-attachments/assets/6dc3b408-dcf9-416c-b6d3-892526c45c9a" />
The final output shows real-time detection of pedestrians and vehicles, along with calculated counts and an adaptive signal decision, including extended crossing time for enhanced pedestrian safety.
#### Diagrams

**System Architecture:**

[Architecture Diagram:<img width="927" height="481" alt="image" src="https://github.com/user-attachments/assets/84c68ab1-bb11-4f6c-8e17-0b05b8625521" />

System Architecture:

The AI Smart Traffic Signal System is structured into multiple logical layers that process traffic input, apply AI-based detection, and generate adaptive signal decisions.
Layered Architecture Description
1️⃣ Input Layer

Traffic image (simulated CCTV input)

Configurable zone type (SCHOOL / NORMAL)

2️⃣ AI Processing Layer

YOLOv8 detects pedestrians and vehicles

Bounding boxes generated for detected objects

Object classification applied

3️⃣ Logic Layer

Count pedestrians and vehicles

Apply school zone weighting (×2 pedestrian score)

Check for vulnerable override condition

Assign dynamic crossing duration (15 seconds for school)

4️⃣ Decision Layer

Compare pedestrian score with vehicle count

If vulnerable detected → override logic

Generate final signal state:

WALK

VEHICLE GO

5️⃣ Output Layer

Display signal status

Display pedestrian & vehicle counts

Display zone type

Display crossing duration

Show “Inclusive Mode Active” if applicable


**Application Workflow:**

![Workflow] <img width="1347" height="1600" alt="image" src="https://github.com/user-attachments/assets/dba70730-d674-4391-9a71-21cfb06d6156" />
*Add caption explaining your workflow*

The system captures a traffic image and uses YOLOv8 to detect pedestrians and vehicles. It calculates real-time density, applies school zone priority logic, checks for vulnerable pedestrian override, and then dynamically updates the traffic signal with an appropriate crossing duration.

### For Hardware:

#### Schematic & Circuit

![Circuit](Add your circuit diagram here)
*Add caption explaining connections*

![Schematic](Add your schematic diagram here)
*Add caption explaining the schematic*

#### Build Photos

![Team](Add photo of your team here)

![Components](Add photo of your components here)
*List out all components shown*

![Build](Add photos of build process here)
*Explain the build steps*

![Final](Add photo of final product here)
*Explain the final build*

---

## Additional Documentation

### For Web Projects with Backend:

#### API Documentation

**Base URL:** `https://api.yourproject.com`

##### Endpoints

**GET /api/endpoint**
- **Description:** [What it does]
- **Parameters:**
  - `param1` (string): [Description]
  - `param2` (integer): [Description]
- **Response:**
```json
{
  "status": "success",
  "data": {}
}
```

**POST /api/endpoint**
- **Description:** [What it does]
- **Request Body:**
```json
{
  "field1": "value1",
  "field2": "value2"
}
```
- **Response:**
```json
{
  "status": "success",
  "message": "Operation completed"
}
```

[Add more endpoints as needed...]

---



## Project Demo

### Video
[Add your demo video link here - YouTube, Google Drive, etc.]

*Explain what the video demonstrates - key features, user flow, technical highlights*

### Additional Demos
[Add any extra demo materials/links - Live site, APK download, online demo, etc.]

---

## AI Tools Used (Optional - For Transparency Bonus)

If you used AI tools during development, document them here for transparency:

**Tool Used:**VS Code – For writing, editing, and debugging the Python code.

Git – For version control and tracking changes in the project.

GitHub – For repository hosting and project submission.

Command Prompt / Terminal – For running the Python application and installing dependencies.



**Key Prompts Used:**
- Generate adaptive traffic signal logic using YOLOv8 in Python.”
“Implement school zone priority with extended crossing time.”
“Add vulnerable pedestrian override mechanism in traffic control system.”

**Percentage of AI-generated code:** Approximately 30%

**Human Contributions:**
-Identified the real-world problem of fixed-timer traffic inefficiency and pedestrian safety risks.
Designed the overall system architecture and adaptive decision flow.
Developed the density-based signal comparison algorithm.
Implemented school zone prioritization with extended crossing duration (15s).
Designed and implemented the inclusive override mechanism for vulnerable pedestrians.
Structured the visual traffic dashboard layout and signal display logic.
Conducted testing, debugging, and performance validation.
Organized project documentation and presentation materials.

*Note: Proper documentation of AI usage demonstrates transparency and earns bonus points in evaluation!*

---

## Team Contributions
Nancy Sunil - Identified the real-world problem of fixed-timer traffic inefficiency and pedestrian safety risks.
Designed the overall system architecture and adaptive decision flow.
Developed the density-based signal comparison algorithm.
Implemented school zone prioritization with extended crossing duration (15s).
Designed and implemented the inclusive override mechanism for vulnerable pedestrians.
Structured the visual traffic dashboard layout and signal display logic.

Nandana Rakesh Krishnan -Organized project repository and GitHub structure.
Prepared README documentation and project formatting.
Created workflow and architecture diagrams.
Conducted testing, debugging, and performance validation.
Organized project documentation and presentation materials.

## License

This project is licensed under the [LICENSE_NAME] License - see the [LICENSE](LICENSE) file for details.

**Common License Options:**
- MIT License 

Made with ❤️ at TinkerHub
