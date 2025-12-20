---
layout: page
title: Heat Exchanger Mini Lab
---

## Heat Exchanger Mini Lab Description

This mini-lab explores a liquid-liquid heat exchanger, a system designed to transfer thermal energy from a hot water stream to a cold water stream without allowing the two fluids to mix. The experimental setup consists of two separate water reservoirs: one maintained at a higher temperature and the other kept at a lower temperature. These reservoirs are connected through flexible tubing and a compact heat exchanger unit.

Hot water is supplied from a heated tank, where an immersion heater maintains a relatively stable temperature. Cold water is drawn from an insulated container filled with ice water to ensure a consistently low inlet temperature. Both fluid streams are circulated through the system using external pumps, which help maintain steady and controlled flow rates during operation. The hot and cold streams enter the heat exchanger through separate inlet ports and flow through internal channels that are thermally coupled but physically isolated. This design allows heat to be transferred through the tube walls while preventing any direct mixing of the fluids.

A key feature of this system is its reconfigurable tubing arrangement, which allows the heat exchanger to operate under different flow configurations. By rearranging the tubing, the exchanger can be run in parallel flow**, **counterflow, or hybrid series/parallel configurations. In a parallel flow setup, both the hot and cold streams enter the exchanger from the same end and flow in the same direction. In a counterflow configuration, the streams enter from opposite ends and move in opposite directions, which increases the temperature gradient along the length of the exchanger. Series and parallel arrangements modify the effective heat transfer area and influence the residence time of the fluids within the system.

Temperature sensors are placed at both the inlet and outlet of the hot and cold streams to measure temperature changes across the exchanger. These measurements provide qualitative insight into the effectiveness of heat transfer for each flow configuration. During operation, heat is transferred from the hot water to the cold water, resulting in a decrease in the hot stream’s outlet temperature and a corresponding increase in the cold stream’s outlet temperature.

Overall, this lab setup serves as a simplified model of real-world heat exchangers commonly used in applications such as power plants, HVAC systems, automotive radiators, and industrial process equipment. The experiment highlights how flow arrangement and system configuration influence heat transfer performance**, making it an effective educational tool for understanding fundamental thermodynamic principles.

## Schematics
### System Diagram: Parallel Flow (Max Flow Rate)

        Hot In (T_h,in, ṁ_h = max)  ──▶
        Cold In (T_c,in, ṁ_c = max) ──▶
              ┌───────────────────────┐
              │     HEAT EXCHANGER     │
              │        (CV)            │
              │   Q̇_h→c (internal)     │
              └───────────────────────┘
        Hot Out (T_h,out) ─────────▶
        Cold Out (T_c,out) ───────▶

Assumptions:
- Steady-state operation
- No work transfer (Ẇ = 0)
- Heat transfer occurs only between streams

### System Diagram: Counterflow (Hot Max, Cold Parallel)

        Hot In (T_h,in, ṁ_h = max) ◀───
        Cold In (T_c,in, ṁ_c = max) ──▶
              ┌───────────────────────┐
              │     HEAT EXCHANGER     │
              │        (CV)            │
              │   Q̇_h→c (internal)     │
              └───────────────────────┘
        Hot Out (T_h,out) ─────────▶
        Cold Out (T_c,out) ◀───────

Assumptions:
- Steady-state control volume
- No work interactions
- Enhanced temperature gradient along length

### System Diagram: Parallel Flow (Hot Max, Cold Min)

        Hot In (T_h,in, ṁ_h = max)  ──▶
        Cold In (T_c,in, ṁ_c = min) ──▶
              ┌───────────────────────┐
              │     HEAT EXCHANGER     │
              │        (CV)            │
              │   Q̇_h→c (internal)     │
              └───────────────────────┘
        Hot Out (T_h,out) ─────────▶
        Cold Out (T_c,out) ───────▶

Assumptions:
- Cold stream has longer residence time
- No external heat losses
- No work transfer

### System Diagram: Counterflow (Hot Max, Cold Min)

        Hot In (T_h,in, ṁ_h = max) ◀───
        Cold In (T_c,in, ṁ_c = min) ──▶
              ┌───────────────────────┐
              │     HEAT EXCHANGER     │
              │        (CV)            │
              │   Q̇_h→c (internal)     │
              └───────────────────────┘
        Hot Out (T_h,out) ─────────▶
        Cold Out (T_c,out) ◀───────

Assumptions:
- Maximum temperature effectiveness
- Strong thermal gradient maintained
- Steady-state CV, no work transfer


These system diagrams illustrate how changes in flow direction and mass flow rates alter the temperature gradients and heat transfer effectiveness of the heat exchanger.

## Experimental Setup

