---
title: "Raoult's Law vs Henry's Law — Reducing Material Loss from NCG Emissions"
date: 2025-12-16
description: "How Raoult's Law and Henry's Law explain and help reduce material loss caused by non-condensable gas emissions in chemical engineering systems."
keywords: [Raoult's Law, Henry's Law, NCG emissions, material loss, VLE, chemical engineering]
author: "Hadel"
---

<!-- MathJax -->
<script>
window.MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']],
    displayMath: [['$$', '$$'], ['\\[', '\\]']]
  },
  options: {
    processHtmlClass: 'mathjax',
    skipHtmlTags: ['script', 'noscript', 'style', 'textarea', 'pre', 'code']
  }
};
</script>
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

## Engineering Problem: Material Loss Caused by NCG Emissions

In many **chemical engineering systems**—such as storage tanks, reactors, absorbers, and transfer lines—**non-condensable gases (NCGs)** are inevitably present.  
Typical NCGs include nitrogen, hydrogen, methane, or purge gases used for safety and process control.

During **venting or purging operations**, NCGs carry volatile liquid components into the vapor phase, leading to:

- Loss of valuable raw materials  
- Increased emissions and environmental impact  
- Higher operating and recovery costs  

A key engineering question therefore arises:

> **How can material loss caused by non-condensable gas emissions be quantitatively estimated and effectively reduced?**

The answer lies in understanding **vapor–liquid equilibrium (VLE)** behavior, which is fundamentally governed by **Raoult’s Law** and **Henry’s Law**.  
This article explains how these two laws describe the same thermodynamic reality from different perspectives and how they can be used to minimize material loss in real engineering systems.

---

## 1. Raoult’s Law and Henry’s Law

### 1.1 Raoult’s Law

**Raoult’s Law** describes the vapor pressure contribution of a volatile component in an **ideal liquid mixture**.  
It is most accurate for **solvents or major components** when intermolecular interactions are similar.

**Mathematical expression:**

<div class="mathjax">
$$
P_i = x_i \cdot P_i^0
$$
</div>

**Symbol definitions (engineering notation):**

- P<sub>i</sub>: partial vapor pressure of component *i*  
- x<sub>i</sub>: mole fraction of component *i* in the liquid phase  
- P<sub>i</sub><sup>0</sup>: saturated vapor pressure of pure component *i* at system temperature  

**Example**

A liquid mixture contains 50 mol% ethanol at 25 °C.  
The saturated vapor pressure of pure ethanol is 0.08 atm.

<div class="mathjax">
$$
P_{\text{ethanol}} = 0.5 \times 0.08 = 0.04\ \text{atm}
$$
</div>

This means ethanol contributes **0.04 atm** to the total vapor pressure.

---

### 1.2 Henry’s Law

**Henry’s Law** describes the equilibrium solubility of a **dilute gas** in a liquid.  
It is applicable to **trace gas components**, such as nitrogen dissolved in hydrocarbons.

**Mathematical expression:**

<div class="mathjax">
$$
C = k_H \cdot P
$$
</div>

**Symbol definitions:**

- C: concentration of dissolved gas in the liquid  
- P: partial pressure of the gas in the vapor phase  
- k<sub>H</sub>: Henry’s constant (depends on solvent and temperature)  

**Typical engineering applications:**

- Gas absorption and stripping  
- Purge gas design  
- Environmental air–water equilibrium calculations  

---

## 2. Relationship Between Raoult’s Law and Henry’s Law

Although Raoult’s Law and Henry’s Law are often taught separately, they describe **linear equilibrium behavior in ideal systems**.

### Linear equilibrium forms

- **Liquid → vapor (Raoult’s Law)**

<div class="mathjax">
$$
P_i = x_i \cdot P_i^0
$$
</div>

- **Gas → liquid (Henry’s Law)**

<div class="mathjax">
$$
C = k_H \cdot P
$$
</div>

Henry’s Law can be rearranged to express vapor pressure:

<div class="mathjax">
$$
P = \frac{C}{k_H}
$$
</div>

At **gas saturation**, the dissolved concentration reaches C<sub>sat</sub>, and the corresponding vapor pressure equals the saturated vapor pressure P<sub>sat</sub>:

<div class="mathjax">
$$
P_{\text{sat}} = \frac{C_{\text{sat}}}{k_H}
$$
</div>

### Conceptual comparison
- **Raoult’s Law**  
  **Engineering focus:** Vapor pressure of volatile liquids  
  **Mathematical form:** P<sub>i</sub> = x<sub>i</sub> P<sub>i</sub><sup>0</sup>

- **Henry’s Law**  
  **Engineering focus:** Solubility of trace gases  
  **Mathematical form:** C = k<sub>H</sub> P<br>
