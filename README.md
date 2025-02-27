# Vending-machine-portfolio-

Overview
This project is a simplified vending machine circuit built on a breadboard, demonstrating fundamental digital logic concepts such as SR latches and delayed resets. The design simulates how a vending machine processes coin input and dispenses an item.

Components Used
-Breadboard

-Slide switches (to represent coin inputs)

-Push-button switches (to simulate item selection)

-LEDs (to indicate machine state and item dispensing)

-Resistors

-Integrated Circuits (ICs) for logic gates (AND, OR, NOR, etc.)

Truth Table
Screenshot 2025-02-27 090014

When A = 0 and B = 0, the latch holds its previous state, meaning no new action is taken.

When A = 0 and B = 1, the latch is set, meaning the vending machine is ready to dispense an item.

When A = 1 and B = 0, the latch is reset, meaning the machine does not dispense.

When A = 1 and B = 1, the state is invalid and should be avoided.

Circuit Diagram
Screenshot 2025-02-27 090323 Screenshot 2025-02-27 090233

How it works
Coin Input
Screenshot 2025-02-27 120412

A user presses a switch, representing a valid coin input.

The logic gate network verifies the correct input combination.

If valid, the circuit sets the SR latch, meaning the vending machine is ready.

Item Selection
Screenshot 2025-02-27 120420

The user presses a push-button switch, signaling item selection.

The SR latch maintains a high output, turning on an LED that represents the vending action.

Delayed Reset Activation
