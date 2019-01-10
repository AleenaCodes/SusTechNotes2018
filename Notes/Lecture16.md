# Lecture 16 - 30/11/18

## Assessment

- Drop-in sessions available for coursework
- End of next week will have covered all content
- Last week - review lecture and tell you which parts will be covered in which assessment
- Will tell which things need to be known in details, and which just key idea
- Recent exams are indicative of what this year will be

## Economic Input-Output LCA

This is different from process-based LCA

- Doesn't look at a specific pipeline, looks at things on a sectoral level
	- Hence less detailed
- Approach to allocation is financial, as opposed to mass/energy flow
	- Allocation is based on value derived from the service

### EIOLCA - The Model of the Economy

- Divide the economy into sectors e.g. 'Computer Peripherals', 'Air Transportation', 'Banking'
- Governments produce 'Input Output' tables of the economy
	- These say how much different sectors buy from other ones in a give time period
	- This provides a measure of how money flows through sectors
- The key idea is being able to see for one product how much money has been spent in other sectors

### Determine Environmental Impacts

- If there is data on the environmental impact of each whole sector, and data about which sectors are used in a single product
	- Then we can allocate the environmental impact of each sector as a percentage to the product
- This gives a cradle-to-gate life cycle impact of a product, but doesn't say anything about use or disposal of the product

### Performing an Economic Input Output LCA

1. Estimate output changes to final demand sector
	- i.e. see how much money someone spends to buy the product
2. Assess direct and indirect economic change with IO model
	- Direct change - making product results in purchase of raw materials
	- Indirect change - the industry that provides raw material will spend money on their own expenses e.g. shipping, mining etc.
3. Assess environmental discharges as a result of each sector output
	- See what share of the product should be given to each of the sectors
4. Sum sector discharges to find overal discharges

Can view stats for different products on [http://www.eiolca.net/](http://www.eiolca.net/)

###  Uncertainties/Inaccuracies

There are many things that can affect the LCA impact

- They look at impacts from all players in a sector - so more expensive products will have more environmental allocation on it
- Models are domestic and assume abroad data is the same - not always true
- Impacts are calculated 'cradle-to-gate' so ignores usage and disposable
- If a company invests in a 'clean' manufacturing plant but passes the cost of that onto the consumers, then its actual impact goes down but according to the EIOLCA it's share of sectoral impacts will go up
- Data can be old or inaccurate
	- e.g. in the US toxic releases below a certain level are not required to be reported
- Allocation of aggregated original data
	- e.g. 'office space' do not have the same impacts in different sectors
- Aggregation of sectors
	- e.g. 'power generation' includes coal and hydro which have very different impacts

### Advantages/Disadvantages of EIO-LCA

Advantages -

- Includes activity in the whole economy, even minor contributers
	- So the system boundary is large compares to a typical process LCA
- Quick, cheap and easy to perform
- Uses publically available data so easy to replicate

Disadvantages -

- Aggregate, sectoral level analysis
- Financial allocation may not reflect reality
- Data is old, assumes US (or other certain region) and uncertain

### What are EIO-LCAs good for

- Not good for -

- Detailed assessments of change to manufacturing process
- Identifying process 'hotspots'#

Good for -

- National level analyses to guide policy
- Broad brush assessments of future products
- Providing inputs into parts of a Process LCA (a Hybrid LCA)

### A Simplified Example

Using the table

![](https://lh3.googleusercontent.com/7Q8KSdupyQzWEsX89JXMi2zadCKU9vrU_t1dyd_W-ir5vBfInkUmcE5aoJBGD_r0T4O9caoRhJHD)
This gives data to say - if you buy one unit from one sector, what percentage is rippled down into the next sector. So here - if you buy $1$ unit of peripherals, you'll be buying $0.1$ units of components, and $0.2$ units of electricity in that process

So say a computer needs £100 or peripherals, £50 of components, and £1 of electricity to build. How much electricity is used across it's entire supply chain?

Define a desire output vector $y$ using the requirements of the computer $y =\left (\begin{array}{c} 100 \\ 50 \\ 1 \end{array}\right )$

To get the direct expenditure of the computer manufacture on each of the supply sectors. We take $\bold{I}y = y$

To get the direct expenditure by each of the supply sectors on their direct suppliers, we calculate $\bold{A} y$

$$
\bold{A} y = \left (\begin{array}{c} 
0 \\ 10 \\ 2.5
\end{array}\right )
$$

Where

- $0$ - expenditure by components and electricity on peripherals
- $10$ - expenditure by peripherals and electricity on components
- $2.5$ - expenditure by components and peripherals on electricity

$\bold{A}^2 y$ gives the expenditure on the secondary sectors by the tertiary sectors
$\bold{A}^3 y$ gives the expenditure on the tertiary sectors by the fourth degree sectors etc.

In our simple case - $\bold{A}^2 y = \left ( \begin{array}{c} 0 \\ 0 \\ 0.1 \end{array} \right )$ and $\bold{A}^3$ and all subsequent terms are zero

So the total expenditure of electricity in the supply chain is $1 + 2.5 + 0.1 = £3.60$

Hence to calculate the entire supply chain's use of different sectors, we calculate

$$(\bold{I} + \bold{A} + \bold{A}^2 + \bold{A}^3 + \bold{A}^4 + \dots) y = (\bold{I}-\bold{A})^{-1} y$$

## Hybrid LCA

A hybrid LCA uses both EIO and process-based approaches

- EIO approach to assess impacts associated with inputs to the process model
	- e.g. coal, iron etc.
- EIO approach for cradle-to-gate
	- e.g. car manufacturing
- Process approach for user-phase
	- e.g. car usage
- Process approach to adjust assumptions around direct environmental impacts of a sector
	- e.g. compare new iron smelting process with industry average process by propogating this across the model
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTg0ODk4NjQyMSw1MzY5NTY3MDQsMTQxND
AxMTY3OCwxMTU2NzA0MTc1LDc2Njc2NjEwMCwtMTc1MjIxNzk0
MCwtMjEzODc0ODYyMywxOTIyNjkyNTc3LC04MjkwNzIxNDcsMz
cyNjMxMTcyLDEzMzAwMjI4NzBdfQ==
-->