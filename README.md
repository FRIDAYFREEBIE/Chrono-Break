# ChronoBreak

### 🎮 Team-Based Turn RPG Project

---

## 📌 Project Overview
- **Game Genre**: 3D Turn-Based RPG
- **Development Period**: 2025 ~ (In Development)
- **Team Size**: 22 Members
  - Programming 4
  - Game Design 4
  - Art 14
- **Role**: Gameplay Programmer(Client)
- **Main Responsibilities**
  - Combat System
  - Gameplay Ability System(GAS)
  - SkillBase Architecture
  - GameplayTag-based Status Effect System
  - Data-driven Skill Pipeline

---

# 🔑 Key Technologies

## Unreal Engine 5
- Gameplay Ability System(GAS)-based combat framework
- GameplayTag / GameplayEffect based status effect system
- Asynchronous skill flow using Montage

## C++
- Reusable object-oriented architecture
- Refactored Blueprint-heavy logic into C++
- Unified SkillContext-based data flow

## System Architecture
- Designed SkillBase-based common skill execution structure
- Implemented SkillTagContainer-based status effect management
- UML-based class and gameplay flow design
- Built data-driven skill creation pipeline

---

# 🧩 System Architecture

## 🔹 Combat System Architecture

<p align="center">
  <img src="./Image/UML_1.png" width="700">
</p>

Designed the combat system using Unreal Engine’s Gameplay Ability System(GAS).
TurnManager controls turn flow,
while GameplayAbilities handle skill execution.

AbilitySystemComponent and AttributeSet manage
damage calculations and gameplay states.

---

## 🔹 SkillBase Skill Architecture

<p align="center">
  <img src="./Image/UML_2.png" width="700">
</p>

Integrated all runtime skill execution data into `FCBSkillContext`
and designed `UCBGA_SkillBase` to handle common skill execution flow.

Blueprint handles montage, camera, and combo flow control,
while core functionality is implemented in C++.

### Skill Execution Flow
SkillDataAsset  
→ GameplayEvent  
→ SkillContextBuilder  
→ FCBSkillContext  
→ UCBGA_SkillBase  
→ ApplyTagToTarget  

---

## 🔹 GameplayTag-Based Status Effect System

<p align="center">
  <img src="./Image/UML_3.png" width="700">
</p>

<p align="center">
  <img src="./Image/UML_4.png" width="700">
</p>

Designed a data-driven status effect system using GameplayTags and GameplayEffects.

`SkillTagContainer` manages active effects,
while each effect inherits from `UCBTagEffectBase`.

### Status Effect Flow
OnApplied()
→ OnTurnTick()
→ OnRemoved()

---

# 🤔 What I Learned

- Gained experience designing scalable combat systems using Gameplay Ability System(GAS).
- Learned the importance of object-oriented architecture by separating responsibilities between SkillBase, SkillContext, and TagEffect systems.
- Designed a GameplayTag-based status effect framework and understood the strengths of data-driven architecture.
- Improved maintainability and collaboration efficiency by refactoring Blueprint-heavy systems into C++.
- Used UML diagrams to visualize and share gameplay architecture with teammates.
- Gained collaborative workflow experience using Git Fork, including branch strategies and Unreal Asset conflict resolution.

# 🎥 Skill Test Videos (YouTube)

## ⚔️ Zero Hour
<p align="center">
  <a href="https://www.youtube.com/watch?v=WNjzdvI6RSM">
    <img src="https://img.youtube.com/vi/WNjzdvI6RSM/maxresdefault.jpg" width="500">
  </a>
</p>

---

## ⏳ Time Echo
<p align="center">
  <a href="https://www.youtube.com/watch?v=KdlDH5MvxLg">
    <img src="https://img.youtube.com/vi/KdlDH5MvxLg/maxresdefault.jpg" width="500">
  </a>
</p>

---

## ⚡ Entropy Sink
<p align="center">
  <a href="https://www.youtube.com/watch?v=biSZbOrcxq8">
    <img src="https://img.youtube.com/vi/biSZbOrcxq8/maxresdefault.jpg" width="500">
  </a>
</p>

---

## 🕒 Chrono Shift
<p align="center">
  <a href="https://www.youtube.com/watch?v=blbhYtTdGug">
    <img src="https://img.youtube.com/vi/blbhYtTdGug/maxresdefault.jpg" width="500">
  </a>
</p>

---
