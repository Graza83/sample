%%%MetaData
status: Draft
version: 1.0
author: Amin Mohammed-Coleman <amin.mohammed-coleman@digital.cabinet-office.gov.uk>
description: Example Service Definition 
lastUpdated: 10/09/2014
type: component
department: GDS
%%%


# People Look Up Service

Example People look up service.

Test business service.

# Context


# Components

The following components where used to build this example service
%%%Component
name: Dao Component
description: Used for Database interaction
link: ../services/daoComponent
%%%  
%%%Component
name: PaymentService
link: ../services/paymentComponent
%%%

# Services

The following section defines the other services used in order to perform the required business function.

%%%Service
name: PaymentService
link: ../../services/PaymentService
%%%

# Transactions
In order to fulfil the requirements of the business service, our service has to perform interaction with multiple other services. The following shows how my example service interacts with the other services defined in this architecture document.
%%%sequence
MyService->PeopleLookUpService: Find Person
Note right of PeopleLookUpService: PeopleLookUpService performs a look up
PeopleLookUpService-->MyService: Returns an individual
MyService->>PeopleLookUpService: Confirmation.
%%%


# Further Reading

Test	

