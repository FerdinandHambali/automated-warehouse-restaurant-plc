# Automated Warehouse & Restaurant Automation Using PLC

**TRC4407 – Industrial Automation | Monash University**

## Project Overview

This project involves the design and implementation of an automated warehouse and restaurant logistics system using Programmable Logic Controllers (PLC) and Human-Machine Interface (HMI) visualisation in CODESYS.

The system integrates automated product identification, measurement verification, storage allocation, inventory management, conveyor transportation, and fault handling.

The warehouse automation system was further extended to support restaurant operations, including ingredient requests, inventory selection, kitchen order management, customer table routing, and dirty-dish handling.

The project was developed and demonstrated using PLC simulation and HMI controls.

## Technologies Used

- **PLC Programming:** Ladder Diagram (LD)
- **Development Software:** CODESYS
- **HMI:** CODESYS Visualization
- **Control Systems:** Sequential logic, timers, counters, interlocks
- **Automation:** Conveyor control, product sorting, inventory management
- **Simulation:** PLC and HMI-based process simulation

## System Features

### 1. Automated Warehouse System

**Product Identification**
- Barcode and SKU validation
- Product information verification
- Invalid identification and retry handling

**Weight and Dimension Verification**
- Measurement checking against expected product specifications
- Weight and dimensional tolerance validation
- Measurement retry and error detection

**Automated Storage Allocation**
- Product classification based on storage requirements
- Storage assignment based on temperature and fragility
- Storage capacity verification
- Inventory quantity tracking

**Environmental Monitoring**
- Refrigerated and frozen storage monitoring
- Temperature and humidity supervision
- Alarm and fault indication

### 2. Restaurant Automation System

**Ingredient Request and Stock Validation**
- Ingredient requests submitted through the HMI
- SKU and quantity validation
- Available stock verification
- Request acceptance or rejection

**FEFO Ingredient Selection**
- First-Expired, First-Out inventory selection
- Selection based on ingredient expiry dates
- Arrival-order priority for equal expiry dates

**Ingredient Retrieval**
- Retrieval confirmation and cancellation
- Automatic inventory deduction
- Protection against repeated retrieval

**Kitchen Order Management**
- Customer order entry and validation
- First-In, First-Out (FIFO) order processing
- Customer table assignment

**Kitchen-to-Customer Delivery**
- Automated routing to assigned customer tables
- Simulated arrival sensor confirmation
- Incorrect table detection

**Dirty Dish Return and Cleaning**
- Dirty-dish return requests
- Cleaning process sequence
- Timer-based cleaning control

### 3. Safety and Fault Management

The system incorporates control mechanisms to improve operational safety and process reliability.

Implemented functions include:

- Emergency stop and system reset
- Conveyor timeout monitoring
- Invalid barcode and measurement handling
- Insufficient stock and full storage detection
- Fault indication and HMI status feedback
- Sequential process interlocks

## HMI Visualisation

The HMI provides operators with interfaces for monitoring and controlling warehouse and restaurant processes.

**Warehouse Interfaces**
- Main system control
- Product identification
- Weight and dimension verification
- Storage assignment
- Inventory and environmental monitoring

**Restaurant Interfaces**
- Ingredient request and validation
- FEFO ingredient selection
- Ingredient retrieval
- Kitchen order management
- Customer table routing
- Dirty-dish return and cleaning

## Project Demonstration

The project demonstrates an integrated automation workflow, from warehouse product handling to restaurant ingredient retrieval and customer order delivery.

The demonstration includes simulated sensor activation, ingredient selection, inventory updates, conveyor operations, customer order routing, and cleaning control.

## Repository Contents

- `CODESYS_Project/` – Main PLC and HMI project
- `Screenshots/` – Warehouse and restaurant HMI images
- `Documentation/` – Supporting PLC logic diagrams and documentation

## How to Open the Project

1. Install a compatible version of CODESYS Development System.
2. Open the `.project` file from the `CODESYS_Project` folder.
3. Review the PLC program and HMI visualisation objects.
4. Enable CODESYS Simulation mode.
5. Build and run the application using the appropriate simulated device configuration.
6. Open the HMI visualisations to interact with the system.

**Note:** This project was developed for an academic automation simulation. Actual physical conveyors, sensors, and industrial equipment are not required for the documented simulation workflow.

## Skills Demonstrated

- PLC ladder logic programming
- Industrial automation system design
- HMI development and integration
- Sequential control and interlocking
- Inventory and warehouse management
- Conveyor and product routing logic
- Error detection and fault handling
- System simulation and testing

## Acknowledgements

Developed as part of TRC4407 – Industrial Automation at Monash University.

This was a group engineering project involving the development and integration of warehouse and restaurant automation functionalities.
