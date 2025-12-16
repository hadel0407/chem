---
title: "Raoult's Law vs Henry's Law: Understanding Vapor Pressure and Gas Solubility in Chemical Engineering"
date: 2025-12-16
description: "Learn the differences between Raoult's Law and Henry's Law, their behavior in ideal and real solutions, and practical applications in chemical engineering."
---

# Raoult's Law vs Henry's Law: Understanding Vapor Pressure and Gas Solubility in Chemical Engineering

In physical chemistry and chemical engineering, **Raoult's Law** and **Henry's Law** are fundamental principles used to describe the relationship between component concentration and partial pressure in solutions. While they apply to different types of substances and describe different properties, their behavior in ideal solutions is similar. This article explains their definitions, conditions of applicability, differences in real solutions, and practical applications in chemical process operations.

---

## 1. Introduction to Raoult's Law and Henry's Law

### Raoult's Law

Raoult's Law describes the vapor pressure of components in a liquid mixture:

\[
P_i = x_i \cdot P_i^0
\]

- **P_i**: Partial vapor pressure of component *i* in the solution  
- **x_i**: Mole fraction of component *i*  
- **P_i^0**: Saturated vapor pressure of pure component *i*  

Raoult's Law applies to solvents and volatile solutes in **ideal solutions**, where intermolecular interactions between different components are negligible.

---

### Henry's Law

Henry's Law describes the solubility of gases in liquids:

\[
C = k_H \cdot P
\]

- **C**: Concentration of the gas in the liquid  
- **P**: Partial pressure of the gas above the liquid  
- **k_H**: Henry's constant, dependent on the solvent and temperature  

Henry's Law is widely used in **gas absorption**, **carbonated beverages**, and **environmental chemistry** to predict how much gas dissolves under a given pressure.

---

## 2. Relationship in Ideal Solutions

In **ideal solutions**, where solute-solvent interactions are negligible, Raoult's Law and Henry's Law exhibit similar linear behavior:

- **Raoult's Law**: Vapor pressure is proportional to mole fraction  
\[
P_i = x_i \cdot P_i^0
\]

- **Henry's Law**: Gas solubility is proportional to partial pressure  
\[
C = k_H \cdot P
\]

We can express Henry's Law in terms of partial pressure:

\[
P = \frac{C}{k_H} \approx C \cdot \frac{1}{k_H}
\]

When the gas reaches saturation (\(C_\text{sat}\)), the partial pressure equals the saturated vapor pressure \(P_\text{sat}\):

\[
P_\text{sat} = \frac{C_\text{sat}}{k_H} \implies \frac{1}{k_H} \approx P_\text{sat}
\]

Thus, in ideal solutions, **Raoult's Law and Henry's Law describe the same linear relationship from different perspectives**:

| Law | Focus | Relation |
|-----|-------|---------|
| Raoult | Vapor Pressure | \(P_i = x_i P_i^0\) |
| Henry | Gas Solubility | \(C = k_H P\) |

- Raoult emphasizes **vapor pressure changes**  
- Henry emphasizes **solute concentration changes**

---

## 3. Differences in Real Solutions

In real solutions, intermolecular interactions such as hydrogen bonding, van der Waals forces, or ionic interactions lead to deviations from ideal behavior.

**Raoult's Law deviations:**
- Vapor pressure may not be proportional to mole fraction  
- Positive deviation: weak solute-solvent interaction, higher vapor pressure than ideal  
- Negative deviation: strong solute-solvent interaction, lower vapor pressure than ideal  

**Henry's Law deviations:**
- Gas solubility may not be proportional to partial pressure  
- Affected by solvent composition, temperature, and solute-solvent interactions  

**Applicable range:**
- Raoult's Law: still valid for **solvent in dilute solutions**  
- Henry's Law: still valid for **trace gases in solution**

**Example:** Nitrogen in propylene  
- Liquid phase: mostly propylene, trace nitrogen  
- Raoult's Law: \(P_\text{propylene} \approx X_\text{propylene} P_\text{propylene}^0\)  
- Henry's Law: \(C_\text{N2} \approx k_H P_\text{N2}\)  

Even in non-ideal solutions, these laws can approximate vapor pressure and gas solubility.

---

## 4. Applications in Chemical Engineering

In industrial processes, **storage and transport of liquids** often involve **non-condensable gas (NCG) purging**. Gas flow can carry volatile liquid, causing material loss. Vapor pressure principles help **predict and minimize losses**.

**Calculating material loss:**
1. Vapor pressure of liquid in gas:

\[
P_\text{material} = X_\text{material} \cdot P_\text{material}^0
\]

2. Gas-phase volume fraction:

\[
y_\text{material} = \frac{P_\text{material}}{P_\text{total}}
\]

3. Reduction strategies:
- **Increase system pressure** → lowers gas-phase fraction  
- **Lower temperature** → reduces saturated vapor pressure

**Example:** Propylene storage tank purged with nitrogen, 20°C, 15 atm  

| Parameter | Value |
|-----------|-------|
| Mole fraction \(X_\text{C3H6}\) | 1 |
| Saturated vapor pressure \(P_\text{C3H6}^0\) | 10 atm |
| System pressure \(P_\text{total}\) | 15 atm |
| Gas-phase fraction \(y_\text{C3H6}\) | 10/15 ≈ 0.667 |

- Increasing pressure decreases \(y_\text{C3H6}\)  
- Lowering temperature (e.g., 0°C, \(P_\text{C3H6}^0 \approx 5.7\) atm) → \(y_\text{C3H6} \approx 0.38\)

This significantly reduces propylene loss during nitrogen purging.

---

## 5. Summary

1. **Raoult's Law and Henry's Law** are similar in ideal solutions: one emphasizes vapor pressure, the other solubility.  
2. In real solutions, deviations exist, but Raoult's Law for solvents and Henry's Law for trace gases remain approximately valid.  
3. Chemical engineers can apply these principles to predict material loss and optimize processes by adjusting **system pressure** and **temperature**.

---

