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
3. Cab finder service
  - help user to get cab for given latitude and longitute
  - interact with location service to get user location and drives near by
  - interact with trip service to update trip infromation
4. Location service
  - manage information about drive and drive location
  - helps to find location on the basis of latituted and longitute
5. Cab request service
  - helps customer to initiate process of cab booking on the basis of source and destination
6. Trip service
  - manages information about customer trips
  - use SQL to store information for transactional data consistency
  - use non SQL to provide historic data about trips
7. Payment service
  - handle information about payments done for the trips 
  - Use SQL to store all the information
