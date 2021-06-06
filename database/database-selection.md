# Database selection
We can select distributed database on the basis of CAP theorem
## CAP 
```Consistency Availability Partition tolerance```
- Consistency : All nodes should have same value
- Availability : Every request will get the response
- Partition tolerance : System should able to work if network goes down between two nodes

![Image CAP theorem](https://github.com/impradeeparya/system-design/blob/main/database/cap.png)


## RDBMS default configuration
- [x] Consistency 
- [x] Availability
- [ ] Partition tolerance

![Image CA](https://github.com/impradeeparya/system-design/blob/main/database/ca.png)


## RDBMS with failover
- [ ] Consistency 
- [x] Availability
- [x] Partition tolerance

![Image AP with failover](https://github.com/impradeeparya/system-design/blob/main/database/ap-with-failover.png)


## Mongo DB default configuration
1. Primary secondary node configuration.
2. Read/Write operation will be on primary node only.
3. Data replication will be from primary node to secondary node.
4. In case of primary goes down, system will be unavailable until new leader comes up.

- [x] Consistency
- [ ] Availability
- [x] Partition tolerance
![Image CP](https://github.com/impradeeparya/system-design/blob/main/database/cp.png)


## Mongo DB custom configuration
1. Primary secondary node configuration.
2. Write operation will be on primary node only
3. Read opertaion will be on both primary and secondary node.
4. Data replication will be from primary node to secondary node.
5. Consistency will be eventual.

- [ ] Consistency
- [x] Availability
- [x] Partition tolerance


## Cassandra
- [ ] Conistency
- [x] Availablity
- [x] Partition tolerance