**Key insight:**  
In ideal systems, both laws describe the **same linear thermodynamic behavior**, but from opposite phase perspectives.

---

## 3. Deviations in Real Solutions

Real industrial systems deviate from ideality due to intermolecular forces.

### 3.1 Raoult’s Law deviations

- Vapor pressure no longer scales linearly with composition  
- **Positive deviation:** weaker interactions → higher vapor pressure  
- **Negative deviation:** stronger interactions → lower vapor pressure  

### 3.2 Henry’s Law deviations

- Valid mainly at low gas concentrations  
- Strong dependence on temperature and solvent composition  

### Practical engineering validity

- Raoult’s Law remains valid for **major liquid components**  
- Henry’s Law remains valid for **trace non-condensable gases**

**Example: Nitrogen dissolved in liquid propylene**

- Liquid phase: mostly propylene  
- Gas phase: nitrogen-rich purge gas  

<div class="mathjax">
$$
P_{\text{propylene}} \approx x_{\text{propylene}} \cdot P_{\text{propylene}}^0
$$
</div>

<div class="mathjax">
$$
C_{\text{N}_2} \approx k_H \cdot P_{\text{N}_2}
$$
</div>

These approximations are widely used in purge and vent loss calculations.

---

## 4. Engineering Application: Reducing Material Loss from NCG Emissions

During NCG purging, volatile liquids evaporate into the gas phase and are discharged.

### Step 1: Vapor pressure of the liquid component

<div class="mathjax">
$$
P_{\text{material}} = x_{\text{material}} \cdot P_{\text{material}}^0
$$
</div>

### Step 2: Gas-phase mole fraction

<div class="mathjax">
$$
y_{\text{material}} = \frac{P_{\text{material}}}{P_{\text{total}}}
$$
</div>

### Loss reduction strategies

- Increase total system pressure  
- Reduce operating temperature  
- Minimize purge flow rate  

### Example: Propylene tank purged with nitrogen


At 20 °C and a total pressure of 15 atm, the saturated vapor pressure of propylene is 10 atm, and the liquid phase consists almost entirely of propylene (mole fraction ≈ 1). Under these conditions, the mole fraction of propylene in the vapor phase can be calculated as follows:

<div class="mathjax"> $$ y_{\text{C3H6}} = \frac{P_{\text{C3H6}}}{P_{\text{total}}} = \frac{10}{15} \approx 0.667 $$ </div>

The relationship between the volume of non-condensable gas (NCG) purged and the propylene lost is given by:

<div class="mathjax"> $$ V_{\text{C3H6,loss}} = \frac{y_{\text{C3H6}}}{1 - y_{\text{C3H6}}} \cdot V_{\text{NCG}} $$ </div>

For example, if 100 L of NCG is purged at this condition:

<div class="mathjax"> $$ V_{\text{C3H6,loss}} \approx \frac{0.667}{1 - 0.667} \cdot 100 \approx 200\ \text{L} $$ </div>

If the temperature is lowered to 0 °C, the saturated vapor pressure of propylene decreases to approximately 5.7 atm. The vapor-phase mole fraction becomes:

<div class="mathjax"> $$ y_{\text{C3H6}} = \frac{5.7}{15} \approx 0.38 $$ </div>

Purging 100 L of NCG under this condition results in:

<div class="mathjax"> $$ V_{\text{C3H6,loss}} \approx \frac{0.38}{1 - 0.38} \cdot 100 \approx 61\ \text{L} $$ </div>

If the total system pressure is increased to 30 atm at 20 °C (with saturated vapor pressure still 10 atm):

<div class="mathjax"> $$ y_{\text{C3H6}} = \frac{10}{30} \approx 0.333 $$ $$ V_{\text{C3H6,loss}} \approx \frac{0.333}{1 - 0.333} \cdot 100 \approx 50\ \text{L} $$ </div>

Conclusion:
Lowering temperature or increasing total pressure both significantly reduce propylene loss during NCG purging. 

---

## 5. Summary

1. Material loss from non-condensable gas emissions originates from vapor–liquid equilibrium behavior.  
2. **Raoult’s Law** governs volatile liquid evaporation, while **Henry’s Law** governs trace gas solubility.  
3. Applying these principles enables effective **pressure control, temperature optimization, and loss reduction** in chemical engineering systems.

---
## Recommended Engineering Tool
To make calculations easier, I developed an app that can calculate the **saturated vapor pressure for hundreds of chemical substances**. You can download it here: [Vapor Pressure Calculator App](https://play.google.com/store/apps/details?id=com.zhanghd.vapor)

---

**Author:** Hadel  
**Published:** 2025-12-16  
**Citation:** chem.zhanghd.fun  

