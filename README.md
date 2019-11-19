# Rental domain ER model
This diagram illustrates a simple rental domain model and entities relationship. 
Diagram was created using [erd](https://github.com/BurntSushi/erd) framework

## Cases covered
* A landlord can rent out a separate apartment, the whole building or several apartments to another party. 
* A landlord can sign a rental contract with one or multiple tenants. 
* One tenant can rent multiple apartments from the same landlord. 
* One tenant can rent multiple apartments simultaneously. 
* A landlord can also be a tenant of another landlord. 

## Further assumptions
* A property may have only one landlord
* Buildings with multiple appartments may exist
* Single landlord may have several properties owned
* A contract describes rental only for one property

## TODO
* A property may have multiple landlords, so we can introduce a Title Deed entity which describes all landlords' relationship to one property
* Each contract has terms, but who watches over their execution? We may introduce a Regulator role
* There is a space to think about signing the contract procedure. How many signers is enough? How contract becomes active after being signed? How signature is being confirmed? 