![Heat exchanger experimental setup showing hot and cold reservoirs, tubing, and pumps](IMG_0756.png)
*Figure 1: Heat exchanger experimental setup with hot and cold water reservoirs.*

![Alternate view of the heat exchanger highlighting tubing configuration and temperature probes](IMG_0757.png)
*Figure 2: Alternate view showing tubing connections and instrumentation.*


## Experimental Data Summary
*Table 1: Summary of measured reservoir temperatures for each heat exchanger configuration tested during the mini-lab.*

| Trial | Flow Configuration | Hot Flow Rate | Cold Flow Rate | Initial Cold Temp (K) | Initial Hot Temp (K) | Time (s) | Final Cold Temp (K) | Final Hot Temp (K) |
|------:|-------------------|---------------|----------------|-----------------------|----------------------|----------|---------------------|--------------------|
| 1 | Parallel | Max | Max | 280.0 | 314.35 | 22.95 | 294.0 | 297.3 |
| 2 | Hot Counterflow, Cold Parallel | Max | Max | 283.0 | 307.15 | 22.18 | 295.1 | 292.4 |
| 3 | Parallel | Max | Low | 282.6 | 307.25 | 22.51 | 294.2 | 296.2 |
| 4 | Counterflow | Max | Low | 308.15 | 282.5 | 22.95 | 293.9 | 290.5 |


## Governing Balance Equations

The heat exchanger is modeled as a **steady-state control volume (CV)** with two fluid streams (hot and cold) exchanging heat internally. No work interactions are present, and mass does not accumulate within the system.

### Assumptions
- Steady-state operation
- Incompressible liquid water
- Constant specific heat, \( c_p \)
- No phase change
- Negligible kinetic and potential energy changes
- Negligible heat loss to surroundings
- No work transfer: \( \dot{W} = 0 \)

---

## Mass Balance

For each fluid stream (hot and cold), mass is conserved independently:

\[
\dot{m}_{in} = \dot{m}_{out}
\]

Thus,

\[
\dot{m}_h^{in} = \dot{m}_h^{out}, \quad
\dot{m}_c^{in} = \dot{m}_c^{out}
\]

Flow rate settings (max vs. low) affect the **magnitude** of \( \dot{m} \), but not the form of the balance.

---

## Energy Balance

For the overall heat exchanger control volume:

\[
\sum \dot{m}_{in} h_{in} - \sum \dot{m}_{out} h_{out} + \dot{Q} - \dot{W} = 0
\]

With \( \dot{W} = 0 \) and negligible heat loss to the environment, the energy balance reduces to:

\[
\dot{m}_h c_p (T_{h,in} - T_{h,out}) = \dot{m}_c c_p (T_{c,out} - T_{c,in})
\]

This equation represents the **fundamental physics of heat exchange**:  
energy lost by the hot stream equals energy gained by the cold stream.

---

## Entropy Balance

For a steady-state control volume:

\[
\sum \dot{m}_{out} s_{out} - \sum \dot{m}_{in} s_{in} = \dot{S}_{gen}
\]

Since heat transfer occurs internally between the streams and irreversibly:

\[
\dot{S}_{gen} \ge 0
\]

Using incompressible liquid approximation:

\[
\dot{S}_{gen} =
\dot{m}_c c_p \ln\!\left(\frac{T_{c,out}}{T_{c,in}}\right)
+
\dot{m}_h c_p \ln\!\left(\frac{T_{h,out}}{T_{h,in}}\right)
\]

Entropy generation arises from **finite temperature differences** between the hot and cold streams during heat transfer.

---

## Application to Individual Trials

### Trial 1: Parallel Flow, Max Flow Rates
- High \( \dot{m}_h \) and \( \dot{m}_c \)
- Short residence time
- Lower effectiveness compared to counterflow
- Moderate entropy generation due to large inlet temperature difference

---

### Trial 2: Hot Counterflow, Cold Parallel (Max Flow Rates)
- Opposing flow directions maintain a higher temperature gradient
- Greater heat transfer effectiveness
- Lower entropy generation compared to parallel flow
- Cold outlet temperature approaches hot inlet temperature more closely

---

### Trial 3: Parallel Flow, Hot Max / Cold Low
- Reduced cold-side mass flow increases residence time
- Larger temperature rise per unit mass of cold fluid
- Energy balance dominated by smaller \( \dot{m}_c \)
- Increased entropy generation due to imbalance in heat capacity rates

---

### Trial 4: Counterflow, Hot Max / Cold Low
- Most thermodynamically effective configuration
- Strong temperature gradient maintained throughout exchanger
- Cold outlet temperature increases significantly
- Entropy generation minimized relative to other configurations

---

*These balance equations capture the essential thermodynamic behavior of the heat exchanger and explain how changes in flow configuration and mass flow rates influence performance.*
