# 🏙️ Victoria 3 Mod: Urban Housing & Real Estate Market

**Project Status:** Active / Playable
**Focus:** Economic Simulation, Scripting, Game Balance.

## 📖 About the Project
This mod introduces a comprehensive **Real Estate Market simulation** to Victoria 3, filling a gap in the base game's urban mechanics. It implements a dual-system economy for housing based on the player's political choices.

### Key Mechanics Implemented:
* **Housing Estates (Conjuntos Habitacionais):** A new building type constructed by the State (Player) to manage urban density.
* **Capitalist Real Estate Market:** Under capitalist laws, the mod simulates **real estate speculation**. Middle-class and Capitalist pops can invest in these buildings, generating wealth through buying/selling dynamics.
* **Socialist Housing Policy:** Includes a toggleable "Production Method" where ownership is fully state-controlled, redirecting 100% of the profits (rents) directly to the Government treasury.
* **Taxation System (IPTU):** Custom scripted modifiers that simulate a Property Tax, adding a new revenue stream and balancing the profitability of real estate assets.

---

## 🛠️ Technical Implementation (Under the Hood)

To achieve this simulation, I had to reverse-engineer and modify several core game files:

* **Production Methods (`.txt`/`.json`):** Created custom logic trees that switch asset ownership based on active laws (Capitalism vs. Socialism).
* **Modifiers & Math:** Balanced the math behind the "IPTU" tax rate to ensure it didn't crash the in-game economy, requiring analysis of income variables.
* **Building Logic:** Defined new asset classes that interact with the game's existing Pop (Population) investment pool.

---
*This project demonstrates my ability to understand complex economic systems and translate them into code logic via configuration files.*
