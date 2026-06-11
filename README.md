# 🔄 Object Pooling Plugin (Unity)
### High-performance pooling tool for Unity

---

## 🧩 Overview

The **Object Pooling Plugin** is a clean, modular and extensible **runtime pooling system** designed to reduce allocations and boost performance in Unity.  
It features both a **ScriptableObject-based workflow** and a **generic key-driven pool manager**, making it suitable for gameplay systems, tools, UI and scalable frameworks.

> 🎯 Designed for readability, extensibility, and real production use, with clean architecture and minimal overhead.

---

## 🚀 Main Features

- **ScriptableObject-Based Pool Setup**: Define pools directly from the inspector.
- **Automatic Runtime Instantiation**: Preload objects at startup with zero runtime allocations.
- **IPoolable Interface**: Custom activation/deactivation logic for pooled objects.
- **Generic ObjectPoolManager<T>**: Key-based retrieval supporting any type.
- **Singleton Architecture**: Lightweight global access with self-validation.
- **Example Scene Included**: Complete demo with keyboard-controlled spawning.
  
---

## 🛠️ Components

### 🧱 ScriptablePool (ScriptableObject)
- Stores pool definitions: prefab, quantity, pool type  
- Ideal for fast editor setup and configuration

---

### 🎛️ ObjectPool (Manager)
- Instantiates and manages pools at runtime  
- Provides `GetPoolObject()` and `DeactivatePoolObject()`  
- Uses queues for O(1) operations  

---

### 🔧 ObjectPoolManager<T>
- Generic pooling system for any type  
- Dictionary-based lookup with optional auto-expansion  
- Perfect for large systems and tools  

---

### 🎬 IPoolable Interface
- `EnableObject()` and `DisableObject()` methods  
- Examples:  
  - **CubeScript** (manual toggle)  
  - **SphereScript** (timed despawn)  

---

### 🕹️ Picker (Demo Input)
- **S** → spawn cube  
- **D** → spawn sphere  
- Objects automatically return to pools after behavior completion  

---

## 🧑‍💻 Author
**Alessio Desidero’**  
Role : *Generalist Game Programmer*


---

*Thank you for checking out the project!* 🌙
