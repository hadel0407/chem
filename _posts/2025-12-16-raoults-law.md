---
title: "Raoult's Law vs Henry's Law: Vapor Pressure and Gas Solubility Explained"
date: 2025-12-16
description: "Learn the differences between Raoult's Law and Henry's Law, their behavior in ideal and real solutions, and practical applications in chemical engineering processes."
---

# Raoult's Law vs Henry's Law: Vapor Pressure and Gas Solubility Explained

In **physical chemistry** and **chemical engineering**, understanding solution behavior is essential. Two fundamental laws describe how components interact in solutions:

- **Raoult's Law**: Relates the vapor pressure of liquid components to their mole fraction.  
- **Henry's Law**: Relates the solubility of gases in liquids to the gas's partial pressure.  

While they apply to different substances, in **ideal solutions**, their behavior is analogous. This article covers:

1. Definitions and formulas  
2. Behavior in ideal solutions  
3. Deviations in real solutions  
4. Applications in chemical engineering

---

## 1. Raoult's Law and Henry's Law

### Raoult's Law

Raoult's Law predicts the **vapor pressure of a component in a liquid mixture**. It is accurate for **solvents and volatile solutes in ideal solutions**, where **intermolecular interactions** between components are negligible.

**Formula:**

$$
P_i = x_i \cdot P_i^{0}
$$

**Where:**  
- \(P_i\) = Partial vapor pressure of component *i*  
- \(x_i\) = Mole fraction of component *i*  
- \(P_i^{0}\) = Saturated vapor pressure of pure component *i*  

**Example:**  
A solution contains 50% ethanol (\(x_{\rm ethanol} = 0.5\)), and the saturated vapor pressure of pure ethanol at 25°C is \(P_{\rm ethanol}^{0} = 0.08 \, \rm atm\). Then:

$$
P_{\rm ethanol} = x_{\rm ethanol} \cdot P_{\rm ethanol}^{0} = 0.5 \times 0.08 = 0.04 \, \rm atm
$$

---

### Henry's Law

Henry's Law describes how **gases dissolve in liquids**. The solubility is proportional to the gas's partial pressure above the liquid:

$$
C = k_H \cdot P
$$

**Where:**  
- \(C\) = Concentration of the gas in the liquid  
- \(P\) = Partial pressure of the gas above the liquid  
- \(k_H\) = Henry's constant (depends on solvent and temperature)  

**Applications:** Gas absorption, carbonated beverages, and environmental chemistry.

---

## 2. Relationship in Ideal Solutions

In **ideal solutions**, solute-solvent interactions are negligible. Both laws exhibit **linear behavior**:

- **Raoult's Law**: Vapor pressure ∝ mole fraction

$$
P_i = x_i \cdot P_i^{0}
$$

- **Henry's Law**: Gas solubility ∝ partial pressure

$$
C = k_H \cdot P
$$

Henry's Law can also be expressed in terms of partial pressure:

$$
P = \frac{C}{k_H} \approx C \cdot \frac{1}{k_H}
$$

At **saturation** (\(C_{\rm sat}\)):

$$
P_{\rm sat} = \frac{C_{\rm sat}}{k_H} \implies \frac{1}{k_H} \approx P_{\rm sat}
$$

**Comparison Table:**

| Law    | Focus            | Mathematical Relation         |
|--------|-----------------|-------------------------------|
| Raoult | Vapor Pressure   | \(P_i = x_i P_i^{0}\)       |
| Henry  | Gas Solubility   | \(C = k_H P\)               |

- **Raoult** emphasizes changes in vapor pressure  
- **Henry** emphasizes changes in solute concentration  

---

## 3. Deviations in Real Solutions

In **non-ideal solutions**, intermolecular interactions (hydrogen bonding, van der Waals, ionic forces) cause deviations.

### Raoult's Law Deviations

- Vapor pressure may **not scale linearly** with mole fraction  
- **Positive deviation**: Weak solute-solvent interaction → higher vapor pressure  
- **Negative deviation**: Strong interaction → lower vapor pressure  

### Henry's Law Deviations

- Gas solubility may **not scale linearly** with partial pressure  
- Influenced by solvent composition, temperature, and solute-solvent interaction  

**Applicability:**

- Raoult: Still valid for **solvent in dilute solutions**  
- Henry: Still valid for **trace gases in solution**  

**Example: Nitrogen in Propylene**

- Liquid: Mostly propylene, trace nitrogen  
- Raoult: \(P_{\rm propylene} \approx X_{\rm propylene} P_{\rm propylene}^{0}\)  
- Henry: \(C_{\rm N2} \approx k_H P_{\rm N2}\)  

Even in non-ideal mixtures, these laws provide reliable approximations.

---

## 4. Applications in Chemical Engineering

In industrial processes, **non-condensable gas (NCG) purging** can carry volatile liquids, causing material loss. Understanding vapor pressure helps **predict and minimize losses**.

### Step 1: Vapor pressure of liquid in gas

$$
P_{\rm material} = X_{\rm material} \cdot P_{\rm material}^{0}
$$

### Step 2: Gas-phase volume fraction

$$
y_{\rm material} = \frac{P_{\rm material}}{P_{\rm total}}
$$

### Mitigation Strategies

- **Increase system pressure** → reduces gas-phase fraction  
- **Lower temperature** → reduces saturated vapor pressure  

**Example:** Propylene tank purged with nitrogen at 20°C, 15 atm  

| Parameter                        | Value                   |
|---------------------------------|------------------------|
| Mole fraction \(X_{\rm C3H6}\)   | 1                      |
| Saturated vapor pressure \(P_{\rm C3H6}^{0}\) | 10 atm |
| System pressure \(P_{\rm total}\) | 15 atm               |
| Gas-phase fraction \(y_{\rm C3H6}\) | 10/15 ≈ 0.667      |

- Increasing pressure decreases \(y_{\rm C3H6}\)  
- Lowering temperature to 0°C (\(P_{\rm C3H6}^{0} \approx 5.7 \, \rm atm\)) → \(y_{\rm C3H6} \approx 0.38\)  

✅ **Result:** Significant reduction in propylene loss during NCG purging.

---

## 5. Summary

1. Raoult's Law and Henry's Law behave similarly in **ideal solutions**, differing mainly in perspective (vapor pressure vs solubility).  
2. Deviations occur in real solutions, but Raoult's Law for solvents and Henry's Law for trace gases remain useful.  
3. Chemical engineers can optimize **pressure and temperature** to minimize material losses using these principles.
