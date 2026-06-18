# FSM-Based Coffee Maker Using FPGA

## 📌 Title

FSM-Based Coffee Maker Using FPGA

A Finite State Machine (FSM) based Coffee Vending Machine implemented using Verilog HDL on an FPGA platform. The system automates beverage selection, payment verification, recipe retrieval, and ingredient dispensing for Coffee, Latte, and Espresso using digital logic and timed hardware control.

---

## 🛠 Technologies

### Hardware
- Altera DE2-115 FPGA Board
- FPGA Switches and LEDs
- Onboard Clock System

### Software
- Verilog HDL
- ModelSim
- Quartus Prime

### Concepts
- Finite State Machines (FSM)
- FPGA Design
- Digital System Design
- RTL Design
- Hardware Simulation
- Sequential Logic
- Memory-Based Recipe Storage

---

## ✨ Features

- Supports three beverages:
  - Coffee
  - Latte
  - Espresso
- FSM-based control architecture
- Payment verification before dispensing
- Invalid payment detection
- Memory-based recipe storage
- Automated ingredient dispensing
- Real-time FPGA implementation
- Modular Verilog design
- ModelSim simulation and verification
- Hardware validation using FPGA

---

## ⌨️ Keyboard Shortcuts

### FPGA Inputs

| Input | Function |
|---------|---------|
| Start | Initiates beverage preparation |
| Reset | Resets the entire system |
| Select = 00 | Coffee |
| Select = 01 | Latte |
| Select = 10 | Espresso |
| Payment = 00 | Coffee Payment |
| Payment = 01 | Latte Payment |
| Payment = 10 | Espresso Payment |

### FPGA Outputs

| Output | Function |
|---------|---------|
| milk_on | Activates milk dispensing |
| coffee_on | Activates coffee dispensing |
| froth_on | Activates froth dispensing |
| busy | Indicates machine is processing |
| done | Indicates beverage is ready |
| invalid_pay | Indicates payment mismatch |

---

## ⚙️ The Process

### 1. Drink Selection

The user selects one of the available beverages:

- Coffee
- Latte
- Espresso

The selected drink information is passed to the FSM controller.

### 2. Payment Verification

The FSM compares the selected drink with the entered payment value.

- Matching payment → Proceed
- Incorrect payment → Invalid Payment State

### 3. Recipe Retrieval

After successful verification, the system retrieves the corresponding ingredient ratios from memory.

### 4. Ingredient Dispensing

The FSM activates dispensing outputs sequentially:

1. Milk
2. Coffee
3. Froth

Each ingredient is dispensed for a predefined number of clock cycles.

### 5. Completion

After dispensing all ingredients, the FSM enters the FINISH state and asserts the `done` signal.

---

## 📚 What I Learned

- Designing Finite State Machines using Verilog HDL
- FPGA-based hardware implementation
- RTL-level digital design
- State transition modelling
- ModelSim simulation and debugging
- Memory interfacing in hardware systems
- Sequential circuit design
- Clock-based timing control
- Hardware verification and validation
- FPGA pin assignment and deployment

---

## 📈 Overall Growth

This project significantly improved my understanding of digital system design and FPGA development. I gained practical experience in converting a real-world automation problem into a hardware solution using FSM architecture. Working with Verilog HDL, ModelSim, and FPGA hardware strengthened my skills in hardware description languages, simulation, debugging, and digital design methodologies.

The project also enhanced my ability to develop modular and scalable hardware systems suitable for real-world embedded applications.

---

## 🚀 How Can It Be Improved

- Add touchscreen user interface
- Integrate IoT connectivity for remote monitoring
- Mobile app-based drink selection
- Cloud-based usage analytics
- Machine learning for personalized beverage recommendations
- Advanced ingredient sensing
- Energy optimization techniques
- Additional beverage options
- Inventory monitoring system
- Smart maintenance alerts

---

## ▶️ Running the Project

### Requirements

- Quartus Prime
- ModelSim
- Altera DE2-115 FPGA Board

### Steps

1. Open the project in Quartus Prime.
2. Compile the Verilog HDL files.
3. Verify functionality using ModelSim simulation.
4. Assign FPGA pins according to the pin assignment table.
5. Program the FPGA board.
6. Select a beverage using FPGA switches.
7. Enter the corresponding payment.
8. Press Start.
9. Observe dispensing outputs through LEDs.
10. Verify successful completion through the `done` signal.

---

## ☕ Beverage Recipes

### Coffee

| Ingredient | Dispensing Time |
|------------|----------------|
| Milk | 30 Clock Cycles |
| Coffee | 60 Clock Cycles |
| Froth | 10 Clock Cycles |

### Latte

| Ingredient | Dispensing Time |
|------------|----------------|
| Milk | 60 Clock Cycles |
| Coffee | 30 Clock Cycles |
| Froth | 10 Clock Cycles |

### Espresso

| Ingredient | Dispensing Time |
|------------|----------------|
| Milk | 5 Clock Cycles |
| Coffee | 90 Clock Cycles |
| Froth | 5 Clock Cycles |

---

## 🔬 FSM States

- IDLE
- WAIT_PAY
- CALC
- DISP_MILK
- DISP_COFFEE
- DISP_FROTH
- FINISH
- INVALID PAYMENT

---

## 🎯 Applications

- Smart Coffee Vending Machines
- Beverage Automation Systems
- FPGA-Based Control Systems
- Industrial Process Automation
- Smart Kitchen Appliances
- Digital Embedded Systems
- Educational FPGA Projects

---

## 👨‍💻 Author

- Santos Benser J

---

*"Brewing intelligence through digital logic and FPGA-based automation."*
