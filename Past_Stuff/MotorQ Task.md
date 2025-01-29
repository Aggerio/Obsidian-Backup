
Vin ---> 17 digit alpha numeric string 

Org --> 

name,  --> primary key alphaNumeric 
account --> varchar()
website --> varchar
fuel Reimbursement policy  --> default 1000
speed Limit policy 
parent org --> either name org foreign key or NULL
child org --> csv, name org can be multiple

Vehicle --> 
vin --> 17 digit alpha numeric string 
orgId --> OrgId foreign key Org


ENDPOINTS TO BE IMPLEMENTED --> 


**GET /vehicles/decode/:vin** --> DONE with bonus 

**POST /vehicles** --> DONE with bonus 

**GET /vehicles/:vin** --> DONE with bonus
 
**POST /Orgs** --> DONE with bonus

**PATCH /orgs** --> DONE with bonus

**GET /orgs** --> DONE with bonus

