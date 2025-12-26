---
title: "Why Light Hydrocarbon Distillation Towers Always Carry Water at the Top"
date: 2025-12-26
description: "Explains why light hydrocarbon distillation columns inevitably carry water at the top and why increasing reflux ratio does not help, using the propane–butane system as an example."
keywords: [light hydrocarbons, distillation, water carryover, reflux ratio, phase equilibrium, chemical engineering]
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

## 1. A Common Problem in Almost All Light Hydrocarbon Units

In **light hydrocarbon distillation units**, engineers frequently encounter the following phenomenon:  

Even when the feed contains only **trace amounts of water**, it can travel with the hydrocarbon vapor all the way to the **top of the column**.  

This seems counterintuitive. Water boils at 100 °C at atmospheric pressure, whereas propane and butane boil at −42 °C and −0.5 °C, respectively.  

Intuitively, one would expect that with enough trays and sufficient reflux, the water would be “washed” back to the column bottom.  

In practice, however, **water still appears at the top**, and paradoxically, increasing the reflux ratio often **makes water carryover worse**.  

Interestingly, in methanol–water distillation, as long as separation is sufficient, the top product can be almost completely water-free.  

> Why is water nearly impossible to block in light hydrocarbon systems, while it can be entirely removed in methanol systems?

---

## 2. Let’s Be Clear: This Is Not a Separation Efficiency Issue

Before discussing the mechanism, an important engineering conclusion must be emphasized:  

**Water carryover at the top of light hydrocarbon columns is not necessarily due to operational or design issues, but is often determined by phase equilibrium limits.**  

If the following conditions are met:  
- Hydrocarbons and water are **immiscible**  
- **Vapor–liquid equilibrium** is established in the column  

Then the **maximum water fraction the top can carry** can be calculated directly at the given top temperature and pressure. Increasing the reflux ratio **cannot surpass this physical limit**.

---

## 3. Key Mechanism: “Simultaneous Vaporization” in Immiscible Systems

The fundamental difference between light hydrocarbon–water and methanol–water systems lies in **miscibility**.  

For systems where water and hydrocarbons form **separate immiscible layers**:  

- At a given temperature, the **total system vapor pressure** equals the sum of the saturated vapor pressures of each liquid phase.  
- When the total vapor pressure equals the operating pressure, **both phases vaporize simultaneously**.  
- The proportion of each component entering the vapor phase is determined **by its own saturated vapor pressure**, not by its relative boiling point.  

---

## 4. An Intuitive Engineering Example: Butane–Water System

Consider a butane–water system at 210.3 kPa and 20 °C:  

- Butane’s saturated vapor pressure ≈ 208 kPa  
- Water’s saturated vapor pressure ≈ 2.3 kPa  

Total pressure: 208 + 2.3 ≈ 210.3 kPa  

Boiling occurs, and because butane and water form separate layers, both vaporize simultaneously in the ratio ≈ 208:2.3.  

This means that even though water’s boiling point is far higher than butane’s, **it still inevitably enters the ascending vapor as a small fraction**, fully dictated by **phase equilibrium**—not tray number or reflux ratio.  

---

## 5. How Much Water Can the Top Actually Carry?

Example: Propane–Butane Column  

- Top pressure: 1.5 MPa (absolute)  
- Top temperature: 44 °C  
- Saturated vapor pressure of water at 44 °C: 9.1 kPa  

Since hydrocarbons and water are immiscible, and free water exists at the top, the **partial pressure of water** in the vapor can be approximated by its saturation pressure.  

Maximum mole fraction of water at the top:  

<div class="mathjax">
$$
y_{\mathrm{H_2O}}^{\max} \approx \frac{P_{\mathrm{H_2O}}^{\mathrm{sat}}}{P_{\mathrm{top}}} = \frac{9.1}{1500} \approx 0.0061
$$
</div>

≈ 0.61 mol% water. This is the **physical limit** determined by temperature and pressure.

---

## 6. Engineering Formula for Maximum Water Carryover

Let:  

- $G_D$ = molar flow of top product  
- $G_R$ = molar flow of top reflux  
- $G_{\text{top}} = G_D + G_R$ = total vapor flow entering the condenser  

Then the **maximum water flow** carried by the top vapor is:  

<div class="mathjax">
$$
G_{\mathrm{H_2O}}^{\max} = \frac{P_{\mathrm{H_2O}}^{\mathrm{sat}}}{P_{\mathrm{top}}} (G_D + G_R)
$$
</div>

Substituting the numbers:  

<div class="mathjax">
$$
G_{\mathrm{H_2O}}^{\max} \approx \frac{9.1}{1500} (G_D + G_R)
$$
</div>

This represents the top’s **maximum theoretical water-carrying capacity** under these operating conditions.

---

## 7. Three Engineering Conclusions

**1️⃣ When is the bottom guaranteed to be water-free?**  

If the feed water content is **less than the top’s maximum water-carrying capacity** and the condenser/reflux drum can completely remove free water, then all feed water will be carried away by the top vapor.  
The bottom product remains water-free.

**2️⃣ Why does increasing the reflux ratio make top water carryover worse?**  

Because:  

<div class="mathjax">
$$
G_{\text{top}} = G_D + G_R
$$
</div>

Increasing reflux → higher total top vapor flow → higher theoretical water-carrying capacity.  
Phase equilibrium does **not** change; only the vapor pathway for water is amplified.

**3️⃣ Water content on trays along the column**  

- Vapor moves up the column, and temperature decreases along the way.  
- Water’s saturation pressure drops, reducing the vapor’s water-carrying ability.  
- With small feed water, condensation may occur at some intermediate tray and drain back to the bottom.  

---

## 8. Engineering Measures: How to Ensure Water-Free Bottom Product

To make the bottom completely water-free, the **core goal** is to ensure all feed water is carried by the top vapor and removed in the condenser.  

**Key measures include:**  

**1. Control feed water content**  
- Feed water must be less than the top’s theoretical maximum water-carrying capacity ($G_{\mathrm{H_2O}}^{\max}$).  
- Otherwise, water will appear at the bottom even with perfect cut-water measures.  

**2. Top liquid–liquid separation and water cut**  
- Equip the top reflux drum with reliable liquid–liquid separation.  
- Remove condensed water completely, preventing it from returning into the column.  
- This is the **most critical step** to ensure all feed water is carried away.  

**3. Tray water cut points**  
- Install water cut points at appropriate trays to remove condensed water.  
- Prevent local water accumulation or entrainment along the column.  

**4. Reflux ratio effect on top water-carrying capacity**  
- Increasing reflux increases total top vapor flow, enhancing the top’s theoretical water-carrying capacity.
  
---
## Recommended Engineering Tool
To make calculations easier, We developed an app that can calculate the **saturated vapor pressure for hundreds of chemical substances**. You can download it here: [Vapor Pressure Calculator App](https://play.google.com/store/apps/details?id=com.zhanghd.vapor)

---
<div class="post-nav" style="display:flex; justify-content:space-between; margin-top:2em;">
  {% if page.previous %}
    <a href="{{ page.previous.url }}" class="button">← Previous: {{ page.previous.title }}</a>
  {% endif %}
  {% if page.next %}
    <a href="{{ page.next.url }}" class="button">Next: {{ page.next.title }} →</a>
  {% endif %}
</div>
---
Author: Hadel  
Published: 2025-12-26  
Source: chem.zhanghd.fun

