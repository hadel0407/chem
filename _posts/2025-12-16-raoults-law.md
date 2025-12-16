---
title: "Raoult's Law vs Henry's Law: Vapor Pressure and Gas Solubility Explained"
date: 2025-12-16
description: "A clear comparison of Raoult's Law and Henry's Law, covering ideal and real solutions with practical chemical engineering examples."
---

<!-- 引入 MathJax 渲染公式 -->
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

In **physical chemistry** and **chemical engineering**, understanding solution behavior is essential for vapor–liquid equilibrium (VLE) analysis, separation processes, and material loss estimation. Two fundamental laws are widely used:

- **Raoult's Law** – relates vapor pressure to liquid-phase composition  
- **Henry's Law** – relates gas solubility to gas-phase partial pressure  

Although they apply to different components, **both laws exhibit linear behavior in ideal solutions**. This article explains their definitions, similarities, deviations in real systems, and practical engineering applications.

---

## 1. Raoult's Law and Henry's Law

### 1.1 Raoult's Law

Raoult's Law describes the **partial vapor pressure of a component in an ideal liquid mixture**. It is accurate for **solvents and volatile components** when intermolecular interactions between unlike molecules are negligible.

**Mathematical expression:**

$$
P_i = x_i \cdot P_i^0
$$

Where:

- $P_i$ — partial vapor pressure of component $i$ in the vapor phase  
- $x_i$ — mole fraction of component $i$ in the liquid phase  
- $P_i^0$ — saturated vapor pressure of pure component $i$ at the same temperature  

**Example**

A liquid mixture contains 50 mol% ethanol.  
The saturated vapor pressure of pure ethanol at 25 °C is 0.08 atm.

$$
x_{\text{ethanol}} = 0.5
$$

$$
P_{\text{ethanol}}^0 = 0.08\ \text{atm}
$$

Applying Raoult’s Law:

$$
P_{\text{ethanol}} = x_{\text{ethanol}} \cdot P_{\text{ethanol}}^0 = 0.5 \times 0.08 = 0.04\ \text{atm}
$$

---

### 1.2 Henry's Law

Henry's Law describes the **solubility of a gas in a liquid at equilibrium**. It is applicable to **dilute gas components** dissolved in liquids.

**Mathematical expression:**

$$
C = k_H \cdot P
$$

Where:

- $C$ — concentration of dissolved gas in the liquid  
- $P$ — partial pressure of the gas in the vapor phase  
- $k_H$ — Henry’s constant (depends on solvent and temperature)  

**Typical applications include:**

- Gas absorption and stripping operations  
- Carbonated beverage production  
- Environmental engineering (air–water equilibrium systems)  

---

## 2. Relationship in Ideal Solutions

In **ideal solutions**, solute–solvent interactions are negligible, and both laws exhibit **linear proportionality**.

### Linear behavior

- **Raoult's Law (liquid → vapor):**

$$
P_i = x_i \cdot P_i^0
$$

- **Henry's Law (gas → liquid):**

$$
C = k_H \cdot P
$$

Henry's Law can be rearranged to express partial pressure:

$$
P = \frac{C}{k_H}
$$

At **gas saturation**, when the dissolved concentration reaches $C_{\text{sat}}$, the corresponding partial pressure equals the saturated vapor pressure $P_{\text{sat}}$:

$$
P_{\text{sat}} = \frac{C_{\text{sat}}}{k_H} \quad \Rightarrow \quad \frac{1}{k_H} \approx P_{\text{sat}}
$$

### Conceptual comparison

| Law | Primary focus | Mathematical form |
|----|----|----|
| Raoult's Law | Vapor pressure | $P_i = x_i P_i^0$ |
| Henry's Law | Gas solubility | $C = k_H P$ |

- **Raoult's Law** focuses on vapor pressure changes caused by liquid composition  
- **Henry's Law** focuses on dissolved gas concentration governed by gas pressure  

In ideal systems, both laws describe the **same linear thermodynamic behavior from different perspectives**.

---

## 3. Deviations in Real Solutions

Real solutions deviate from ideality due to **intermolecular forces**, such as hydrogen bonding, polarity differences, and van der Waals forces.

### 3.1 Raoult's Law deviations

- Vapor pressure no longer varies linearly with mole fraction  
- **Positive deviation**: weaker intermolecular interactions → higher vapor pressure  
- **Negative deviation**: stronger interactions → lower vapor pressure  

### 3.2 Henry's Law deviations

- Gas solubility deviates from linearity at elevated pressures  
- Strongly influenced by solvent composition and temperature  

### Practical validity in real systems

- **Raoult's Law** remains valid for the **solvent** in dilute solutions  
- **Henry's Law** remains valid for **trace gas solutes**

**Example: Nitrogen dissolved in liquid propylene**

- Liquid phase: predominantly propylene with trace nitrogen  
- Propylene vapor pressure:

$$
P_{\text{propylene}} \approx X_{\text{propylene}} \cdot P_{\text{propylene}}^0
$$

- Nitrogen solubility:

$$
C_{\text{N}_2} \approx k_H \cdot P_{\text{N}_2}
$$

These approximations are widely used for engineering calculations.

---

## 4. Applications in Chemical Engineering

In industrial storage and transfer systems, **non-condensable gas (NCG) purging** is commonly required. During purging, volatile liquids may evaporate into the gas phase, resulting in material losses.

### Step 1: Vapor pressure of liquid component

$$
P_{\text{material}} = X_{\text{material}} \cdot P_{\text{material}}^0
$$

### Step 2: Gas-phase volume fraction

$$
y_{\text{material}} = \frac{P_{\text{material}}}{P_{\text{total}}}
$$

### Loss reduction strategies

- Increasing system pressure reduces vapor-phase concentration  
- Lowering temperature reduces saturated vapor pressure  

### Example: Propylene tank purged with nitrogen

Operating conditions: 20 °C, total pressure = 15 atm

| Parameter | Value |
|----|----|
| Mole fraction $X_{\text{C}_3\text{H}_6}$ | 1 |
| Saturated vapor pressure $P_{\text{C}_3\text{H}_6}^0$ | 10 atm |
| System pressure $P_{\text{total}}$ | 15 atm |

Vapor-phase mole fraction:

$$
y_{\text{C}_3\text{H}_6} = \frac{10}{15} \approx 0.667
$$

Lowering the temperature to 0 °C:

$$
P_{\text{C}_3\text{H}_6}^0 \approx 5.7\ \text{atm} \quad \Rightarrow \quad y_{\text{C}_3\text{H}_6} \approx 0.38
$$

Increasing total pressure while keeping temperature at 20 °C:

$$
y_{\text{C}_3\text{H}_6} = \frac{10}{30} \approx 0.333
$$

✅ **Result:** Both lowering temperature and increasing total pressure reduce propylene loss. Combined, the effect is even more significant.

---

## 5. Summary

1. Raoult's Law and Henry's Law show similar linear behavior in **ideal solutions**.  
2. In real systems, deviations occur, but Raoult's Law remains applicable to solvents and Henry's Law to trace gases.  
3. These principles are powerful tools for **pressure control, temperature optimization, and material loss reduction** in chemical engineering practice.
