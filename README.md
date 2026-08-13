# Investigative Object Manager (INOM)

A lightweight, client-side web application designed for link analysis, timeline visualization, and chain-of-custody tracking in Open Source Intelligence (OSINT) investigations. 

It allows investigators to visually map relationships between target entities, verify evidence integrity using cryptographic hashes, and switch seamlessly between an interactive node canvas and a chronological timeline view.

---

## 🌟 Key Features

* **Interactive Visual Board (Canvas):**
  * Drag-and-drop node placement on an infinite canvas.
  * Smooth pan and zoom controls (mouse wheel or navigation controls).
  * Automatic radial layout generator for auto-organizing nodes.
* **Investigative Objects (INOs):**
  * Classify entities using predefined icons (Person 👤, Address 🏠, Phone 📞, Vehicle 🚗, Document 📄, Server 🖥️, Domain 🌐).
  * Assign confidence levels: **Confirmed** (Green), **Probable** (Orange), **Unverified** (Pink), and **Disinformation** (Red).
* **Chain-of-Custody Integrity:**
  * Upload image evidence per node with automatic **SHA-256 hash generation** for verification.
* **Connection Management:**
  * Draw visual connection lines between related entities with custom text labels/notes.
  * Directly edit or delete connections via canvas interactions or the Connections Registry table.
* **Timeline View:**
  * Toggle between the canvas and a chronological timeline.
  * **Smart Stacking:** Automatically groups and vertically stacks multiple events or entities occurring on the same date.
* **Search & Filtering:**
  * Filter nodes in real time by plain text, entity type/icon, or confidence level.
* **Import / Export:**
  * Save and load investigation cases locally using JSON exports.
  * Export high-resolution PNG board reports for case documentation.

---

## 🚀 Getting Started

### Prerequisites
No server setup or installation is required! The application runs entirely inside any modern web browser.

### Running the Application
1. Download or clone the project repository.
2. Open `index.html` in your web browser (Chrome, Firefox, Edge, Safari).
3. Click **"+ New Investigation"** on the welcome screen to start a new case, or **"Import JSON"** to load an existing file.

---

## 🛠️ Usage Guide

### Board & Node Navigation
| Action | How-To |
| :--- | :--- |
| **Pan Canvas** | Click and drag on any empty space on the board. |
| **Zoom** | Use the mouse wheel or the `+` / `-` buttons in the top navigation bar. |
| **Add Entity (INO)** | Click the floating `+` button in the bottom-right corner. |
| **Move Entity** | Click and drag any node across the canvas. |
| **Edit / Delete Entity** | Right-click on any node to open the context menu. |

### Creating & Managing Connections
1. **Create Connection:** Right-click the source node, select **"Create Connection"**, and click on the target node.
2. **Edit / Delete Connection:** Click directly on any connection line (or its text label) on the board to edit the note or delete the connection. Alternatively, use the **Delete (X)** button in the Connections Registry sidebar table.

---

## 📂 Data & Privacy

* **Local Storage:** All progress is saved locally within your browser (`localStorage`). No data is sent to external servers.
* **Portable JSON Files:** Always export your investigation (`Export JSON`) to backup your work or share
