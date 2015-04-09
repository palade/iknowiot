# Basic Messaging Model 

**Messaging is implemented with a broker**: Participants send messages and broker delivers them to recipients

**Two main models**
  - **Point-to-Point**: Messages are delivered only once and held on a queue from which a consumer picks one at a time
  - **Publish/Subscribe**: Messages are broadcasted to many consumers at once

## Point-to-Point

- Queue is a destination that contains messages sent from a producer that awaits delivery to a designated consumer
- Messages are delivered **in-order**
- Guarantees that each message is processed only once

## Pub/Sub model
- Multiple consumers subscribe for messages
- Topics are used to send messages to one or more consumers
- **No guarantees**, that messages are sent in order
- **No guarantees**, that each message is processed only once