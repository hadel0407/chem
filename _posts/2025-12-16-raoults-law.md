---
title: "Raoult's Law vs Henry's Law: Vapor Pressure and Gas Solubility Explained"
date: 2025-12-16
description: "A clear and engineering-oriented comparison of Raoult's Law and Henry's Law, including vapor pressure, gas solubility, and loss reduction by pressure control."
---

# Raoult's Law vs Henry's Law: Vapor Pressure and Gas Solubility Explained

In physical chemistry and chemical engineering, vapor–liquid equilibrium (VLE) is essential for separation design, storage safety, and material loss estimation. Two classical laws are widely used:

- Raoult's Law — vapor pressure of volatile liquid components  
- Henry's Law — solubility of dilute gases in liquids  

Although they apply to different components, both laws describe linear behavior under ideal conditions. This article explains their physical meaning, mathematical form, deviations in real systems, and practical engineering applications.

---

## 1. Raoult's Law

Raoult's Law applies to volatile components in an ideal liquid mixture. It relates the partial pressure of a component in the vapor phase to its mole fraction in the liquid phase.

### Mathematical form

$$
P_i = x_i P_i^0
$$

Where:

- $P_i$ is the partial pressure of component $i$  
- $x_i$ is the mole fraction of component $i$ in the liquid phase  
- $P_i^0$ is the saturated vapor pressure of pure component $i$ at the same temperature  

### Example: Ethanol–water mixture

A liquid mixture contains 50 mol% ethanol.  
The saturated vapor pressure of pure ethanol at 25 °C is 0.08 atm.

$$
x_{\text{ethanol}} = 0.5
$$

$$
P_{\text{ethanol}}^0 = 0.08 \text{ atm}
$$

Applying Raoult's Law:

$$
P_{\text{ethanol}} = 0.5 \times 0.08 = 0.04 \text{ atm}
$$

This result shows that vapor pressure decreases linearly with liquid-phase mole fraction in ideal solutions.

---

## 2. Henry's Law

Henry's Law describes the equilibrium solubility of a gas dissolved in a liquid. It is valid for dilute gases at relatively low pressures.

### Mathematical form

$$
C = k_H P
$$

Where:

- $C$ is the concentration of dissolved gas in the liquid  
- $P$ is the partial pressure of the gas  
- $k_H$ is Henry’s constant, dependent on temperature and solvent  

### Typical applications

- Gas absorption and stripping columns  
- Carbonated beverages  
- Environmental air–water equilibrium modeling  

---

## 3. Conceptual Relationship Between the Two Laws

Both laws express linear equilibrium behavior, but from opposite directions.

### Raoult's Law

$$
\text{liquid composition} \rightarrow \text{vapor pressure}
$$

### Henry's Law

$$
\text{gas pressure} \rightarrow \text{dissolved concentration}
$$

In ideal systems, Henry’s Law can be rearranged:

$$
P = \frac{C}{k_H}
$$

At saturation:

$$
P_{\text{sat}} = \frac{C_{\text{sat}}}{k_H}
$$

This shows that Henry’s Law and Raoult’s Law describe the same thermodynamic equilibrium limit, but for different components.

---

## 4. Validity in Real Solutions

Real solutions deviate from ideality due to intermolecular forces.

### Raoult's Law

- Valid for solvents and major components  
- Deviations occur for strongly non-ideal mixtures  

### Henry's Law

- Valid for trace gas solutes  
- Deviations occur at high pressures or strong gas–liquid interactions  

### Engineering example: Nitrogen dissolved in liquid propylene

Liquid phase: mostly propylene  
Gas solute: nitrogen at low concentration

Propylene vapor pressure:

$$
P_{\text{propylene}} \approx x_{\text{propylene}} P_{\text{propylene}}^0
$$

Nitrogen solubility:

$$
C_{\text{N}_2} \approx k_H P_{\text{N}_2}
$$

This combination is commonly used in storage tank and absorption calculations.

---

## 5. Reducing Material Loss by Increasing Total Pressure

In many industrial systems, a volatile liquid is purged with an inert gas such as nitrogen. The material loss depends on the vapor-phase mole fraction of the volatile component.

### Step 1: Partial pressure of the volatile liquid

$$
P_v = x_v P_v^0
$$

For a pure liquid:

$$
x_v = 1
$$

### Step 2: Vapor-phase mole fraction

$$
y_v = \frac{P_v}{P_{\text{total}}}
$$

---

## 6. Example: Effect of Total Pressure on Purge Loss

### Case A: Low total pressure

Temperature: 20 °C  
Saturated vapor pressure of propylene:

$$
P_{\text{C}_3\text{H}_6}^0 = 10 \text{ atm}
$$

Total system pressure:

$$
P_{\text{total}} = 15 \text{ atm}
$$

Vapor-phase mole fraction:

$$
y_{\text{C}_3\text{H}_6} = \frac{10}{15} = 0.667
$$

### Case B: Increased total pressure

Increase total pressure to:

$$
P_{\text{total}} = 30 \text{ atm}
$$

Vapor-phase mole fraction becomes:

$$
y_{\text{C}_3\text{H}_6} = \frac{10}{30} = 0.333
$$

### Result

Doubling the total pressure reduces the vapor-phase concentration of propylene by 50 percent, directly lowering purge loss.

---

## 7. Engineering Insight

- Increasing total pressure reduces vapor losses  
- Lowering temperature reduces saturated vapor pressure  
- Combining pressure and temperature control is the most effective strategy  

These principles are widely applied in storage tanks, nitrogen blanketing systems, and flare loss minimization.

---

## 8. Summary

1. Raoult's Law governs vapor pressure of volatile liquids  
2. Henry's Law governs solubility of dilute gases  
3. Both laws are linear in ideal systems  
4. Increasing total pressure is an effective method to reduce volatile material loss  

Understanding and applying these laws correctly leads to safer and more economical chemical process design.
