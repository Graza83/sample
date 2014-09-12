%%%MetaData
status: Draft
version: 0.2
author: Amin Mohammed-Coleman <amin.mohammed-coleman@digital.cabinet-office.gov.uk>
description: Example Service Definition 
lastUpdated: 10/09/2014
%%%


# People Look Up Service

Example People look up service.

Test business service.

# Context


# Components

The following components where used to build this example service
    - name: component one
      description:
        Here I describe the component one in some detail. It should
        perhaps be snapped out as a separate element?        
	- name: component two
	  description:
	   	Here I describe the component one in some detail. It should
	    perhaps be snapped out as a separate element?        
	- name: component three
	  description:
		Here I describe the component one in some detail. It should
		perhaps be snapped out as a separate element?        
  

# Services

The following section defines the other services used in order to perform the required business function.

%%%Service
type: Service
name: PaymentService
link: ../../services/PaymentService
%%%

# Transactions
In order to fulfil the requirements of the business service, our service has to perform interaction with multiple other services. The following shows how my example service interacts with the other services defined in this architecture document.
%%%sequence
MyService->PeopleLookUpService: Find Person
Note right of PeopleLookUpService: PeopleLookUpService performs a look up
PeopleLookUpService-->MyService: Returns an individual
MyService->>PeopleLookUpService: Confirmation Required
%%%


# Further Reading

Test	

