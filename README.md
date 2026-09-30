# 🔍 LiveDetective

**LiveDetective** is a real-time Android detection and tracking application built with **Kotlin** and **Jetpack Compose**. It uses **Google ML Kit** to detect objects through the camera, track their movement, identify them using image labeling, and present the results through a futuristic sci-fi interface.

The app turns the camera into a real-time **object detection scanner**, allowing users to detect, identify, classify, and save interesting targets into a personal **Codex**.

## ✨ Features

* 🎥 **Real-Time Camera Detection**

  * Detects objects directly from the camera feed.
  * Works continuously as objects move through the frame.

* 🎯 **Object Tracking**

  * Uses ML Kit Object Detection to locate objects.
  * Assigns tracking IDs so detection boxes can smoothly follow moving targets.

* 🧠 **Object Identification**

  * Uses ML Kit Image Labeling to identify detected objects.
  * Supports hundreds of common real-world labels such as animals, people, plants, laptops, and more.

* 🧬 **Smart Taxonomy**

  * Automatically categorizes detected targets as:

    * 🐾 Creature
    * 📦 Object

* ⭐ **Dynamic Rarity System**

  * Detection confidence is converted into a sci-fi rarity tier:

    * 🟣 **LEGENDARY** — 90%+
    * 🔵 **RARE** — 75–89%
    * 🟢 **UNCOMMON** — 50–74%
    * ⚪ **COMMON** — Below 50%

* 🕶️ **Sci-Fi AR Interface**

  * Futuristic glowing detection brackets.
  * Scanning-line animation.
  * Smooth object-following animations.
  * Jetpack Compose spring animations for natural movement.

* 📸 **Capture System**

  * Capture detected targets with their:

    * Name
    * Confidence score
    * Rarity
    * Timestamp

* 📖 **Codex**

  * Saved detections are stored locally.
  * Browse and manage previously captured targets.

## ⚙️ How It Works

LiveDetective uses a **two-stage machine-learning pipeline**.

### 1. Spatial Detection & Tracking

**ML Kit Object Detection** analyzes the camera frames and determines where objects are located.

Each detected object receives a tracking ID, allowing the application to maintain its identity while it moves around the camera frame.

### 2. Precision Identification

The detected region is then analyzed using **ML Kit Image Labeling**.

This provides labels such as:

`Cat` → `Dog` → `Person` → `Plant` → `Laptop`

along with a confidence score.

### 3. Taxonomy Mapping

The detected label is passed through the application's taxonomy system and classified into a broader category such as **CREATURE** or **OBJECT**.

### 4. Rarity Calculation

The confidence score is converted into the application's custom rarity system.

This gives every detection a more game-like identity and makes the scanning experience more engaging.

### 5. AR-Style Visualization

Jetpack Compose renders the detection overlay and animations on top of the camera preview.

Spring-based animations help the detection brackets smoothly follow moving targets instead of appearing rigid or jumpy.

### 6. Local Codex Storage

When the user captures a target, its information is saved locally using **Room Database**.

The saved record contains the target's name, confidence, rarity, and timestamp.

## 🛠️ Tech Stack

| Technology                  | Purpose                               |
| --------------------------- | ------------------------------------- |
| **Kotlin**                  | Primary programming language          |
| **Jetpack Compose**         | Modern Android UI                     |
| **ML Kit Object Detection** | Real-time object detection & tracking |
| **ML Kit Image Labeling**   | Object identification                 |
| **Room Database**           | Local detection storage               |
| **CameraX**                 | Camera integration                    |
| **Compose Animations**      | Smooth AR-style visual effects        |
| **Android SDK**             | Android application platform          |

## 🧠 Core Concepts Demonstrated

This project demonstrates practical experience with:

* Real-time camera processing
* Machine-learning integration on Android
* Object detection and tracking
* Image classification
* Confidence-score processing
* Custom taxonomy systems
* Local database persistence
* Jetpack Compose UI
* Animation and state management
* CameraX
* Modern Android development

## 🚀 Project Goal

The goal of LiveDetective is to experiment with combining **computer vision, mobile development, and interactive UI design** into a single Android application.

Instead of presenting ML detection as a simple list of labels, the project transforms it into an interactive **sci-fi scanning experience**.

## 🔮 Future Improvements

Possible future improvements include:

* Custom TensorFlow Lite models for specialized creatures
* More advanced object tracking
* Detection history and statistics
* More detailed Codex entries
* Additional creature and object categories
* Offline custom-model detection
* More advanced AR effects
* Exporting captured discoveries

## 👨‍💻 Built With

**Kotlin + Jetpack Compose + CameraX + Google ML Kit + Room**

Built as an Android development project to explore real-time computer vision and modern Android UI development.

---

⭐ **If you find the project interesting, feel free to explore the code and experiment with it.**
