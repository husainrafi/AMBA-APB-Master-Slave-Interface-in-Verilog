

# AMBA APB Master–Slave Interface in Verilog

# Overview

This project implements an AMBA APB (Advanced Peripheral Bus) Master–Slave Interface using Verilog HDL. The design demonstrates low-power peripheral communication commonly used in embedded systems and System-on-Chip (SoC) architectures.

The project includes the design, implementation, and verification of APB Master and APB Slave modules, supporting both read and write transactions.

# Features

APB Master Module

APB Slave Module

Read and Write Operations

Finite State Machine (FSM) Based Design

Simulation and Verification using Verilog

APB Protocol Compliance

RTL Design and Testing


# APB Protocol States

1. IDLE State

No communication is active.

PSEL = 0

Bus waits for a new transfer request.


2. SETUP State

Transfer initiation phase.

PSEL = 1

PENABLE = 0

Address and control signals are generated.


3. ENABLE State

Data transfer phase.

PSEL = 1

PENABLE = 1

Read or write operation is completed.


# APB Architecture
<img width="1080" height="682" alt="image" src="https://github.com/user-attachments/assets/b880aae3-3b17-436b-9aa8-20cec348b39d" />


The system consists of:

*APB Master

Controls bus transactions.

Generates address, control, and data signals.


*APB Slave

Receives requests from the master.

Performs read/write operations.



# Key Signals

Signal	Description

PCLK	APB Clock
PRESETn	Active Low Reset
PSEL	Slave Select
PENABLE	Transfer Enable
PWRITE	Read/Write Control
PADDR	Address Bus
PWDATA	Write Data
PRDATA	Read Data


# Design Flow

1. RTL Design using Verilog HDL


2. Functional Verification


3. Testbench Development


4. Simulation


5. Waveform Analysis


6. Result Verification



# Simulation Results

<img width="1080" height="577" alt="image" src="https://github.com/user-attachments/assets/cb0b1a7e-8976-45a6-91a5-b16bbe653503" />

The APB Master and Slave were successfully verified through simulation.

Verified:

Write Transfer

Read Transfer

State Transitions

Control Signal Generation

Data Integrity

#  RTL-level synthesized schematic

<img width="1080" height="645" alt="image" src="https://github.com/user-attachments/assets/331193ed-e0df-4cbf-bd18-55333fe5b318" />

# Tools Used

Verilog HDL

EDA Playground

Digital Electronics Concepts

AMBA APB Protocol


# Learning Outcomes

VLSI Design Fundamentals

RTL Coding

FSM Design

APB Protocol Implementation

Functional Verification

Simulation and Debugging

SoC Communication Architecture


# Future Improvements

Multiple Slave Support

APB Bridge Integration

FPGA Implementation

UVM-Based Verification

Advanced Error Handling


 # Author

Shaikh Husain Rafi
Electronics and Communication Engineering
Bearys Institute of Technology, Mangalore

Connect with Me

LinkedIn: (linkedin.com/in/husain-rafi-a96a732b5 )

Email: (Shaikhhusainrafi1@gmail.com)





