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


