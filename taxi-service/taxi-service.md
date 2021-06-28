### Functional Requirement
1. User account creation
2. User should able to see taxis
3. User should get ETA and price while booking taxi
4. User should able to book taxi
5. User should able to see taxi location
6. Fraud detection
7. Driver/User profiling


### Non functional Requirement
1. System should be highly available
2. Low taency
3. Scalable, estimating 5millions ride per day


### Services
1. User service 
    - manage user data
    - provide trip information by intracting with trip service
    - use SQL to store user data
2. Driver service
    - mange drive data
    - provide payment information by intracting with payment service
    - use SQL to store drive data
3. Taxi finder service
    - help user to get 
    for given latitude and longitute
    - interact with location service to get user location and drives near by
    - interact with trip service to update trip infromation
4. Location service
    - manage information about drive and drive location
    - helps to find location on the basis of latituted and longitute
5. Taxi request service
    - helps customer to initiate process of taxi booking on the basis of source and destination
    - fetch customer location by intracting with location servicce
    - fetch near area of cutomer location
    - fetch drivers present in those area
    - assign driver to customer
6. Trip service
    - manages information about customer trips
    - use SQL to store information for transactional data consistency
    - use non SQL to provide historic data about trips
7. Payment service
    - handle information about payments done for the trips 
    - Use SQL to store all the information


### Design diagram
![Image](https://github.com/impradeeparya/system-design/blob/main/taxi-service/taxi-service.png)
