---
words:
  2025-08-25: 603
tags:
  - MANASCI
---

## Purchase Cost of Inventory Items
Total Inventory cost can be written to include cost of purchased items
- Annual purchases cost is constant at D x C no matter the order policy, whre
C is the purchase cost per unit 
D is the annual demand in units
- Formula for average level of inventory 
- Holding cost often expressed as an annual percentage of the unit cost or price of the inventory
Cost of storing inventory 
$$I = Annual\,inventory\,holding\,charge\,of\,unit\,price\,or\,cost$$

## Reorder Point
- next decision is when to order
- time between placing an order and its receipt is called the Lead Time(L)/delivery time
$$
ROP = [Demand\,per\,day][Lead\,time\,for\,a\,new\,order/day]
$$
$$ROP = d * L$$

$$
[Inventory\,Position]=[Invenotry\,on\,hand][Inventory\,on\,Order]
$$

### EOQ w/o Instantaneous Receipt
- when inventory accumulates over the time, the instantaneous receipt assumption does not apply?
	- d must be taken into account
	- **Production run model**

$Q = \text{number of piecer per order/production run}$
$C_s = \text{Set-up cost}$
$C_h = \text{holding/carrying\,cost}$
$p = \text{daily production rate}$
$d = \text{daily demand}$
$t = \text{length of production in days}$


### Maximum Inventory Level 
$= ( \text{Total produced during the production run}) - (\text{Total used during the production run})$
$= (\text{Daily production rate)(Number of days production}) - (\text{Daily demand)(Number of days production})$
$=(pt)-(dt)$

Since Total Produced = $Q = Pt$ and $t=\frac{Q}{p}$

$$\text{Maximum Invetory Level} = pt-dt = p\frac{Q}{p}-d\frac{Q}{p} =Q [1 -\frac{d}{p}]$$
$$=Q [1 -\frac{d}{p}]$$
### Average Inventory
$$\frac {Q}{2}[1-\frac{d}{p}]$$
### Annual Holding Cost
$$C_h=\frac {Q}{2}[1-\frac{d}{p}]C_h$$
### Annual Set-up Cost
$$C_s= \frac {D}{Q}C_S$$
### Solving EOQ
$$Q*=\sqrt{\frac{2DC_s}{C_h(1-\frac{d}{p})}}$$






## Quantity Discount Model

\- basic EOQ model is adjusted by adding in the purchase or material cost
$$Total\,Cost=Material\,Cost+Ordering\,Cost+Holding\,Cost$$
> [!info]+
> Holding cost per unit is based on cost, so
> $$C_h=I*C$$
> where: I = holding cost as percentage of unit cost

$$Total\,Cost=DC+\frac{D}{Q}C_o+\frac{Q}{2}C_h$$



### Steps in the Process
1. For each discounted price(C), compute 
$$\sqrt{\frac{2DC_o}{IC}}$$
2. If EOQ < Minimum for discount, adjust the quantity to Q = Minimum for discount
3. For each EOQ or adjusted Q, compute
$$Total\,Cost=DC+\frac{D}{Q}C_o+\frac{Q}{2}C_h$$
4. Choose the lowest-cost quantity

### Use of Safety Stock
- objective is to choose a safety stock amount the minimizes total holding and stockout costs
- if variation in demand and holding and stockout costs are known, payoff/cost tables could be used to determine safety stock
- More general approach is to choose a desired **service level**  based on satisfying customer demand

***

## Just-Time-Inventory Control

- Organizations have tried to have less in-process inventory hand achieve greeter efficiency in the production process
- This is known as **JIT Inventory**
	- The Inventory arrives just in time to be used during the manufacturing process 
- One technique of implementing JIT is a manual process called Kanban