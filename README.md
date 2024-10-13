# Lyft System FORAGE Design Project

## Overview
This project simulates the creation and servicing of various car models using object-oriented principles. The project includes different car components like engines and batteries, allowing for modular and flexible design. The system also incorporates testing to ensure each car model is correctly constructed and serviced.

## Project Structure
The project is divided into several stages, each focusing on a different aspect of the car's design:

- **Stage 2**: Focuses on building car models with different combinations of engines and batteries. Key components include:
  - **Engines**: Capulet, Sternman, and Willoughby engines with varying service requirements.
  - **Batteries**: Spindler and Nubbin batteries, each with unique characteristics.
  
- **Stage 3** and **Stage 4** build upon this system, introducing additional features, refinements, and testing capabilities.

---

# Lyft System Design Project (Stage 4)

## Overview
This project simulates a modular car system with engines, batteries, and tires. The system is designed to handle various car models by assembling different components (engines, batteries, and tires) using object-oriented principles. This stage focuses on the integration of tire components and expands the testing coverage for all key parts of the system.

## Stage 4 Enhancements
### New Features:
- **Tires Integration**: Added two types of tires—**Carrigan Tires** and **Octoprime Tires**—which introduce new logic for determining when tires need servicing.
  - **Carrigan Tires**: Needs service based on wear levels.
  - **Octoprime Tires**: Needs service if a cumulative wear threshold is exceeded.

- **Expanded Testing**: Introduced unit tests for tires, engines, and batteries to ensure each component works correctly.

## Key Components
- **Car Models**: Each car is composed of an engine, battery, and tires, allowing flexibility in configuring different models.
  - Engines: **Capulet**, **Willoughby**, and **Sternman** engines.
  - Batteries: **Spindler** and **Nubbin** batteries.
  - Tires: **Carrigan** and **Octoprime** tires.

## Project Structure
```
.
├── car_factory.py            # Factory for creating car models
├── car.py                    # Car class that integrates engine, battery, and tires
├── engine                    # Contains different engine classes
│   ├── capulet_engine.py
│   ├── sternman_engine.py
│   ├── willoughby_engine.py
├── battery                   # Contains different battery classes
│   ├── spindler_battery.py
│   ├── nubbin_battery.py
├── tires                     # Contains tire-related classes
│   ├── carrigan_tires.py
│   ├── octoprime_tires.py
├── test                      # Unit tests for engines, batteries, and tires
│   ├── test_capulet_engine.py
│   ├── test_willoughby_engine.py
│   ├── test_spindler_battery.py
│   ├── test_nubbin_battery.py
│   ├── test_carrigan_tires.py
│   ├── test_octoprime_tires.py
├── serviceable.py             # Interface for serviceable components
├── README.md                 # Project overview (this file)
```

## How to Use
1. **Clone the repository**:
   ```bash
   git clone https://github.com/YOUR-USERNAME/lyft-stage-4-project.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd lyft-stage-4-project
   ```

3. **Run the unit tests** to ensure everything is working correctly:
   ```bash
   python -m unittest discover test
   ```

## Testing
The project includes comprehensive unit tests for:
- Engines (Capulet, Willoughby, Sternman)
- Batteries (Spindler, Nubbin)
- Tires (Carrigan, Octoprime)

These tests can be run to ensure the system's accuracy and functionality across all components.

## Future Enhancements
- Further optimize the tire servicing algorithms for more realistic wear-and-tear simulation.
- Extend the system to support more car models with additional customizable components.
- Add more comprehensive performance testing.
