# LMM-AI

## Language-to-Motion Model

LMM-AI is an AI-driven animation system that maps spoken or written language — including emotional tone and context — into full-body skeletal motion using real-time inverse kinematics.

This is not just a pose model. LMM understands intention, physical dynamics, tone, and expression. It’s designed for use in 3D pipelines (Blender, Unity, Unreal), real-time agents, and advanced game characters.

---

## 🚧 Status: Active Development

- 🔄 Transformer-based motion model in early training
- 🦴 Rig naming standard defined (`L_PointerF`, `R_Leg`, etc.)
- 🔁 Real-time motion engine (WIP)
- 🔉 Audio-to-context training pipeline started
- 💬 Prompt-to-motion tool (planned)

This project is structured to allow **modular contributions** by specialists in NLP, motion synthesis, animation tools, or Blender scripting.

---

## 🔍 Use Cases

| Use Case | Description |
|----------|-------------|
| 🎮 Game AI / NPCs | Real-time motion from TTS or in-game events |
| 🎥 Blender Animation | Prompt → Motion without keyframing |
| 🧍 Avatar UX | Human-like gestures for digital agents or VTubers |
| 🐾 Future: Animal motion | Motion for characters with tail, ears, etc. |

---

## 🧱 System Architecture

- **Multimodal Input:** Text + audio
- **Motion Modeling:** Transformer + gesture classification
- **Data Source:** Video clips (dialogue, physical interaction)
- **Pose Extraction:** OpenPose / MediaPipe (BVH or SMPL)
- **Output Layer:** Blender-compatible IK skeleton (JSON/FBX)

---

## 🔠 Bone Naming Format (Required)

| Format Type | Example |
|-------------|---------|
| Dual-Part   | `Amputed_Left_Leg` |
| Singular    | `Weak_Heart` |
| Multiple     | `Cold_Right_Finger2_Hand` |

Model must have full bone mapping using these conventions. AI will ignore bones not named correctly (e.g., missing `R_Leg` will simulate a limp or amputation).

---

## 🔐 License

Custom license by **Deprecated**.  
MIT license may be adopted if project is officially partnered with open research institutions (e.g., MIT, CMU, etc.).

> Redistribution and commercial deployment prohibited unless explicitly licensed. Contact for lab or R&D use.

---

## 🧑‍💻 Dev Stack

| Layer | Tools |
|-------|-------|
| Model | Python, PyTorch |
| Pose | OpenPose, FFMPEG |
| Output | Blender API (Python) |
| Dev | VSCode |
| Plugin (Planned) | Blender Addon in Python |
| Web UI (Planned) | React + Three.js |

---

## 🧪 Contribution Guidelines

I'm seeking:

- ML engineers (motion modeling / transformer tuning)
- Blender devs (rig validation / automation)
- Audio/NLP researchers (tone → motion)
- Dataset builders (gesture labeling, pose synthesis)

---

## 📍 Maintained by

**Deprecated**  
[github.com/DeprecatedForever](https://github.com/DeprecatedForever)

If you're interested to help this project please DM me on [discord](discordapp.com/users/1379677148327186483)
