### Chat service

## Functional requirement
1. One to one chat
2. Group chat
3. Text message
4. Image
5. Last seen
6. Read receipt


## Non functional requirement
1. High availablity
2. Low latency
3. Highly scalable

## Services
1. Message service
    - Handles messages flow
    - Store messages in DB
2. Group service
    - Handles group message flow
3. Resource service
    - Handles image messages
    - Store image
4. User service
    - Manage user data
    - Store user information in RDBMS
5. User activity service
    - Store information about user last seen
    - Handles high writes


## Design
![Image](https://github.com/impradeeparya/system-design/blob/main/chat-service/chat-service.png)
