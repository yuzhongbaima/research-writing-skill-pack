# Domain Workflows

This reference specializes the suite for four engineering-oriented domains:

- transportation engineering
- energy saving and environmental engineering
- ocean engineering
- low-altitude aircraft systems

Use this file when the paper topic is domain-heavy and the generic engineering workflow needs to be tightened around domain-specific evidence, variables, and reviewer expectations.

## Shared domain workflow frame

For all four domains, keep this order:

1. define the engineering system and boundary
2. identify the practical decision problem
3. map the evidence ladder available to the paper
4. compare against domain-appropriate baselines
5. report conditions, uncertainty, and feasibility
6. preflight likely reviewer objections before polishing

## Transportation Engineering

### Typical contribution shapes

- traffic prediction or control strategy
- transport network optimization
- logistics or scheduling method
- safety analysis or risk assessment
- energy consumption or emissions reduction under transport scenarios
- intelligent transportation system integration or deployment study

### Preferred workflow emphasis

#### Literature review

- Compare by network scale, transport mode, temporal granularity, and decision horizon.
- Separate simulation-only studies from studies with detector, trajectory, fleet, or operational data.
- Track policy or regulatory context when it materially affects the problem.

#### Research positioning

- Frame the problem in terms of throughput, delay, reliability, safety, emissions, or operating cost.
- Make clear whether the paper targets strategic planning, tactical optimization, or real-time control.

#### Method design

- State the network or corridor boundary, demand assumptions, and control variables.
- Distinguish prediction, optimization, simulation, and deployment modules.
- Explain data availability and update frequency if the method is operational.

#### Figures and tables

- Use time-series plots, network diagrams, spatiotemporal heatmaps, or tradeoff tables.
- Report axes, units, and scenario definitions explicitly.

#### Reviewer preflight

- Are baselines realistic for the same network scale and information availability?
- Are claims about real-world deployment overstated if the study is only simulation-based?
- Are robustness checks done across demand fluctuations, incidents, or weather effects if relevant?

### Common evaluation dimensions

- delay or travel time
- queue length or congestion level
- safety surrogate metrics
- energy use and emissions
- reliability and robustness
- computational latency for online methods

## Energy Saving and Environmental Engineering

### Typical contribution shapes

- efficiency improvement mechanism
- low-carbon process or control strategy
- pollution reduction or treatment performance study
- multi-objective energy-environment optimization
- lifecycle or system-level sustainability assessment
- monitoring, diagnosis, or management framework

### Preferred workflow emphasis

#### Literature review

- Compare by system boundary, pollutant type, energy form, and accounting method.
- Distinguish lab-scale results, pilot-scale results, and full-scale engineering deployment.
- Watch for inconsistent baselines, reporting units, and normalization methods.

#### Research positioning

- Frame significance through energy intensity, carbon reduction, pollutant removal, lifecycle impact, safety, or compliance.
- Make explicit whether the paper's claim is mechanism discovery, performance optimization, process integration, or system assessment.

#### Method design

- State material balance, energy balance, assumptions, and omitted losses where relevant.
- Separate process model, optimization layer, control strategy, and measurement layer.
- Include cost and feasibility hooks if the paper implies engineering deployment value.

#### Figures and tables

- Use Sankey or flow diagrams, performance-versus-condition plots, removal-efficiency tables, or cost-emission tradeoff plots.
- Always label functional unit, normalization basis, and operating conditions.

#### Reviewer preflight

- Is carbon, energy, or pollutant accounting method defensible and transparent?
- Are comparisons fair in terms of feed conditions, residence time, load, or reactor scale?
- Are economic or environmental claims larger than the available evidence supports?

### Common evaluation dimensions

- energy intensity or energy saving rate
- removal efficiency or emission reduction
- lifecycle impact indicators
- cost or payback
- stability and repeatability
- scale-up feasibility

## Ocean Engineering

### Typical contribution shapes

- hydrodynamic or structural design method
- offshore system control or monitoring strategy
- mooring, station-keeping, or trajectory solution
- marine energy device optimization
- underwater sensing, communication, or inspection framework
- experimental tank validation or field case study

### Preferred workflow emphasis

#### Literature review

- Compare by sea state, water depth, platform type, loading condition, and validation regime.
- Distinguish analytical models, CFD studies, tank tests, and field measurements.
- Track assumptions about waves, currents, wind, and coupling effects.

#### Research positioning

- Frame value through survivability, stability, efficiency, inspection quality, safety, maintenance, or operational cost.
- Clarify whether the novelty is model fidelity, control strategy, hardware system, or operational method.

#### Method design

- State environmental loads, coordinate frames, coupling assumptions, and scale-model conditions.
- Separate fluid model, structural model, control logic, sensing, and mission or operating workflow.
- Be explicit about numerical settings or experimental facilities when they are central to validity.

#### Figures and tables

- Use system schematics, sea-state comparison plots, response-amplitude curves, trajectory plots, or loading tables.
- Include units, sea-state definitions, and test conditions in the figure or caption.

#### Reviewer preflight

- Are conclusions too broad relative to the tested sea states or operating envelope?
- Are scale effects and simplifications acknowledged?
- If the work is simulation-dominant, is there enough validation against experimental or field references?

### Common evaluation dimensions

- stability and motion response
- structural load or fatigue indicators
- control accuracy or station-keeping performance
- energy capture or energy efficiency
- mission success under marine uncertainty
- robustness under environmental disturbance

## Low-Altitude Aircraft Systems

### Typical contribution shapes

- vehicle design or subsystem integration
- guidance, navigation, and control method
- mission planning or airspace coordination
- energy management or endurance improvement
- safety assurance or fault diagnosis framework
- low-altitude logistics, surveillance, or inspection deployment study

### Preferred workflow emphasis

#### Literature review

- Compare by platform class, payload, endurance, operating altitude, mission type, and validation environment.
- Distinguish simulation, hardware-in-the-loop, flight-test, and operational data evidence.
- Track regulatory, safety, communication, and weather constraints.

#### Research positioning

- Frame significance through safety, endurance, mission effectiveness, noise, energy use, operational cost, or airspace efficiency.
- Clarify whether the contribution is at vehicle, control, mission, or system-of-systems level.

#### Method design

- State flight envelope, mission profile, disturbances, sensor suite, control loop timing, and constraints.
- Separate vehicle model, estimation or perception, guidance and control, mission planner, and communication architecture.
- Note assumptions about communication latency, GNSS quality, weather, and fault modes if relevant.

#### Figures and tables

- Use mission-flow diagrams, trajectory plots, envelope charts, comparison tables, or safety-logic diagrams.
- Put test conditions, payload, wind, speed, and mission assumptions in captions.

#### Reviewer preflight

- Are flight-test claims being made from simulation-only evidence?
- Are safety and regulation implications addressed if the paper proposes real deployment?
- Are baselines fair in terms of platform capability, mission profile, and disturbance environment?

### Common evaluation dimensions

- tracking or navigation accuracy
- endurance and energy consumption
- mission completion rate
- safety margin and fault tolerance
- computational and communication latency
- deployability under realistic constraints

## Domain selection heuristic

- If the paper revolves around networks, traffic flow, fleets, routing, or multimodal systems, start from transportation engineering.
- If the paper revolves around energy efficiency, emissions, pollutants, carbon, reactors, treatment, or sustainability metrics, start from energy and environmental engineering.
- If the paper revolves around offshore structures, underwater systems, marine loads, sea states, or ocean energy, start from ocean engineering.
- If the paper revolves around UAVs, eVTOL, low-altitude logistics, flight control, airspace coordination, or onboard energy management, start from low-altitude aircraft systems.
