# Gang of Four (GoF) Design Patterns

## 🏗️ 1. Creational Patterns (5)
**Purpose:** These are all about **how objects are born.** They handle the instantiation process.

> **Mnemonic:** **S**ome **F**actory **A**lways **B**uilds **P**rototypes.

* **S**ingleton: Only one instance exists (The Boss).
* **F**actory Method: Lets subclasses decide which class to instantiate.
* **A**bstract Factory: Creates families of related objects.
* **B**uilder: Constructs complex objects step-by-step.
* **P**rototype: Creates new objects by cloning an existing one.

## 🏛️ 2. Structural Patterns (7)
**Purpose:** These are about **how classes and objects are assembled** into larger structures, like blueprints for a building’s frame.

> **Mnemonic:** **ABCD FPP** (Think: "A Broad Comprehensive Design For Professional Project")

* **A**dapter: Makes incompatible interfaces work together (The Plug).
* **B**ridge: Decouples an abstraction from its implementation.
* **C**omposite: Treats individual objects and compositions uniformly (Tree structures).
* **D**ecorator: Adds responsibilities to objects dynamically (The Garnish).
* **F**acade: Provides a simplified interface to a complex system.
* **P**roxy: A placeholder to control access to another object.
* **F**lyweight: Shares small objects to save memory.

## 🧠 3. Behavioral Patterns (11)
**Purpose:** These focus on **communication and responsibility.** How do these objects talk to each other and get work done?

> **Mnemonic:** **2 MICS, 2 OSS, V T** (Imagine a stage with 2 mics and a sound system).

* **M**ediator: Centralizes communication between objects.
* **M**emento: Captures and restores an object's internal state (Undo).
* **I**terator: Sequentially accesses elements of a collection.
* **C**ommand: Encapsulates a request as an object.
* **S**tate: Object changes behavior when its internal state changes.
* **S**trategy: Swaps algorithms at runtime.
* **O**bserver: A way of notifying multiple objects of state changes (Pub/Sub).
* **V**isitor: Adds new operations to existing object structures without modifying them.
* **T**emplate Method: Defines the skeleton of an algorithm, letting subclasses fill in the blanks.
* **C**hain of Responsibility: Passes a request along a chain of handlers.
* **I**nterprete**r**: Given a language, defines a representation for its grammar.


---

## 📖 The "Smart Construction" Story
If mnemonics aren't your style, visualize this scenario:

1.  **Creational (The Birth):** You go to the **Abstract Factory** to get parts. The **Builder** assembles the complex crane step-by-step, but there is only **One (Singleton)** foreman on-site.
2.  **Structural (The Skeleton):** To connect your old tools to new power outlets, you use an **Adapter**. You use a **Facade** (the front wall) to hide all the messy wiring inside. To save space, you use **Flyweight** bricks—they all look the same and share resources.
3.  **Behavioral (The Action):** When the foreman shouts, all workers react (**Observer**). If a worker hits a problem they can’t solve, they pass it up the **Chain of Responsibility**. If the weather changes (**State**), the crew switches their **Strategy** from roofing to indoor tiling.

Does focusing on one specific category—like the structural patterns—help clarify things, or would you like to see a code example for a specific one?