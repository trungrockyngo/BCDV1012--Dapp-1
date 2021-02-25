This is the lab for designing the simple state machine of automobile (mostly car) accident claim and implementing the sufficient chaincode 
.....


### About Auto insurance claim 

+ File report to be made in 7 days 

+ Exhaustive info related to car accident 
- Your policy number
- Make, model, year, registration and licence plate number of the vehicle
- Driver’s name
- Licence number (if the driver was not the registered owner)
- Time date and location of the accident
- Injury descriptions
- Number of passengers involved
- Vehicle damage's description 
- Names and driver’s licence numbers of all drivers involved
- Names of insurance companies, and auto insurance policies of all drivers involved
- Name and badge number of the investigating officer – if the accident was reported to police


##### State diagram 

1. States - data

> States: ["**Accident**", "**Claim Submitted**", "**Claim coverage decision pending**", "**Coverage**"] 


2. Transitions - functions 

> Key Transitions: 
- FillInClaim(CarInfo[], Name, Address)
- SubmitClaim(Name)
- Incomplete(Name)
- Rejected(Name)
- Approved(Name, Phone)
- ReviewContract(Name)
- ClaimCoverageDeductibles(Name)
- ReviewPastCoverage(Name)

> Other functions: 
- CheckStatus(Name)
- UnderstandPossibleDeductibles(Name)
- ContactInsuranceComp(Name)

3. Roles 
- FillInClaim(...) - driver in accident 
- SubmitClaim(...) - driver in accident/car insurance agent 
- Incomplete(...) - system 
- Rejected(...) - claim adjuster 
- Approved(...) - claim adjuster 
- ReviewContract(...) - system/ claim adjuster
- ClaimCoverageDeductibles(...) - driver in accident/car insurance agent 
- ContactInsuranceComp(...) - driver



#### ![State diagram](https://github.com/trungrockyngo/BCDV1012--Dapp-1/blob/main/car-insurance-claim-lab/state-diagram.png?raw=true)
 

Original: 
https://lucid.app/lucidspark/invitations/accept/bdece8f3-019a-474d-b6cd-3b26c180597b


