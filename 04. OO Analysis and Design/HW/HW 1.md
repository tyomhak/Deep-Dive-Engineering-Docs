[Project Description](HW%20-%20Project%20Description.pdf)
Create Use-Case and Concept Design Diagrams for the project.
# Country Insurance Toolkit (CIT)

## Requirements
### Usability

#### Users (policyholders and agents)
- log in to their portal (username, password).
- will be presented with their name and surname upon successful login.
- Can initiate the contract signing process by providing a vehicle's license plate number.

##### Policyholders
**Policyholders** are assigned a Bonus Malus (BM) class (1 to 22). Class is calculated based on active contracts and incidents (calculation outside scope).

**Individual Policyholders** (individual users)
- **view** active **contracts**
- can sign contracts only for vehicles registered under their name.

**Legal policyholders** (business representative users)
- **view** company's active **contracts**
- Required to provide their TPIN (Taxpayer ID Number) in account section.
- can sign contracts only for vehicles owned by their company.
##### Agents:
Agents represent insurance companies.
- must have their license number recorded in the system.
- have access to **view contracts** signed with their company. access may vary based on **privileges**.
- can sign contracts for all vehicles.

| ***Privilege*** | ***Access Type***                                         |
| --------------- | --------------------------------------------------------- |
| VIEW_ALL        | view all contracts with their ins. company                |
| VIEW_OWN        | view contracts with their ins. company **signed by them** |
#### Contract Details:
##### Contract contains:
- start date
- end date
- duration (1 week, 1 month, 3 months, 6 months, 1 year)
- purpose of vehicle use ("TAXI", "PERSONAL")
- calculated contract price determined by the insurance company (currently, insurance prices are regulated in Armenia, and they are consistent across all insurance companies).

##### Price Calculation:
> [!WARNING]  Price calculation is based on the following formula; however, it's important to acknowledge that laws and policies may evolve in the coming years:

$$
PRICE\ =\ BM\ coef\ *\ purpose\ coef\ *\ vehicle\ production\ year\ coef\ *\ BASE\_PRICE
$$

Where
	BASE_PRICE = 41,000 AMD (but it may be subject to change in the future).
	BM coefficient is based on the BM class (1 to 22).

##### Additional details:
- only one contract can exist for a given period for a particular vehicle.
### Other
- Tailored to align with the existing laws and policies in Armenia. Multiple countries in the future
