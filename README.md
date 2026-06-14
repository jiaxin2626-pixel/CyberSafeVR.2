
# CyberSafe VR 2

**CyberSafeVR.2** is a Virtual Reality Cybersecurity Training Platform developed by Hardhat Enterprises as part of the **Deakin University Capstone Project**.

It provides immersive VR training for:

- Smishing
- Password Security
- Safe Web Browsing
- Securing Shared Accounts
- CyberAttack Time Machine
- Insider Threats


---

## Project Structure

```
CyberSafeVR.2/
- Assets/
- Packages/
- ProjectSettings/
- UIElementsSchema/
- UserSettings/

### research

- tutorial design for the VR project based on user personas analysis
- tutorial design to help solve learning anxiety based on Persona-Gen tool
- Understanding Cyber Scams Through Human Friction: A Qualitative Alignment Matrix
- a survey regarding 24 Deakin students' well-being and stress levels in their life, which might lead to students’ vulnerabilities and make them targets for cyber-scams.
- a data analysis based on the survey to understand how students’ financial status, academic pressure and supporting system affect their cyber-safe condition.
- 12 students' contact details who are willing to take part in the Cyber-safe VR experience later next trimester.
 
```
### Folder and Asset Organization 
All assets must be placed in centralized folders under `Assets/`:
Assets/
- Animation/          Animations for characters or environment
- Art/                Artwork (may be added in future trimesters)
- Audio/
  - Music/            Background music
  - Sound FX/         Sound effects
- Code/
  - Scripts/          All C# scripts
  - Shaders/          Custom shaders
- Docs/               Documentation, concept art, marketing material
- Materials/          Materials for 3D models
- Models/             3D models
- Prefabs/            Reusable components and game objects
- Scenes/             Unity scene files (.unity)
- Textures/           Textures used in materials or models
- UI/                 User interface elements
- TextMeshPro/        TextMeshPro-related assets
- research/
---
**Asset Placement Rule:** Keep shared assets (e.g., CityPeople, OfficeProps) in the root `Assets/` folder.


### Scene Naming and Build Settings

- Place all scene files under `Assets/Scenes/`.  
- Use the format `[FullModuleName][ActivityNumber].unity`.  
  - Example: SafeWebBrowsing01.unity  
  - If multiple scenes for an activity: SafeWebBrowsing01_Office.unity, SafeWebBrowsing01_End.unity  
- Add your scene to **Build Profiles**:  
  - Open the scene in Unity → File → Build Profiles → Add Open Scenes  
  - Do **not** remove existing scenes from the build list.

### Asset Placement/Naming Conventions

- Each module should have its own folder; activity-specific files go in relevant subfolders.  
  - Example: `Assets/Code/Scripts/SafeWebBrowsing/Activity01/`  
  - Models: `Assets/Models/SafeWebBrowsing/Activity01/`  
  - UI: `Assets/UI/SafeWebBrowsing/Activity01/`  
- Avoid generic names like NewScript.cs or Scene1.unity. Use descriptive names such as LoginManager.cs or SafeWebBrowsing01_Start.unity.

### Script Class Naming / Namespaces

- Use clear and descriptive class names within unique namespaces to prevent conflicts.  
- Each module or activity should define its own namespace:  
  - Example: PasswordSecurity01 for the first activity of the Password Security module.

### Rules and Reminders

- Never push directly to main.  
- All code must go through pull requests.  
- Always merge activity branches into the module branch **before** merging the module branch to main.  
- Pull the latest changes from the base branch before starting or submitting work.

---

## Setup Instructions

### Requirements

- **Unity Version:** 6000.0.43f1 (LTS)

---

### Steps

1. **Clone the Repository**

```bash
git clone https://github.com/Hardhat-Enterprises/CyberSafeVR.2.git
```

2. **Open in Unity Hub**

- Use **Unity 6000.0.43f1 LTS**
- Open the `CyberSafeVR.2` folder

3. **Run the Project**

- Go to `Assets/Scenes/`
- Open `MainMenu.unity`
- Click **Play**

4. **Set Up VR**

- Enable **OpenXR** or **Oculus Plugin** in **Project Settings → XR Plug-in Management**
- Use **XR Device Simulator** if you don’t have a headset:

```bash
Window → XR → XR Interaction Debugger → Device Simulator
```

---

## 📄 License

This project is for **educational use only** as part of Deakin University's Capstone Program.
