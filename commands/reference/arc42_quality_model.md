# Arc42 Quality Model

<arc42-quality-model>

Source: [https://quality.arc42.org](https://quality.arc42.org)

Model as at: 2026-06-14

| Attribute                     | What it covers                                                    | Source                                        |
| ----------------------------- | ----------------------------------------------------------------- | --------------------------------------------- |
| [Reliable](#reliable)         | Perform specified functions without interruptions or failures     | <https://quality.arc42.org/tag-reliable/>     |
| [Flexible](#flexible)         | Adapt to changes in requirements, contexts, or system environment | <https://quality.arc42.org/tag-flexible/>     |
| [Efficient](#efficient)       | Perform within time, capacity and resource parameters             | <https://quality.arc42.org/tag-efficient/>    |
| [Usable](#usable)             | Enable users to work safely, effectively and efficiently          | <https://quality.arc42.org/tag-usable/>       |
| [Secure](#secure)             | Protect data and defend against attack patterns                   | <https://quality.arc42.org/tag-secure/>       |
| [Safe](#safe)                 | Avoid states endangering life, health, or environment             | <https://quality.arc42.org/tag-safe/>         |
| [Operable](#operable)         | Easy to deploy, operate, monitor and control                      | <https://quality.arc42.org/tag-operable/>     |
| [Suitable](#suitable)         | Meet stated and implied needs of stakeholders                     | <https://quality.arc42.org/tag-suitable/>     |
| [Maintainable](#maintainable) | Analyze, modify, test and evolve with predictable effort          | <https://quality.arc42.org/tag-maintainable/> |

## Reliable

"Capability of a product to perform specified functions under specified conditions for a specified period of time without interruptions and failures.  
Note: Wear does not occur in software. Limitations in reliability are due to results from faults in requirements, design and implementation, or from contextual changes."
[ISO-25010:2023](https://quality.arc42.org/references/#iso-25010-2023)

### Typical Acceptance Criteria

- Time or time interval when the system shall be available
- Availability percentage
- Time to detect a fault
- Time to repair a fault
- Time or time interval in which the system may operate in degraded mode
- Proportion (e.g. 99%) or rate (e.g. up to 42 per second) of a certain class or types of faults that the system either prevents or handles without failing  
  Source: [Bass et al., 2021, p. 75](https://quality.arc42.org/references/#bass2021software)

### What Stakeholders mean by _reliable_

| Stakeholder   | (potential) Expectation for reliable                                                   |
| ------------- | -------------------------------------------------------------------------------------- |
| User          | \* available when need it                                                              |
|               | \* produces expected results                                                           |
|               | \* offers expected functionality                                                       |
|               | \* user documentation is reliable                                                      |
| Product-Owner | \* reliably add new functions and features                                             |
|               | \* reliable estimates concerning effort for changes                                    |
|               | \* reliable at runtime, available when users need it                                   |
| Management    | \* cost and effort of development, operations and support are reliably predictable     |
|               | \* reliable with respect to operations, especially security and interoperability       |
| Developer     | \* reliably add new features or functions to the system without unwanted side-effects. |
|               | \* reliably predict the effects of changes to the system                               |
| Tester        | test results are reliable (as in consistent or repeatable)                             |
| Admin         | \* reliably start, configure and monitor the system                                    |
|               | \* reliable release and update processes                                               |
| Domain-Expert | -                                                                                      |
| Others        | \* technical documentation is reliable (current and correct)                           |

### Qualities tagged with #reliable

- [Accuracy](https://quality.arc42.org/qualities/accuracy): The degree of conformity of a measured or calculated value to the true value, typically based on a global reference system ([NIST Glossary](https://csrc.nist.gov/glossary/term/accuracy_absolute))
- [Analysability](https://quality.arc42.org/qualities/analysability): Capability of a product to be effectively and efficiently assessed regarding the impact of an intended change to one or more of its parts, to diagnose it for deficiencies or causes of failures, or to identify parts to be modified. Implementation can include providing mechanisms for the product to analyse its own faults and provide reports prior to a failure or other event. (from [ISO-25010:2023](https://quality.arc42.org/references/#iso-25010-2023))
- [Atomicity](https://quality.arc42.org/qualities/atomicity)
- [Availability](https://quality.arc42.org/qualities/availability)
- [Backward compatibility](https://quality.arc42.org/qualities/backward-compatibility)
- [Bias Mitigation](https://quality.arc42.org/qualities/bias-mitigation)
- [Capacity](https://quality.arc42.org/qualities/capacity)
- [Certifiability](https://quality.arc42.org/qualities/certifiability)
- [Clarity](https://quality.arc42.org/qualities/clarity)
- [Compatibility](https://quality.arc42.org/qualities/compatibility)
- [Completeness](https://quality.arc42.org/qualities/completeness)
- [Compliance](https://quality.arc42.org/qualities/compliance)
- [Correctness](https://quality.arc42.org/qualities/correctness)
- [Credibility](https://quality.arc42.org/qualities/credibility)
- [Data Integrity](https://quality.arc42.org/qualities/data-integrity)
- [Data Quality](https://quality.arc42.org/qualities/data-quality)
- [Dependability](https://quality.arc42.org/qualities/dependability)
- [Determinism](https://quality.arc42.org/qualities/determinism)
- [Diagnosability](https://quality.arc42.org/qualities/diagnosability)
- [Durability](https://quality.arc42.org/qualities/durability)
- [Fail safe](https://quality.arc42.org/qualities/fail-safe)
- [Failure Transparency](https://quality.arc42.org/qualities/failure-transparency)
- [Fairness](https://quality.arc42.org/qualities/fairness)
- [Fault isolation](https://quality.arc42.org/qualities/fault-isolation)
- [Fault tolerance](https://quality.arc42.org/qualities/fault-tolerance)
- [Faultlessness](https://quality.arc42.org/qualities/faultlessness)
- [Functional Appropriateness](https://quality.arc42.org/qualities/functional-appropriateness)
- [Functional completeness](https://quality.arc42.org/qualities/functional-completeness)
- [Functional suitability](https://quality.arc42.org/qualities/functional-suitability)
- [Functionality](https://quality.arc42.org/qualities/functionality)
- [Graceful degradation](https://quality.arc42.org/qualities/graceful-degradation)
- [Hazard warning](https://quality.arc42.org/qualities/hazard-warning)
- [Immunity](https://quality.arc42.org/qualities/immunity)
- [Jitter](https://quality.arc42.org/qualities/jitter)
- [Longevity](https://quality.arc42.org/qualities/longevity)
- [Operational constraint](https://quality.arc42.org/qualities/operational-constraint)
- [Patient Safety](https://quality.arc42.org/qualities/patient-safety)
- [Precision](https://quality.arc42.org/qualities/precision)
- [Predictability](https://quality.arc42.org/qualities/predictability)
- [Provability](https://quality.arc42.org/qualities/provability)
- [Recoverability](https://quality.arc42.org/qualities/recoverability)
- [Redundancy](https://quality.arc42.org/qualities/redundancy)
- [Reliability](https://quality.arc42.org/qualities/reliability)
- [Resilience](https://quality.arc42.org/qualities/resilience)
- [Risk identification](https://quality.arc42.org/qualities/risk-identification)
- [Robustness](https://quality.arc42.org/qualities/robustness)
- [Safe integration](https://quality.arc42.org/qualities/safe-integration)
- [Safety](https://quality.arc42.org/qualities/safety)
- [Security](https://quality.arc42.org/qualities/security)
- [Stability](https://quality.arc42.org/qualities/stability)
- [Suitability](https://quality.arc42.org/qualities/suitability)
- [Sustainability](https://quality.arc42.org/qualities/sustainability)
- [Timeliness](https://quality.arc42.org/qualities/timeliness)
- [Traceability](https://quality.arc42.org/qualities/traceability)
- [Transactionality](https://quality.arc42.org/qualities/transactionality)
- [Transparency](https://quality.arc42.org/qualities/transparency)
- [Verifiability](https://quality.arc42.org/qualities/verifiability)
- [Vulnerability](https://quality.arc42.org/qualities/vulnerability)

## Flexible

Easy to:

- adapt to changed contexts of use and environments
- run in new or modified execution environments (hardware, OS, cloud provider, region)
- handle changed workload profiles
- configure or tailor behavior without invasive redesign

###

### Definition

Capability of a product to be adapted to changes in its requirements, contexts of use, or system environment.  
Note: Flexibility to context of use should consider two distinguished aspects, i.e. technical and non-technical. The technical aspect is related with the execution environment of products, such as software, hardware and communication facility; and the non-technical aspect is related with the social environment, such as user and task, and the physical environment, such as climate and nature.  
++[ISO-25010:2023](https://quality.arc42.org/references/#iso-25010-2023)++

### Typical Acceptance Criteria

Flexible, as we saw above, means “_adaptable to change_”.  
For Q42, _#flexible_ focuses on adaptation to external context and runtime/operational variability. Developer-focused changeability concerns (e.g. analyzability, modifiability, testability) belong primarily to ++[#maintainable](https://quality.arc42.org/tag-maintainable)++.  
When defining what exactly _#flexible_ shall mean for a specific system and stakeholders, we should consider:

- Which external changes are expected (infrastructure, workload, integrations, locales, user/task context)?
- At which point adaptation is needed (installation, deployment, startup, runtime)?
- Which adaptations must be configuration-driven vs requiring rollout/redeployment?  
  Typical acceptance criteria might include:
- Time/effort to deploy to a new environment (e.g. cloud provider/region/OS)
- Time/effort to reconfigure behavior for a new context of use
- Performance/SLA impact while scaling up or down
- Number of integration endpoints/protocol variants supported without redesign
- Side-effects on reliability, security, usability, and operability

### Scenario Response Measures from [Bass et al.]

Cost in terms of

- Number, size, complexity of affected artifacts
- Effort
- Elapsed time
- Money
- Extent to which this modification affects other quality attributes
- New defects introduced  
  ++[Bass et al., 2021](https://quality.arc42.org/references/#bass2021software)++

### _flexible_ for Stakeholders

| Stakeholder   | (potential) Expectation for flexible                                                                                         |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| User          | behavior can be tailored to usage context, language, and channel                                                             |
| Product-Owner | product can support adjacent use cases/markets without re-architecture                                                       |
| Management    | low business risk and cost when market/context shifts require adaptation                                                     |
| Developer     | extension points and configuration options support context adaptation (internal maintainability is covered by #maintainable) |
| Tester        | adaptations can be validated across supported environment/context variants                                                   |
| Admin         | easy environment migration, scaling, and runtime configuration                                                               |
| Domain-Expert | business rules can be parameterized for variant contexts                                                                     |
| Others        | partner/integration interfaces can evolve with controlled impact                                                             |

### Qualities tagged with #flexible

- ++[Adaptability](https://quality.arc42.org/qualities/adaptability)++
- ++[Agility](https://quality.arc42.org/qualities/agility)++
- ++[Changeability](https://quality.arc42.org/qualities/changeability)++
- ++[Co-existence](https://quality.arc42.org/qualities/co-existence)++
- ++[Composability](https://quality.arc42.org/qualities/composability)++
- ++[Configurability](https://quality.arc42.org/qualities/configurability)++
- ++[Customizability](https://quality.arc42.org/qualities/customizability)++
- ++[Distributability](https://quality.arc42.org/qualities/distributability)++
- ++[Elasticity](https://quality.arc42.org/qualities/elasticity)++
- ++[Evolvability](https://quality.arc42.org/qualities/evolvability)++
- ++[Extensibility](https://quality.arc42.org/qualities/extensibility)++
- ++[Flexibility](https://quality.arc42.org/qualities/flexibility)++
- ++[Independence](https://quality.arc42.org/qualities/independence)++
- ++[Installability](https://quality.arc42.org/qualities/installability)++
- ++[Integrability](https://quality.arc42.org/qualities/integrability)++
- ++[Interchangeability](https://quality.arc42.org/qualities/interchangeability)++
- ++[Internationalization](https://quality.arc42.org/qualities/internationalization)++
- ++[Localizability](https://quality.arc42.org/qualities/localizability)++
- ++[Longevity](https://quality.arc42.org/qualities/longevity)++
- ++[Modifiability](https://quality.arc42.org/qualities/modifiability)++
- ++[Personalization](https://quality.arc42.org/qualities/personalization)++
- ++[Portability](https://quality.arc42.org/qualities/portability)++
- ++[Replaceability](https://quality.arc42.org/qualities/replaceability)++
- ++[Reusability](https://quality.arc42.org/qualities/reusability)++
- ++[Scalability](https://quality.arc42.org/qualities/scalability)++
- ++[Self-containedness](https://quality.arc42.org/qualities/self-containedness)++
- ++[Themability](https://quality.arc42.org/qualities/themability)++
- ++[Versatility](https://quality.arc42.org/qualities/versatility)++

##

### Requirements tagged with #flexible

- ++[Adding a new entity type within 5 days and ≤ 3 modules](https://quality.arc42.org/requirements/adding-entity-type-within-5-days)++
- ++[Compatible with 5 different battery providers](https://quality.arc42.org/requirements/compatible-with-5-battery-providers)++
- ++[Configurable UI theme](https://quality.arc42.org/requirements/configurable-ui-theme)++
- ++[Core functions can be used on multiple OSs](https://quality.arc42.org/requirements/core-functions-on-mac-win-linux)++
- ++[CRM System Data Synchronization](https://quality.arc42.org/requirements/crm-data-synchronization)++
- ++[Easily change cloud provider](https://quality.arc42.org/requirements/change-cloud-provider)++
- ++[Efficient change of business rules](https://quality.arc42.org/requirements/luggage-routing)++
- ++[Independent enhancement of subsystem](https://quality.arc42.org/requirements/independent-enhancement-of-subsystem)++
- ++[Independent replacement of subsystem](https://quality.arc42.org/requirements/independent-replacement-of-subsystem)++
- ++[Localizable to several languages](https://quality.arc42.org/requirements/localizable-to-n-languages)++
- ++[Modular System for Data Analysis](https://quality.arc42.org/requirements/modular-system-for-data-analysis)++
- ++[On-prem installation ready in 30 minutes](https://quality.arc42.org/requirements/on-prem-installation-ready-in-30-min)++
- ++[Portable Business Data Checker](https://quality.arc42.org/requirements/portable-business-data-checker)++
- ++[Efficient update of annual accounting report](https://quality.arc42.org/requirements/annual-tax-update)++
- ++[Shared library adoption by product teams](https://quality.arc42.org/requirements/shared-library-adoption-by-product-teams)++
- ++[User Interface can be used in Current Browsers](https://quality.arc42.org/requirements/user-interface-works-with-current-browsers)++

### Approaches tagged with #flexible

- ++[Asynchronous Messaging](https://quality.arc42.org/approaches/asynchronous-messaging)++
- ++[CQRS](https://quality.arc42.org/approaches/cqrs)++
- ++[Feature Toggles](https://quality.arc42.org/approaches/feature-toggles)++
- ++[Plugin Architecture](https://quality.arc42.org/approaches/plugin-architecture)++

## Efficient

- Resource-efficient, fast, low-footprint, low latency.
- Energy-, storage- and network efficient, having adequate capacity
- Development-efficient, being easy to change (although that aspect may better be covered by ++[#flexible](https://quality.arc42.org/tag-flexible)++)
- Time-to-market, how efficient new features can _go live_

### Definitions

capable of producing desired results with little or no waste (as of time or materials)  
++[Merriam-Webster](https://www.merriam-webster.com/dictionary/efficient)++

The amount of computing resources and code required by a program to perform a function.  
++[McCall-1978](https://quality.arc42.org/references/#mccall)++

### Effective vs Efficient

The words effective and efficient both mean “capable of producing a result,” but there is an important difference. Effective means “producing a result that is wanted”. Efficient means “capable of producing desired results without wasting materials, time, or energy”. The difference is that when something is effective it produces a result even if it takes some unnecessary resources to do so. When something is efficient, not only does it produce a result, but it does so in a quick or simple way using as little material, time, effort, or energy as possible. The following example sentences show how the two words are used.

- The 200-page instruction manual was effective (_=successful_) in teaching the teen to repair the car himself, but it would have been more efficient (_=faster and easier_) for someone to show him.
- His disorganized method of cleaning the house was effective but it was not efficient; in the end, the house was clean, but it took much longer than it should have.  
  The word _effective_ puts more attention on the actual ability to produce a desired result. The word _efficient_ puts more attention on the lack of waste in producing that result.  
  ++[Britannica Dictionary](https://www.britannica.com/dictionary/eb/qa/How-to-Use-Effective-and-Efficient)++

### Typical Acceptance Criteria

Efficient, as we saw above, can mean several different things:

- efficient at runtime, like defined by specific time behavior, resource consumption (e.g. energy, memory, processes, threads, network) or capacity (throughput, volume processed)
- efficient to change or modify something within the system or its infrastructure
- efficient concerning energy or CO2 consumption
- efficient development processes, like short time-to-market  
  **Scenario Response Measures from [Bass et al.]**
- The (maximum, medium, mean median) time the response takes ([++[latency](https://quality.arc42.org/qualities/latency)++])
- The number or percentage of satisfied requests over some time interval (throughput) or set of events received
- The number or percentage of requests that go unsatisfied
- The variation in response time (++[jitter](https://quality.arc42.org/qualities/jitter)++)
- Usage level of a computing resource  
  ++[Bass et al., 2021](https://quality.arc42.org/references/#bass2021software)++

### Qualities tagged with #efficient

- ++[Affordability](https://quality.arc42.org/qualities/affordability)++
- ++[Capacity](https://quality.arc42.org/qualities/capacity)++
- ++[Carbon Emission Efficiency](https://quality.arc42.org/qualities/carbon-emission-efficiency)++
- ++[Code Complexity](https://quality.arc42.org/qualities/code-complexity)++
- ++[Code Readability](https://quality.arc42.org/qualities/code-readability)++
- ++[Coherence](https://quality.arc42.org/qualities/coherence)++
- ++[Cohesion](https://quality.arc42.org/qualities/cohesion)++
- ++[Compliance](https://quality.arc42.org/qualities/compliance)++
- ++[Conciseness](https://quality.arc42.org/qualities/conciseness)++
- ++[Consistency](https://quality.arc42.org/qualities/consistency)++
- ++[Cost](https://quality.arc42.org/qualities/cost)++
- ++[Cycle time](https://quality.arc42.org/qualities/cycle-time)++
- ++[Determinism](https://quality.arc42.org/qualities/determinism)++
- ++[Distributability](https://quality.arc42.org/qualities/distributability)++
- ++[Effectiveness](https://quality.arc42.org/qualities/effectiveness)++
- ++[Efficiency](https://quality.arc42.org/qualities/efficiency)++
- ++[Energy Efficiency](https://quality.arc42.org/qualities/energy-efficiency)++
- ++[Energy Proportionality](https://quality.arc42.org/qualities/energy-proportionality)++
- ++[Jitter](https://quality.arc42.org/qualities/jitter)++
- ++[Latency](https://quality.arc42.org/qualities/latency)++
- ++[Loose Coupling](https://quality.arc42.org/qualities/loose-coupling)++
- ++[Memory usage](https://quality.arc42.org/qualities/memory-usage)++
- ++[Performance](https://quality.arc42.org/qualities/performance)++
- ++[Profitability](https://quality.arc42.org/qualities/profitability)++
- ++[Releasability](https://quality.arc42.org/qualities/releasability)++
- ++[Resource efficiency](https://quality.arc42.org/qualities/resource-efficiency)++
- ++[Resource utilization](https://quality.arc42.org/qualities/resource-utilization)++
- ++[Response Time](https://quality.arc42.org/qualities/response-time)++
- ++[Responsiveness](https://quality.arc42.org/qualities/responsiveness)++
- ++[Shutdown Time](https://quality.arc42.org/qualities/shutdown-time)++
- ++[Simplicity](https://quality.arc42.org/qualities/simplicity)++
- ++[Speed](https://quality.arc42.org/qualities/speed)++
- ++[Startup Time](https://quality.arc42.org/qualities/startup-time)++
- ++[Sustainability](https://quality.arc42.org/qualities/sustainability)++
- ++[Throughput](https://quality.arc42.org/qualities/throughput)++
- ++[Time behaviour](https://quality.arc42.org/qualities/time-behaviour)++
- ++[Time to Market](https://quality.arc42.org/qualities/time-to-market)++

###

### Requirements tagged with #efficient

- ++[Add new product under 60 minutes](https://quality.arc42.org/requirements/add-new-product)++
- ++[Affordable CRM (customer relationship management)](https://quality.arc42.org/requirements/affordable-crm)++
- ++[Budget constrained library update](https://quality.arc42.org/requirements/budget-constraint-library-update)++
- ++[Save at least 20% of carbon emissions with every new version](https://quality.arc42.org/requirements/carbon-efficiency-save)++
- ++[Consistent keyboard shortcuts](https://quality.arc42.org/requirements/consistent-keyboard-shortcuts)++
- ++[Data Throughput for Visual Test System](https://quality.arc42.org/requirements/data-throughput-for-visual-test-system)++
- ++[Efficient change of business rules](https://quality.arc42.org/requirements/luggage-routing)++
- ++[Efficient generation of test data](https://quality.arc42.org/requirements/efficient-generation-of-test-data)++
- ++[Fast and accurate sensor](https://quality.arc42.org/requirements/fast-accurate-sensor)++
- ++[Efficient save function](https://quality.arc42.org/requirements/efficient-save-function)++
- ++[Fast creation of sales report](https://quality.arc42.org/requirements/fast-creation-of-sales-report)++
- ++[Fast rollout of changes](https://quality.arc42.org/requirements/fast-rollout-of-changes)++
- ++[Fast shutdown time (less than 10 sec)](https://quality.arc42.org/requirements/fast-shutdown-time)++
- ++[Fast startup time (less than 90 sec)](https://quality.arc42.org/requirements/fast-startup-time)++
- ++[Independent enhancement of subsystem](https://quality.arc42.org/requirements/independent-enhancement-of-subsystem)++
- ++[Independent replacement of subsystem](https://quality.arc42.org/requirements/independent-replacement-of-subsystem)++
- ++[Low impact diagnosis](https://quality.arc42.org/requirements/low-impact-diagnosis)++
- ++[Monolith loose coupling: change blast radius](https://quality.arc42.org/requirements/monolith-loose-coupling-change-blast-radius)++
- ++[Service loose coupling: change blast radius](https://quality.arc42.org/requirements/service-loose-coupling-change-blast-radius)++
- ++[Modular System for Data Analysis](https://quality.arc42.org/requirements/modular-system-for-data-analysis)++
- ++[Near instant search results](https://quality.arc42.org/requirements/near-instant-search-results)++
- ++[Maintainable checking strategies](https://quality.arc42.org/requirements/maintainable-checking-strategy)++
- ++[Parallel Data Modification](https://quality.arc42.org/requirements/parallel-data-modification)++
- ++[Low-overhead query execution measurement](https://quality.arc42.org/requirements/query-execution-management)++
- ++[Quickly locate bugs](https://quality.arc42.org/requirements/quickly-locate-bugs)++
- ++[Reduce energy consumption with every new version](https://quality.arc42.org/requirements/reduce-energy-consumption-with-new-version)++
- ++[Efficient update of annual accounting report](https://quality.arc42.org/requirements/annual-tax-update)++
- ++[Respond to 15000 requests per workday](https://quality.arc42.org/requirements/respond-to-15000-requests-per-workday)++
- ++[Response time for image rendering](https://quality.arc42.org/requirements/response-time-for-image-rendering)++
- ++[Restricted Memory](https://quality.arc42.org/requirements/restricted-memory)++
- ++[Scale up in 2 Minutes](https://quality.arc42.org/requirements/scale-up-in-2-minutes)++
- ++[Capacity to process 1000 sensor inputs per minute](https://quality.arc42.org/requirements/capacity-to-process-sensor-inputs)++

###

### Approaches tagged with #efficient

- ++[Asynchronous Messaging](https://quality.arc42.org/approaches/asynchronous-messaging)++
- ++[Caching](https://quality.arc42.org/approaches/caching)++
- ++[Content Delivery Network (CDN)](https://quality.arc42.org/approaches/content-delivery-network)++
- ++[CQRS](https://quality.arc42.org/approaches/cqrs)++
- ++[Database Sharding](https://quality.arc42.org/approaches/database-sharding)++

## Usable

The main idea of _usability_ is that a system shall be designed with (generalized) users’ psychology and physiology in mind, to make that system:

- more efficient to use, so it takes less time to accomplish particular tasks
- easier to learn
- more satisfying to use

### Definitions

Capability of a product to be interacted with by specified users to exchange information between a user and a system via the user interface to complete the intended task. ++[ISO-25010:2023](https://quality.arc42.org/references/#iso-25010-2023)++

The capacity of a system to provide a condition for its users to perform the tasks safely, effectively, and efficiently while enjoying the experience. ++[Wikipedia](https://en.wikipedia.org/wiki/Usability)++

Enable users to perform their tasks safely, effectively and efficiently while enjoying the experience.  
++[Volere Version 2.0](https://quality.arc42.org/references/#volere)++

### Typical Acceptance Criteria

**Scenario Response Measures from [Bass et al.]**  
The system should:

- provide the user with the features needed
- anticipate the user’s needs
- provide appropriate feedback to the user  
  The system’s response might be measured in one or more of the following:
- task time
- number of errors
- learning time
- ratio of learning time to task time
- number of tasks accomplished
- user satisfaction
- gain of user knowledge
- ratio of successful operations to total operations
- amount of time or data lost when an error occurs  
  ++[Bass et al., 2021](https://quality.arc42.org/references/#bass2021software)++

### What Stakeholders mean by _usable_

| Stakeholder | (potential) Expectation for usable         |
| ----------- | ------------------------------------------ |
| User        | see the criteria above. More specifically: |

- functional-completeness
- accessibility
- correctness
- visual and behavioural consistency
- understandability
- ease-of-use
- functional-suitability
- learnability
- nice user-experience
  (maybe even more) |
  | Product-Owner | - |
  | Management | - |
  | Developer | \* understandable source-code and dependencies
- an appropriate technology-stack
- no (or at least predictable) side-effects when changing the system |
  | Tester | \* testability
- predictable test behaviour |
  | Admin | \* easy to deploy and install,
- installability
- deployability |
  | Domain-Expert | - |
  | Others | - |

### Qualities tagged with #usable

- ++[Accessibility](https://quality.arc42.org/qualities/accessibility)++
- ++[Accuracy](https://quality.arc42.org/qualities/accuracy)++
- ++[Adaptability](https://quality.arc42.org/qualities/adaptability)++
- ++[Affordability](https://quality.arc42.org/qualities/affordability)++
- ++[Anticipated Workplace Environment](https://quality.arc42.org/qualities/anticipated-workplace-environment)++
- ++[Appearance](https://quality.arc42.org/qualities/appearance)++
- ++[Appropriateness recognizability](https://quality.arc42.org/qualities/appropriateness-recognizability)++
- ++[Attractiveness](https://quality.arc42.org/qualities/attractiveness)++
- ++[Availability](https://quality.arc42.org/qualities/availability)++
- ++[Backward compatibility](https://quality.arc42.org/qualities/backward-compatibility)++
- ++[Clarity](https://quality.arc42.org/qualities/clarity)++
- ++[Code Complexity](https://quality.arc42.org/qualities/code-complexity)++
- ++[Code Readability](https://quality.arc42.org/qualities/code-readability)++
- ++[Coherence](https://quality.arc42.org/qualities/coherence)++
- ++[Communicability](https://quality.arc42.org/qualities/communicability)++
- ++[Compatibility](https://quality.arc42.org/qualities/compatibility)++
- ++[Compliance](https://quality.arc42.org/qualities/compliance)++
- ++[Conciseness](https://quality.arc42.org/qualities/conciseness)++
- ++[Configurability](https://quality.arc42.org/qualities/configurability)++
- ++[Consent Management](https://quality.arc42.org/qualities/consent-management)++
- ++[Consistency](https://quality.arc42.org/qualities/consistency)++
- ++[Controllability](https://quality.arc42.org/qualities/controllability)++
- ++[Convenience](https://quality.arc42.org/qualities/convenience)++
- ++[Correctness](https://quality.arc42.org/qualities/correctness)++
- ++[Customizability](https://quality.arc42.org/qualities/customizability)++
- ++[Data Quality](https://quality.arc42.org/qualities/data-quality)++
- ++[Discoverability](https://quality.arc42.org/qualities/discoverability)++
- ++[Ease of Use](https://quality.arc42.org/qualities/ease-of-use)++
- ++[Fault tolerance](https://quality.arc42.org/qualities/fault-tolerance)++
- ++[Faultlessness](https://quality.arc42.org/qualities/faultlessness)++
- ++[Features](https://quality.arc42.org/qualities/features)++
- ++[Functional Appropriateness](https://quality.arc42.org/qualities/functional-appropriateness)++
- ++[Functional completeness](https://quality.arc42.org/qualities/functional-completeness)++
- ++[Functional suitability](https://quality.arc42.org/qualities/functional-suitability)++
- ++[Functionality](https://quality.arc42.org/qualities/functionality)++
- ++[Graceful degradation](https://quality.arc42.org/qualities/graceful-degradation)++
- ++[Inclusivity](https://quality.arc42.org/qualities/inclusivity)++
- ++[Interaction capability](https://quality.arc42.org/qualities/interaction-capability)++
- ++[Internationalization](https://quality.arc42.org/qualities/internationalization)++
- ++[Interoperability](https://quality.arc42.org/qualities/interoperability)++
- ++[Intuitiveness](https://quality.arc42.org/qualities/intuitiveness)++
- ++[Latency](https://quality.arc42.org/qualities/latency)++
- ++[Learnability](https://quality.arc42.org/qualities/learnability)++
- ++[Legal Requirements](https://quality.arc42.org/qualities/legal-requirements)++
- ++[Legibility](https://quality.arc42.org/qualities/legibility)++
- ++[Localizability](https://quality.arc42.org/qualities/localizability)++
- ++[Operability](https://quality.arc42.org/qualities/operability)++
- ++[Precision](https://quality.arc42.org/qualities/precision)++
- ++[Readability](https://quality.arc42.org/qualities/readability)++
- ++[Recoverability](https://quality.arc42.org/qualities/recoverability)++
- ++[Reproducibility](https://quality.arc42.org/qualities/reproducibility)++
- ++[Responsiveness](https://quality.arc42.org/qualities/responsiveness)++
- ++[Self-descriptiveness](https://quality.arc42.org/qualities/self-descriptiveness)++
- ++[Simplicity](https://quality.arc42.org/qualities/simplicity)++
- ++[Suitability](https://quality.arc42.org/qualities/suitability)++
- ++[Understandability](https://quality.arc42.org/qualities/understandability)++
- ++[Usability](https://quality.arc42.org/qualities/usability)++
- ++[User assistance](https://quality.arc42.org/qualities/user-assistance)++
- ++[User engagement](https://quality.arc42.org/qualities/user-engagement)++
- ++[User error protection](https://quality.arc42.org/qualities/user-error-protection)++
- ++[User experience](https://quality.arc42.org/qualities/user-experience)++
- ++[User interface aesthetics](https://quality.arc42.org/qualities/user-interface-aesthetics)++

### Requirements tagged with #usable

- ++[Access Control via SSO](https://quality.arc42.org/requirements/access-control-via-sso)++
- ++[Access find function in three seconds](https://quality.arc42.org/requirements/access-find-function-quickly)++
- ++[Accessible User Interface](https://quality.arc42.org/requirements/accessible-user-interface)++
- ++[Accurate estimate of insurance contract rate](https://quality.arc42.org/requirements/accurate-estimate-of-insurance-rate)++
- ++[Vehicle's position validity influences accuracy](https://quality.arc42.org/requirements/accurate-vehicle-position-gps)++
- ++[Appearance of mobile UI](https://quality.arc42.org/requirements/appearance-requirements)++
- ++[Attractive Appearance of Website](https://quality.arc42.org/requirements/attractive-quality-knowledge-base)++
- ++[Clarity in technical documentation](https://quality.arc42.org/requirements/clarity-in-technical-documentation)++
- ++[Compliance with WCAG accessibility guidelines](https://quality.arc42.org/requirements/compliance-to-wcag)++
- ++[Compliance with UI styleguide](https://quality.arc42.org/requirements/compliance-with-ui-styleguide)++
- ++[Configurable UI theme](https://quality.arc42.org/requirements/configurable-ui-theme)++
- ++[Consistent keyboard shortcuts](https://quality.arc42.org/requirements/consistent-keyboard-shortcuts)++
- ++[Convenient online banking](https://quality.arc42.org/requirements/convenient-online-banking)++
- ++[Core functions can be used on multiple OSs](https://quality.arc42.org/requirements/core-functions-on-mac-win-linux)++
- ++[Cultural Sensitivity in Content](https://quality.arc42.org/requirements/cultural-sensitivity-in-content)++
- ++[Data Throughput for Visual Test System](https://quality.arc42.org/requirements/data-throughput-for-visual-test-system)++
- ++[Detect inconsistent user input](https://quality.arc42.org/requirements/detect-inconsistent-user-input)++
- ++[Display Data Based on Context](https://quality.arc42.org/requirements/display-data-based-on-context)++
- ++[Understandable acceptance test cases](https://quality.arc42.org/requirements/understandable-acceptance-tests)++
- ++[Easy UI](https://quality.arc42.org/requirements/easy-ui)++
- ++[Expressive error messages](https://quality.arc42.org/requirements/expressive-error-messages)++
- ++[First-time onboarding without errors](https://quality.arc42.org/requirements/first-time-onboarding-without-errors)++
- ++[Inclusive User Testing](https://quality.arc42.org/requirements/inclusive-user-testing)++
- ++[Interruptable backend process](https://quality.arc42.org/requirements/interruptable-backend-process)++
- ++[Keep data on error](https://quality.arc42.org/requirements/keep-data-on-error)++
- ++[New users learn to find articles on their own](https://quality.arc42.org/requirements/learnability-find-article)++
- ++[Restored to fully functional state 12h after complete failure](https://quality.arc42.org/requirements/mttr-12h)++
- ++[Multilinguality Support](https://quality.arc42.org/requirements/multilinguality-support)++
- ++[Near instant search results](https://quality.arc42.org/requirements/near-instant-search-results)++
- ++[New user completes core tasks without prior training](https://quality.arc42.org/requirements/new-user-completes-core-tasks-without-training)++
- ++[Parallel Data Modification](https://quality.arc42.org/requirements/parallel-data-modification)++
- ++[Recognize Assistive Technologies](https://quality.arc42.org/requirements/recognize-assistive-technology)++
- ++[Available 7x24 with 99% uptime](https://quality.arc42.org/requirements/available-7-24-99)++
- ++[Restore Filter after Log In](https://quality.arc42.org/requirements/restore-filter-after-log-in)++
- ++[Search and graph text filter available on Q42](https://quality.arc42.org/requirements/search-and-graph-text-filter-available-on-q42)++
- ++[Unavailable for max 2 minutes](https://quality.arc42.org/requirements/unavailability-max-2-minutes)++
- ++[Usable Despite Color Blindness](https://quality.arc42.org/requirements/usable-despite-color-blindness)++
- ++[Usable on Factory Floor](https://quality.arc42.org/requirements/usable-on-factory-floor)++
- ++[User Interface can be used in Current Browsers](https://quality.arc42.org/requirements/user-interface-works-with-current-browsers)++
- ++[Usable With Gloves](https://quality.arc42.org/requirements/usable-with-gloves)++
- ++[User tries to achieve primary function](https://quality.arc42.org/requirements/user-tries-primary-function)++

### Approaches tagged with #usable

- ++[Progressive Disclosure](https://quality.arc42.org/approaches/progressive-disclosure)++
- ++[Responsive Design](https://quality.arc42.org/approaches/responsive-design)++

### Standards related to #usable

**[EN 301 549 - Accessibility requirements for ICT products and services](https://quality.arc42.org/standards/en-301-549)**  
 #accessibility, #usability

**[ISO/IEC 25010 - Systems and Software Quality](https://quality.arc42.org/standards/iso-25010)**  
 #general, #usability

**[ISO/IEC 25022 - Measurement of quality in use](https://quality.arc42.org/standards/iso-25022)**  
 #data, #usability

**[ISO/IEC/IEEE 26514 - Design and Development of Information for Users](https://quality.arc42.org/standards/iso-26514)**  
 #documentation, #usability, #accessibility

**[WCAG 2.2 - Web Content Accessibility Guidelines](https://quality.arc42.org/standards/wcag-2-2)**  
 #accessibility, #usability

## Secure

- preventing unauthorized access to assets such as computers, networks, and data.
- maintaining confidentiality, integrity and availability of (sensitive) information

### Definition

Capability of a product to protect information and data so that persons or other products have the degree of data access appropriate to their types and levels of authorization, and to defend against attack patterns by malicious actors.  
++[ISO-25010:2023](https://quality.arc42.org/references/#iso-25010-2023)++

### Typical Acceptance Criteria

**Scenario Response Measures from [Bass et al.]**

- How much of a resource is compromised or ensured?
- Accuracy of attack detection
- How much time passes before an attack is detected?
- How many attacks are resisted?
- How long does it take to recover from a successful attack?
- How much data is vulnerable to a particular attack?  
  ++[Bass et al., 2021](https://quality.arc42.org/references/#bass2021software)++

### What Stakeholders mean by _secure_

| Stakeholder                                                    | (potential) Expectation for secure                                            |
| -------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| User                                                           | \* my personal data is never compromised or leaked to (hostile) third parties |
| \* a good compromise between privacy and usability is achieved |
| Management                                                     | \* lowest possible risk of data breaches                                      |

- full compliance with GDPR or similar data protection and privacy regulations
- full adherence to all licenses, of e.g. commercial or open-source tools, libraries or frameworks
- appropriate network security measures taken
- regular backups, tested and automated
- minimal attack vectors |
  | Developer | \* despite corporate security measures, public sources (like Stack Overflow, GitHub and common search engines) are accessible
  security strategies like VPNs or MFA are easy to use
- automated and tested backup for everything
- all important documents and files are version-controlled |
  | Tester | - |
  | Admin | \* smallest possible attack surface
- restrictive firewall rules
- minimal access rights for all stakeholders (least privilege)
- intrusion detection in place
- automated malware scans for all incoming data and files
- |
  | Domain-Expert | - |
  | Others | Security auditor, Data protection officer, government or corporate security departments, attackers |

### Qualities tagged with #secure

- [++ Access Control++](https://quality.arc42.org/qualities/access-control)
- [++ Accountability++](https://quality.arc42.org/qualities/accountability)
- [++ Authenticity++](https://quality.arc42.org/qualities/authenticity)
- [++ Compliance++](https://quality.arc42.org/qualities/compliance)
- [++ Confidentiality++](https://quality.arc42.org/qualities/confidentiality)
- [++ Consent Management++](https://quality.arc42.org/qualities/consent-management)
- [++ Cyber Security++](https://quality.arc42.org/qualities/cyber-security)
- [++ Data Integrity++](https://quality.arc42.org/qualities/data-integrity)
- [++ Data Localization++](https://quality.arc42.org/qualities/data-localization)
- [++ Data Minimization++](https://quality.arc42.org/qualities/data-minimization)
- [++ Data Protection++](https://quality.arc42.org/qualities/data-protection)
- [++ Data Sovereignty++](https://quality.arc42.org/qualities/data-sovereignty)
- [++ Faultlessness++](https://quality.arc42.org/qualities/faultlessness)
- [++ Governability++](https://quality.arc42.org/qualities/governability)
- [++ Immunity++](https://quality.arc42.org/qualities/immunity)
- [++ Injection Resistance++](https://quality.arc42.org/qualities/injection-resistance)
- [++ Integrity++](https://quality.arc42.org/qualities/integrity)
- [++ Intrusion Detection++](https://quality.arc42.org/qualities/intrusion-detection)
- [++ Intrusion Prevention++](https://quality.arc42.org/qualities/intrusion-prevention)
- [++ Non-repudiation++](https://quality.arc42.org/qualities/non-repudiation)
- [++ Patient Safety++](https://quality.arc42.org/qualities/patient-safety)
- [++ Privacy++](https://quality.arc42.org/qualities/privacy)
- [++ Resilience++](https://quality.arc42.org/qualities/resilience)
- [++ Resistance++](https://quality.arc42.org/qualities/resistance)
- [++ Safety++](https://quality.arc42.org/qualities/safety)
- [++ Securability++](https://quality.arc42.org/qualities/securability)
- [++ Security++](https://quality.arc42.org/qualities/security)
- [++ Vulnerability++](https://quality.arc42.org/qualities/vulnerability)

### Requirements tagged with #secure

- [++ Access control is enforced++](https://quality.arc42.org/requirements/access-control-is-enforced)
- [++ Access Control via SSO++](https://quality.arc42.org/requirements/access-control-via-sso)
- [++ Detailed audit log++](https://quality.arc42.org/requirements/detailed-audit-log)
- [++ Authenticity of a digital document++](https://quality.arc42.org/requirements/authenticity-of-digital-document)
- [++ Data Localization for Citizen Records++](https://quality.arc42.org/requirements/data-localization-for-citizen-records)
- [++ Automated Personal Data Lifecycle Protection++](https://quality.arc42.org/requirements/personal-data-lifecycle-protection)
- [++ Employee attempts to modify pay rate++](https://quality.arc42.org/requirements/employee-attempts-to-modify-pay-rate)
- [++ Encrypted storage++](https://quality.arc42.org/requirements/encrypted-storage)
- [++ Financial transactions are ACID-compliant and fully reconcilable++](https://quality.arc42.org/requirements/financial-transactions-are-acid-compliant)
- [++ Governance policies are enforced and auditable++](https://quality.arc42.org/requirements/governance-policy-enforcement)
- [++ Public API intrusion attempts blocked and alerted++](https://quality.arc42.org/requirements/public-api-intrusion-attempts-blocked)
- [++ Every data modification is logged++](https://quality.arc42.org/requirements/every-data-modification-is-logged)
- [++ Confidentiality by multi-tenancy++](https://quality.arc42.org/requirements/confidentiality-by-multitenance)
- [++ Tamper-Evident Digital Contract Signatures++](https://quality.arc42.org/requirements/tamper-evident-digital-signatures)
- [++ Only authenticated users can access data++](https://quality.arc42.org/requirements/only-authenticated-users-can-access)
- [++ Parallel Data Modification++](https://quality.arc42.org/requirements/parallel-data-modification)
- [++ Protect Data by Establishing Security Protocols++](https://quality.arc42.org/requirements/protect-data-by-security-procols)
- [++ Avoid common vulnerabilities++](https://quality.arc42.org/requirements/avoid-common-vulnerabilities)
- [++ Zero-knowledge data storage++](https://quality.arc42.org/requirements/zero-knowledge-data-storage)

### Approaches tagged with #secure

- [++ API Gateway++](https://quality.arc42.org/approaches/api-gateway)
- [++ Encryption at Rest + in Transit++](https://quality.arc42.org/approaches/encryption-at-rest-and-in-transit)
- [++ Fine-Grained Authorization (RBAC/ABAC)++](https://quality.arc42.org/approaches/fine-grained-authorization)
- [++ Input Sanitization / Output Encoding++](https://quality.arc42.org/approaches/input-sanitization-output-encoding)
- [++ Least Privilege++](https://quality.arc42.org/approaches/least-privilege)
- [++ Rate Limiting++](https://quality.arc42.org/approaches/rate-limiting)
- [++ Secret Management++](https://quality.arc42.org/approaches/secret-management)
- [++ Strong Authentication (MFA / OIDC)++](https://quality.arc42.org/approaches/strong-authentication)

### Standards tagged with #secure

- [++ CRA++](https://quality.arc42.org/standards/cra)
- [++ ETSI EN 304 223++](https://quality.arc42.org/standards/etsi-en-304-223)
- [++ GDPR++](https://quality.arc42.org/standards/gdpr)
- [++ IEC 62443++](https://quality.arc42.org/standards/iec-62443)
- [++ ISO 15408++](https://quality.arc42.org/standards/iso-15408)
- [++ ISO/IEC TR 24028++](https://quality.arc42.org/standards/iso-24028)
- [++ ISO/IEC 27001++](https://quality.arc42.org/standards/iso-27001)
- [++ NIST SP 800-53++](https://quality.arc42.org/standards/nist-800-53)
- [++ NIST AI RMF++](https://quality.arc42.org/standards/nist-ai-rmf)
- [++ NIST PF++](https://quality.arc42.org/standards/nist-privacy-framework)
- [++ OWASP ASVS++](https://quality.arc42.org/standards/owasp-asvs)
- [++ PCI DSS++](https://quality.arc42.org/standards/pci-dss)
- [++ SOC 2++](https://quality.arc42.org/standards/soc-2)

## Safe

A _safety- or life-critical_ system is a system whose failure or malfunction may result in one (or more) of the following outcomes:

- death or serious injury to people
- loss or severe damage to equipment/property
- environmental harm  
  Quoted from ++[Wikipedia/Safety-critical system](https://en.wikipedia.org/wiki/Safety-critical_system)++

Safety means:

- protected from harm or other danger
- in control of recognized or accepted dangers or hazards
- achieve an acceptable level of risk  
  Quoted from ++[Wikipedia/Safety](https://en.wikipedia.org/wiki/Safety)++

### Typical Acceptance Criteria

**Scenario Response Measures from [Bass et al.]**

- Amount or percentage of unsafe states that are avoided
- Amount or percentage of unsafe states from which the system can (automatically) recover
- Change in risk exposure: size(loss) \* prob(loss)
- Percentage of times the system can recover
- Amount of time the system is in a degraded or safe mode
- Amount or percentage of time the system is shut down
- Elapsed time to enter and recover (from manual operation, from a safe or degraded mode)  
  ++[Bass et al., 2021](https://quality.arc42.org/references/#bass2021software)++

### What Stakeholders mean by _safe_

| Stakeholder                                                             | (potential) Expectation for safe                           |
| ----------------------------------------------------------------------- | ---------------------------------------------------------- |
| User                                                                    | \* using the system will never cause any risk to my health |
| \* it is not possible to injure myself accidentally by using the system |
| Management                                                              | \* minimal risk of any liability lawsuit                   |

- no person will ever get hurt when using or maintaining our system
- the system poses no risk or danger to any humans’ health
- the system poses no risk to the environment |
  | Developer | development processes comply with appropriate safety standards and regulations, e.g. SPICE |
  | Tester | - |
  | Admin | - |
  | Domain-Expert | the system and its implementation comply with all required safety standards, like ISO-26262 |
  | Others | Safety auditors, government agencies requiring compliance with safety standards, law |

### Qualities tagged with #safe

- [++ Bias Mitigation++](https://quality.arc42.org/qualities/bias-mitigation)
- [++ Certifiability++](https://quality.arc42.org/qualities/certifiability)
- [++ Compliance++](https://quality.arc42.org/qualities/compliance)
- [++ Explainability++](https://quality.arc42.org/qualities/explainability)
- [++ Fail safe++](https://quality.arc42.org/qualities/fail-safe)
- [++ Failure Transparency++](https://quality.arc42.org/qualities/failure-transparency)
- [++ Fairness++](https://quality.arc42.org/qualities/fairness)
- [++ Fault isolation++](https://quality.arc42.org/qualities/fault-isolation)
- [++ Hazard warning++](https://quality.arc42.org/qualities/hazard-warning)
- [++ Operational constraint++](https://quality.arc42.org/qualities/operational-constraint)
- [++ Patient Safety++](https://quality.arc42.org/qualities/patient-safety)
- [++ Provability++](https://quality.arc42.org/qualities/provability)
- [++ Risk identification++](https://quality.arc42.org/qualities/risk-identification)
- [++ Safe integration++](https://quality.arc42.org/qualities/safe-integration)
- [++ Safety++](https://quality.arc42.org/qualities/safety)

### Requirements tagged with #safe

- [++ Medical triage model confidence is calibrated++](https://quality.arc42.org/requirements/calibrated-medical-triage-confidence)
- [++ Service Circuit Breakers and Graceful Degradation++](https://quality.arc42.org/requirements/circuit-breaker-failure-transparency)
- [++ Content Moderation Fairness++](https://quality.arc42.org/requirements/content-moderation-fairness)
- [++ Credit Scoring Fairness++](https://quality.arc42.org/requirements/credit-scoring-fairness)
- [++ Deterministic behavior for medical imaging++](https://quality.arc42.org/requirements/deterministic-behavior-for-medical-imaging)
- [++ Facial Recognition Bias Mitigation++](https://quality.arc42.org/requirements/facial-recognition-bias-mitigation)
- [++ Global Explainability++](https://quality.arc42.org/requirements/global-explainability)
- [++ Severe errors are detected and the system shuts down into safe state++](https://quality.arc42.org/requirements/shutdown-to-safe-state)
- [++ Grounded and explainable loan decision++](https://quality.arc42.org/requirements/grounded-explainable-loan-decision)
- [++ Grounded medical triage draft++](https://quality.arc42.org/requirements/grounded-medical-triage-draft)
- [++ Backup patient monitoring sensor takes over++](https://quality.arc42.org/requirements/backup-patient-monitoring-sensor)
- [++ Local Explainability++](https://quality.arc42.org/requirements/local-explainability)
- [++ Patient Data Quality in Healthcare System++](https://quality.arc42.org/requirements/patient-data-quality)
- [++ Protect Data by Establishing Security Protocols++](https://quality.arc42.org/requirements/protect-data-by-security-procols)
- [++ Provable Insulin Dosage Safety++](https://quality.arc42.org/requirements/provable-insulin-dosage-safety)
- [++ Provable railway interlocking routing logic++](https://quality.arc42.org/requirements/provable-railway-interlocking-routing-logic)
- [++ Provable Railway Interlocking Safety++](https://quality.arc42.org/requirements/provable-railway-interlocking-safety)
- [++ Reliable ERH System++](https://quality.arc42.org/requirements/reliable-erh-system)
- [++ Reliable Backup and Restore++](https://quality.arc42.org/requirements/reliable-backup-and-restore)
- [++ Replication and Quorum Reads/Writes++](https://quality.arc42.org/requirements/replication-and-quorum-failure-transparency)

### Approaches tagged with #safe

- [++ B-Method++](https://quality.arc42.org/approaches/b-method)
- [++ Fail-Safe Defaults++](https://quality.arc42.org/approaches/fail-safe-defaults)
- [++ Safety Interlocks++](https://quality.arc42.org/approaches/safety-interlocks)
- [++ Watchdog Supervision++](https://quality.arc42.org/approaches/watchdog-supervision)

### Standards tagged with #safe

- [++ IEC 61508++](https://quality.arc42.org/standards/iec-61508)
- [++ IEC 62304++](https://quality.arc42.org/standards/iec-62304)
- [++ ISO 26262++](https://quality.arc42.org/standards/iso-26262)
- [++ DO-178C++](https://quality.arc42.org/standards/do-178c)
- [++ MISRA-C++](https://quality.arc42.org/standards/misra-c)

## Operable

Easy to:

- build (compile, package)
- install, deploy
- configure
- operate, monitor, supervise, control
- decommission

Deployability is a…  
Measure of cost, time or process effectiveness for a deployment, for a series of deployments over time.  
++[Bass et al., 2021](https://quality.arc42.org/references/#bass2021software)++

### Typical Acceptance Criteria

**Scenario Response Measures for “Deployability” from [Bass et al.]**  
Bass et al. define ++[deployability](https://quality.arc42.org/qualities/deployability)++ as a property, and somehow omit other operational characteristics.  
Cost in terms of

- Number, size and complexity of affected artifacts
- Average/worst-case effort
- Elapsed clock or calendar time
- Money (direct outlay or opportunity cost)
- New defects introduced  
  Extend to which this deployment affects other functions or quality attributes.
- Number of failed deployments
- Repeatability of the process
- Traceability of the process
- Cycle time of the process  
  ++[Bass et al., 2021](https://quality.arc42.org/references/#bass2021software)++

### What Stakeholders mean by _operable_

| Stakeholder                                                                              | (potential) Expectation for operable |
| ---------------------------------------------------------------------------------------- | ------------------------------------ |
| User                                                                                     | -                                    |
| Product-Owner                                                                            | -                                    |
| Management                                                                               | \* appropriate operational costs     |
| \* appropriate licensing cost for required 3rd party software, like database, middleware |
| Developer                                                                                | \* automated test and build          |

- appropriate automation of deployments
- appropriate similarity of development and production environments |
  | Tester | - |
  | Admin | \* easy to build and deploy
- appropriate monitoring facilities
- appropriate procedures for crisis management in place
- appropriate management of credentials required |
  | Domain-Expert | - |
  | Others | - |

**Qualities tagged with #operable**

- [++ Appropriateness recognizability++](https://quality.arc42.org/qualities/appropriateness-recognizability)
- [++ Auditability++](https://quality.arc42.org/qualities/auditability)
- [++ Autonomy++](https://quality.arc42.org/qualities/autonomy)
- [++ Backward compatibility++](https://quality.arc42.org/qualities/backward-compatibility)
- [++ Change failure rate++](https://quality.arc42.org/qualities/change-failure-rate)
- [++ Compatibility++](https://quality.arc42.org/qualities/compatibility)
- [++ Controllability++](https://quality.arc42.org/qualities/controllability)
- [++ Cycle time++](https://quality.arc42.org/qualities/cycle-time)
- [++ Debuggability++](https://quality.arc42.org/qualities/debuggability)
- [++ Deployability++](https://quality.arc42.org/qualities/deployability)
- [++ Deployment frequency++](https://quality.arc42.org/qualities/deployment-frequency)
- [++ Devops-Metrics++](https://quality.arc42.org/qualities/devops-metrics)
- [++ Diagnosability++](https://quality.arc42.org/qualities/diagnosability)
- [++ Drift Detectability++](https://quality.arc42.org/qualities/drift-detectability)
- [++ Ease of Use++](https://quality.arc42.org/qualities/ease-of-use)
- [++ Expected physical environment++](https://quality.arc42.org/qualities/expected-physical-environment)
- [++ Governability++](https://quality.arc42.org/qualities/governability)
- [++ Installability++](https://quality.arc42.org/qualities/installability)
- [++ Integrability++](https://quality.arc42.org/qualities/integrability)
- [++ Interaction capability++](https://quality.arc42.org/qualities/interaction-capability)
- [++ Interchangeability++](https://quality.arc42.org/qualities/interchangeability)
- [++ Interoperability++](https://quality.arc42.org/qualities/interoperability)
- [++ Latency++](https://quality.arc42.org/qualities/latency)
- [++ Lead time for changes++](https://quality.arc42.org/qualities/lead-time-for-changes)
- [++ Learnability++](https://quality.arc42.org/qualities/learnability)
- [++ Legal Requirements++](https://quality.arc42.org/qualities/legal-requirements)
- [++ Mean time between failures++](https://quality.arc42.org/qualities/mean-time-between-failures)
- [++ Mean time to recovery++](https://quality.arc42.org/qualities/mean-time-to-recovery)
- [++ Observability++](https://quality.arc42.org/qualities/observability)
- [++ Operability++](https://quality.arc42.org/qualities/operability)
- [++ Operational and Environment Requirements++](https://quality.arc42.org/qualities/operational-environment-requirements)
- [++ Portability++](https://quality.arc42.org/qualities/portability)
- [++ Redundancy++](https://quality.arc42.org/qualities/redundancy)
- [++ Releasability++](https://quality.arc42.org/qualities/releasability)
- [++ Replaceability++](https://quality.arc42.org/qualities/replaceability)
- [++ Traceability++](https://quality.arc42.org/qualities/traceability)
- [++ Understandability++](https://quality.arc42.org/qualities/understandability)
- [++ Updateability++](https://quality.arc42.org/qualities/updateability)
- [++ Upgradeability++](https://quality.arc42.org/qualities/upgradeability)
- [++ Usability++](https://quality.arc42.org/qualities/usability)
- [++ User error protection++](https://quality.arc42.org/qualities/user-error-protection)

### Requirements tagged with #operable

- [++ Core functions can be used on multiple OSs++](https://quality.arc42.org/requirements/core-functions-on-mac-win-linux)
- [++ CRM System Data Synchronization++](https://quality.arc42.org/requirements/crm-data-synchronization)
- [++ Any passing build deploys to production within 15 minutes++](https://quality.arc42.org/requirements/deploy-to-production-within-15-minutes)
- [++ Fast deployment++](https://quality.arc42.org/requirements/fast-deployment)
- [++ Fast rollout of changes++](https://quality.arc42.org/requirements/fast-rollout-of-changes)
- [++ Fraud detection drift detected within 1 hour++](https://quality.arc42.org/requirements/fraud-detection-drift-detected-within-1-hour)
- [++ Governance policies are enforced and auditable++](https://quality.arc42.org/requirements/governance-policy-enforcement)
- [++ Severe errors are detected and the system shuts down into safe state++](https://quality.arc42.org/requirements/shutdown-to-safe-state)
- [++ Independent replacement of subsystem++](https://quality.arc42.org/requirements/independent-replacement-of-subsystem)
- [++ Rollout of a new feature++](https://quality.arc42.org/requirements/rollout-new-feature)
- [++ Interoperable with Java 12++](https://quality.arc42.org/requirements/interoperable-with-java-12)
- [++ Low effort deployment++](https://quality.arc42.org/requirements/low-effort-deployment)
- [++ Restored to fully functional state 12h after complete failure++](https://quality.arc42.org/requirements/mttr-12h)
- [++ System can run >12h without re-booting the operating system++](https://quality.arc42.org/requirements/long-running-without-reboot)
- [++ On-prem installation ready in 30 minutes++](https://quality.arc42.org/requirements/on-prem-installation-ready-in-30-min)
- [++ Portable Business Data Checker++](https://quality.arc42.org/requirements/portable-business-data-checker)
- [++ Production anomalies detectable within 2 minutes++](https://quality.arc42.org/requirements/production-anomalies-detectable-within-2-minutes)
- [++ Quick unit tests++](https://quality.arc42.org/requirements/quick-unit-tests)
- [++ Available 7x24 with 99% uptime++](https://quality.arc42.org/requirements/available-7-24-99)
- [++ Retail demand forecast drift detected before replenishment++](https://quality.arc42.org/requirements/retail-demand-forecast-drift-before-replenishment)
- [++ System runs offline++](https://quality.arc42.org/requirements/system-runs-offline)
- [++ Fleet OTA updates with safe rollback++](https://quality.arc42.org/requirements/fleet-ota-updates-with-safe-rollback)
- [++ User Interface can be used in Current Browsers++](https://quality.arc42.org/requirements/user-interface-works-with-current-browsers)
- [++ Zone failure: no service interruption++](https://quality.arc42.org/requirements/zone-failure-no-service-interruption)

### Approaches tagged with #operable

- [++ API Gateway++](https://quality.arc42.org/approaches/api-gateway)
- [++ Blue-Green Deployment++](https://quality.arc42.org/approaches/blue-green-deployment)
- [++ Canary Deployment++](https://quality.arc42.org/approaches/canary-deployment)
- [++ Circuit Breaker++](https://quality.arc42.org/approaches/circuit-breaker)
- [++ Content Delivery Network (CDN)++](https://quality.arc42.org/approaches/content-delivery-network)
- [++ Event-Driven Architecture++](https://quality.arc42.org/approaches/event-driven-architecture)
- [++ Feature Toggles++](https://quality.arc42.org/approaches/feature-toggles)
- [++ Secret Management++](https://quality.arc42.org/approaches/secret-management)

## Suitable

_Suitable_ might be the most generic term within the Q42 dimensions.  
Being right or appropriate for a particular person, purpose, or situation.

Note: In previous versions of Q42, the term “_testable_” was used instead of _suitable_. Users found that to be overly specific, see the discussion ++[here](https://github.com/arc42/quality.arc42.org-site/issues/90)++.

### Definition

(Functional) Suitability:  
…provides functions that meet stated and implied needs of intended users when it is used under specified conditions.  
++[ISO-25010:2023](https://quality.arc42.org/references/#iso-25010-2023)++

The ISO restricts _Suitability_ to functional aspects. In our opinion, it is useful in a broader sense: For example, seen from a testing perspective, suitable can mean “easy to test”.

### “Responsibility” as an alternative term

++[Bass et al., 2021](https://quality.arc42.org/references/#bass2021software)++ propose to use the term “responsibility” instead of (functional) suitability. That is, from our perspective, a matter of taste.

##

### Typical Acceptance Criteria

(todo)

##

### What Stakeholders mean by _suitable_

| Stakeholder | (potential) Expectation for suitable                               |
| ----------- | ------------------------------------------------------------------ |
| User        | \* offers the required (suitable) functions in appropriate quality |

- adequate performance
- adequate robustness
- adequate accessibility and useability |
  | Product-Owner | \* providing appropriate (suitable) functions in suitable quality
- easy to enhance with new functions or features |
  | Management | \* appropriate cost/benefit ratio
- appropriate effort required to add new features or functions |
  | Developer | \* appropriate effort required to understand internals
- good code readability
- appropriate effort required to locate and fix bugs
- appropriate technologies used
- appropriate technical documentation |
  | Tester | _appropriate effort required for testing |
  | Admin |_ easy to perform required administration tasks (like deploy, install, configure etc) |
  | Domain-Expert | - |
  | Others | - |

### Qualities tagged with #suitable

- [++ Affordability++](https://quality.arc42.org/qualities/affordability)
- [++ Autonomy++](https://quality.arc42.org/qualities/autonomy)
- [++ Bias Mitigation++](https://quality.arc42.org/qualities/bias-mitigation)
- [++ Calibration++](https://quality.arc42.org/qualities/calibration)
- [++ Certifiability++](https://quality.arc42.org/qualities/certifiability)
- [++ Cohesion++](https://quality.arc42.org/qualities/cohesion)
- [++ Completeness++](https://quality.arc42.org/qualities/completeness)
- [++ Compliance++](https://quality.arc42.org/qualities/compliance)
- [++ Correctness++](https://quality.arc42.org/qualities/correctness)
- [++ Cost++](https://quality.arc42.org/qualities/cost)
- [++ Cycle time++](https://quality.arc42.org/qualities/cycle-time)
- [++ Data Localization++](https://quality.arc42.org/qualities/data-localization)
- [++ Data Quality++](https://quality.arc42.org/qualities/data-quality)
- [++ Data Residency++](https://quality.arc42.org/qualities/data-residency)
- [++ Data Sovereignty++](https://quality.arc42.org/qualities/data-sovereignty)
- [++ Deployability++](https://quality.arc42.org/qualities/deployability)
- [++ Deployment frequency++](https://quality.arc42.org/qualities/deployment-frequency)
- [++ Expected physical environment++](https://quality.arc42.org/qualities/expected-physical-environment)
- [++ Explainability++](https://quality.arc42.org/qualities/explainability)
- [++ Fairness++](https://quality.arc42.org/qualities/fairness)
- [++ Functional Appropriateness++](https://quality.arc42.org/qualities/functional-appropriateness)
- [++ Functional completeness++](https://quality.arc42.org/qualities/functional-completeness)
- [++ Functional suitability++](https://quality.arc42.org/qualities/functional-suitability)
- [++ Functionality++](https://quality.arc42.org/qualities/functionality)
- [++ Groundedness++](https://quality.arc42.org/qualities/groundedness)
- [++ Loose Coupling++](https://quality.arc42.org/qualities/loose-coupling)
- [++ Mean time to recovery++](https://quality.arc42.org/qualities/mean-time-to-recovery)
- [++ Model Transparency++](https://quality.arc42.org/qualities/model-transparency)
- [++ Suitability++](https://quality.arc42.org/qualities/suitability)
- [++ Test Coverage++](https://quality.arc42.org/qualities/test-coverage)
- [++ Testability++](https://quality.arc42.org/qualities/testability)
- [++ Timeliness++](https://quality.arc42.org/qualities/timeliness)
- [++ Versatility++](https://quality.arc42.org/qualities/versatility)

### Requirements tagged with #suitable

- [++ Access control is enforced++](https://quality.arc42.org/requirements/access-control-is-enforced)
- [++ Access Control via SSO++](https://quality.arc42.org/requirements/access-control-via-sso)
- [++ Detailed audit log++](https://quality.arc42.org/requirements/detailed-audit-log)
- [++ Accurate estimate of insurance contract rate++](https://quality.arc42.org/requirements/accurate-estimate-of-insurance-rate)
- [++ Add new product under 60 minutes++](https://quality.arc42.org/requirements/add-new-product)
- [++ Affordable CRM (customer relationship management)++](https://quality.arc42.org/requirements/affordable-crm)
- [++ Assess impact of proposed change++](https://quality.arc42.org/requirements/assess-impact-of-proposed-change)
- [++ Authenticity of a digital document++](https://quality.arc42.org/requirements/authenticity-of-digital-document)
- [++ Budget constrained library update++](https://quality.arc42.org/requirements/budget-constraint-library-update)
- [++ Content Moderation Fairness++](https://quality.arc42.org/requirements/content-moderation-fairness)
- [++ Convenient online banking++](https://quality.arc42.org/requirements/convenient-online-banking)
- [++ Credit Scoring Fairness++](https://quality.arc42.org/requirements/credit-scoring-fairness)
- [++ Data Localization for Citizen Records++](https://quality.arc42.org/requirements/data-localization-for-citizen-records)
- [++ Any passing build deploys to production within 15 minutes++](https://quality.arc42.org/requirements/deploy-to-production-within-15-minutes)
- [++ Display Data Based on Context++](https://quality.arc42.org/requirements/display-data-based-on-context)
- [++ Automated Personal Data Lifecycle Protection++](https://quality.arc42.org/requirements/personal-data-lifecycle-protection)
- [++ Understandable acceptance test cases++](https://quality.arc42.org/requirements/understandable-acceptance-tests)
- [++ Efficient generation of test data++](https://quality.arc42.org/requirements/efficient-generation-of-test-data)
- [++ Financial Data Accuracy for Reporting++](https://quality.arc42.org/requirements/financial-data-accuracy)
- [++ Global Explainability++](https://quality.arc42.org/requirements/global-explainability)
- [++ Grounded customer support answer++](https://quality.arc42.org/requirements/grounded-customer-support-answer)
- [++ Grounded and explainable loan decision++](https://quality.arc42.org/requirements/grounded-explainable-loan-decision)
- [++ Grounded medical triage draft++](https://quality.arc42.org/requirements/grounded-medical-triage-draft)
- [++ Hiring Algorithm Bias Mitigation++](https://quality.arc42.org/requirements/hiring-algorithm-bias-mitigation)
- [++ Rollout of a new feature++](https://quality.arc42.org/requirements/rollout-new-feature)
- [++ Local Explainability++](https://quality.arc42.org/requirements/local-explainability)
- [++ Monolith loose coupling: change blast radius++](https://quality.arc42.org/requirements/monolith-loose-coupling-change-blast-radius)
- [++ Service loose coupling: change blast radius++](https://quality.arc42.org/requirements/service-loose-coupling-change-blast-radius)
- [++ Restore Filter after Log In++](https://quality.arc42.org/requirements/restore-filter-after-log-in)
- [++ Search and graph text filter available on Q42++](https://quality.arc42.org/requirements/search-and-graph-text-filter-available-on-q42)
- [++ Test with path coverage in 30min++](https://quality.arc42.org/requirements/test-with-path-coverage-30min)
- [++ Up to date API++](https://quality.arc42.org/requirements/up-to-date-api)
- [++ Usable on Factory Floor++](https://quality.arc42.org/requirements/usable-on-factory-floor)
- [++ Usable With Gloves++](https://quality.arc42.org/requirements/usable-with-gloves)

### Approaches tagged with #suitable

- [++ A/B Testing++](https://quality.arc42.org/approaches/ab-testing)

## Maintainable

Easy to:

- understand and analyze when changes are needed
- modify with low effort and low risk
- verify and test after changes
- update or upgrade over the system lifetime

### Definition

Capability of a product to be modified by the intended maintainers with effectiveness and efficiency.  
Modifications can include corrections, improvements or adaptation to changes in environment and requirements. Maintainability includes installation of updates and upgrades.  
++[ISO-25010:2023](https://quality.arc42.org/references/#iso-25010-2023)++

Maintainability is the ease with which software can be maintained, enhanced, adapted, or corrected to satisfy specified requirements.  
++[SWEBOK (IEEE), citing IEEE 610.12](https://quality.arc42.org/references/#swebok)++

Maintainability is concerned with modifications after the software baseline is established.  
We measure maintainability as the amount of work required to modify, test, and maintain our software base in response to changes in environmental elements.  
++[Kazman et al., p.5](https://quality.arc42.org/references/#kazman-maintainability)++

### Typical Acceptance Criteria

Maintainable means “_economical and predictable change_”.  
When defining what _#maintainable_ means for a specific system and stakeholders, consider:

- Which types of change are expected (defect fix, refactoring, feature extension, dependency update)?
- How much code, configuration, and documentation should typically be affected?
- What regression risk and verification effort are acceptable after each change?  
  Typical acceptance criteria might include:
- Effort/time to implement representative changes
- Number and complexity of artifacts touched per change
- Change failure rate and rollback frequency
- Effort/time to analyze root causes and fix defects
- Effort/time to adapt or extend tests after changes

### Scenario Response Measures from [Bass et al.]

Cost in terms of:

- Number, size, complexity of affected artifacts
- Effort
- Elapsed time
- Money
- Extent to which this modification affects other quality attributes
- New defects introduced  
  ++[Bass et al., 2021](https://quality.arc42.org/references/#bass2021software)++

### _maintainable_ for Stakeholders

| Stakeholder   | (potential) Expectation for maintainable                        |
| ------------- | --------------------------------------------------------------- |
| User          | defects are fixed quickly and reliably                          |
| Product-Owner | predictable effort and lead time for requested changes          |
| Management    | lower long-term cost of change and reduced change risk          |
| Developer     | code is understandable, analyzable, modular, and safe to change |
| Tester        | tests can be adapted quickly; regressions are easy to detect    |
| Admin         | updates/upgrades can be applied with low operational risk       |
| Domain-Expert | business-rule changes can be implemented without long delays    |
| Others        | technical documentation remains current and change-oriented     |

**Qualities tagged with #maintainable**

- [++ Analysability++](https://quality.arc42.org/qualities/analysability)
- [++ Changeability++](https://quality.arc42.org/qualities/changeability)
- [++ Cohesion++](https://quality.arc42.org/qualities/cohesion)
- [++ Debuggability++](https://quality.arc42.org/qualities/debuggability)
- [++ Evolvability++](https://quality.arc42.org/qualities/evolvability)
- [++ Extensibility++](https://quality.arc42.org/qualities/extensibility)
- [++ Longevity++](https://quality.arc42.org/qualities/longevity)
- [++ Loose Coupling++](https://quality.arc42.org/qualities/loose-coupling)
- [++ Maintainability++](https://quality.arc42.org/qualities/maintainability)
- [++ Modifiability++](https://quality.arc42.org/qualities/modifiability)
- [++ Modularity++](https://quality.arc42.org/qualities/modularity)
- [++ Reusability++](https://quality.arc42.org/qualities/reusability)
- [++ Test Coverage++](https://quality.arc42.org/qualities/test-coverage)
- [++ Testability++](https://quality.arc42.org/qualities/testability)
- [++ Themability++](https://quality.arc42.org/qualities/themability)
- [++ Updateability++](https://quality.arc42.org/qualities/updateability)
- [++ Upgradeability++](https://quality.arc42.org/qualities/upgradeability)
- [++ Verifiability++](https://quality.arc42.org/qualities/verifiability)

### Requirements tagged with #maintainable

- [++ Adding a new entity type within 5 days and ≤ 3 modules++](https://quality.arc42.org/requirements/adding-entity-type-within-5-days)
- [++ Efficient change of business rules++](https://quality.arc42.org/requirements/luggage-routing)
- [++ Independent enhancement of subsystem++](https://quality.arc42.org/requirements/independent-enhancement-of-subsystem)
- [++ Monolith loose coupling: change blast radius++](https://quality.arc42.org/requirements/monolith-loose-coupling-change-blast-radius)
- [++ Service loose coupling: change blast radius++](https://quality.arc42.org/requirements/service-loose-coupling-change-blast-radius)
- [++ Modular System for Data Analysis++](https://quality.arc42.org/requirements/modular-system-for-data-analysis)
- [++ Good code readability score++](https://quality.arc42.org/requirements/good-code-readability-score)
- [++ Efficient update of annual accounting report++](https://quality.arc42.org/requirements/annual-tax-update)
- [++ Shared library adoption by product teams++](https://quality.arc42.org/requirements/shared-library-adoption-by-product-teams)
- [++ Test Coverage for Critical Business Logic++](https://quality.arc42.org/requirements/test-coverage-for-critical-business-logic)
- [++ Fleet OTA updates with safe rollback++](https://quality.arc42.org/requirements/fleet-ota-updates-with-safe-rollback)
- [++ Understandable generated code++](https://quality.arc42.org/requirements/understandable-generated-code)
- [++ Safety requirements traceable to executable evidence++](https://quality.arc42.org/requirements/safety-requirements-traceable-to-evidence)

</arc42-quality-model>
