# Lecture 14 - 16/11/18

## Parts of an LCA (cont.)

### Inventory Analysis

![](https://lh3.googleusercontent.com/t-xDC2bILA7nM3pcjjRlU47-C4uDujPXGdVDAmXCMU_kX7u4pMnmozhIAeDCeGSekNLW-T8VeFMO)
- We're most interested in what comes in and out of the process - energy, raw materials, chemicals etc.
- The process is modelled down to unit processes, to a level that we can collect data
- Data is collected
	- Primary Data - measured directly from the system under study - e.g. energy used, amount of chemical put in etc.
	- Secondary Data - data from other sources - e.g. how much materia in outsourced production
- Data is validated and assessed for quality
- Data is normalised with regards to reference flow - the flow of material and energy required to deliver the functional unit

![enter image description here](https://lh3.googleusercontent.com/eEjkXeb4TtO9Yb6GLU-KJdCJcdAplGDmfDJ8X2BFwlOFs90wxdJpLgsD1Q8CczIFljvxSTY9yroe)
Processes are modelled by being broken down into sub-systems until they become 'unit processes'

#### Modelling the Process

- Identify the key relevant Elementary Flows - materials and energy entering and leaving the process directly to the environment
- We distinguish between the systems
	- Foreground System - system that we have more control over/or one that we want a more detailed understanding of
	- Background System - provide inputs into foreground system - modelled in less detail
		- e.g. energy system, forestry, mining etc.

Cut-off rules -

- Cut-off rules dictate which parts of the process are 'cut off' e.g. disregarded due to their environmental impact being negligible
- Typically a unit process can be left out if they contribute less than 1% of a substance or energy
- Total application of cut-off rules shouldn't exceed 5% of a substance or energy - but how can you tell before you've done the analysis?
	- Can conduct a scoping LCA to determine this

##### Example Process Models

![enter image description here](https://lh3.googleusercontent.com/bffJtdkVd7LcsAcFrlhlYAU4CdNMEv57XbYECHr_JWh9NflD7hoKApm4XsfQ7ZcBNrJ94zgahTp7)
- Above is a process model for drinks cans
- Extract ore and using Bayer process and electrolysis to manufacture the metal
- Cast and create the can, and transport these
- Note that there are several recycling loops
- Disposal of waste at the bottom

![enter image description here](https://lh3.googleusercontent.com/hYo_Cu7jhpzwRkRqqd03hyw_Hod60J75vR2rI37Pje1Kxn6MoCha9pjEPruXmCL7ZZrtfsfJ2MSJ)
Digital services are modelled a bit different - here we see the networks

##### Sources and Quality of Data

Sources of primary data

- Direct measurement of a process
- Utility and fuel bills
- Process monitoring and control software
- Equipment and process specification
- Company data logs and records

Sources of secondary data

- LCA data bases
- Other LCAs
- Estimation (expected to be conservative)

It's important to be open about data quality -

- Clearly identify data sources, including missing data and estimates
- Highlight the quality of different data sources in the LCA
- Note potential quality issues
	- Time/age of data
	- Geographical coverage
	- Technology involves
	- Representativeness of data
	- Consistency
	- Precision

#### Modelling the Use Phase

- Modelling the use phase requires a model of user behabiour
- This is usually an 'average' user, but this can mask significant variations so this should sometimes be made explicit

#### Challenges for Assessment of Electronic and IT Products

- Input data is scarce - uncertainty is difficult
- Large supply chains - high potential for cut-off errors
- Quick change of materials and product composition
- Large amount of air-shipping as electronics are high-value
- Use phase is significant and high variance in use patterns

#### Allocation in LCA

- Often a specific functional unit takes a 'share' of some process output - so needs a share of associated environmental impact
- Allocation is the process of deciding what share  to allocate

There are two approaches to allication

- System expansion
	- Splitting into sub-processes to see which part is relevant to the service being analysis
	- More time-consuming
- Partitioning
	- Leave black box and argue the share that is for the service being analysed
	- Increases uncertainty
	- Needs specific data to be collected to help in allocation

![enter image description here](https://lh3.googleusercontent.com/Fxb8eQ_w3-8qcmdfY7_IbgP5CtgBCrCu3F7Z1CX-uq1l0VdQYfnv8lzf5RDEm3hveOuqN4lzNTc1)
System expansion splits out relevant parts

![enter image description here](https://lh3.googleusercontent.com/O49r1OYxZOiX5EyqdIxAK3lveee6vYkSssO13Ry-uy32iIyDFA_CyKrz5blxmwIQ30WKpd6fI2uL)
Partitioning looks at the limiting factor (e.g. weight in a lorry) used to split to give allocation

##### Example - Playing Music

Some possible ways are

- Expansion - measure power consumption per component (e.g. used X% of CPU and CPU uses Y much energy)
- Problems with this thought
	- Power consumption is non-linear
	- Idle power - how is energy from the idle process allocated?
- Possible to partition - how much time a software is used, or even perceived user relevance - if people keep Facebook on to get notifications then this can be the measure
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc1NTU3NTkyLDIyMTk2OTc1LDEyNjQ2ND
U5NjYsNjk3MDk1MTU5LDE2MjY3NjU1MjAsLTE4OTU4MTQ2NDks
NzMwOTk4MTE2XX0=
-->