# Moken (Decentralized airbnb)
## ZENCON Hackathon 2023
## [Trailer]()

![Moken Mockup](https://github.com/Moken-DApp-Zeniq/.github/assets/99221221/3620b42d-4aea-4054-abbd-c34ac5377805)

## Our solution
The real estate market, despite its established status, faces a series of challenges that directly impact efficiency, transparency, and the costs of real estate transactions.

One of the most apparent problems is the lack of efficiency that permeates the entire process. The absence of innovation results in slow and bureaucratic processes, making access to properties more time-consuming and complex than it should be. Furthermore, the excessive presence of intermediaries in the transaction cycle exacerbates this scenario. The large number of agents involved makes the process even more complicated and costly, contributing to the lack of efficiency and the opacity that often surrounds transactions.

To overcome these challenges, we introduce Moken, an innovative solution that provides access to properties for a specified period, leveraging blockchain and IoT (Internet of Things) technologies. The approach is straightforward: property owners register their properties on the Moken platform and generate utility tokens. When users acquire these tokens, they gain access to the property for the specified time, and after that period, the token automatically expires.

Additionally, properties registered on the platform are equipped with an IoT system in the door lock that includes a microcontroller and an RFID reader. To access the property, users simply bring the Zeniq card close to the lock, ensuring easy entry, complete transparency, and maximum security.

Moken aims to revolutionize the real estate market by eliminating deeply-rooted inefficiencies, increasing transparency, and substantially reducing costs, offering a more efficient, cost-effective, and advantageous real estate experience for all parties involved. #YourTraverYourRules

## Our repositories

Each repository contains instructions on how to run the code and specific informations.
- frontend: Contains the code related to the application's frontend.
- backend: Repository for the mqtt pubilsher/subscriber scheme that the iot will use to communicate with the blockchain
- foundry: Contains code for the created contracts.
- hardware: The code that has being used in the hardware device

## Architecture

![Architeture (1)](https://github.com/Moken-DApp-Zeniq/.github/assets/99221221/ccd2bd74-e0ab-4870-95d8-648aac435a93)

To communicate with IoT devices, a protocol called MQTT is used. The MQTT, or Message Queuing Telemetry Transport, is a communication protocol designed for efficient data transmission between devices, particularly in the context of the Internet of Things (IoT). It operates on the principles of simplicity, reliability, and scalability.

At its core, MQTT follows a client-server architecture. The participants in MQTT communication include:

MQTT Broker: This is the central hub of MQTT communication. It acts as a server, receiving and distributing messages between clients. The broker ensures that messages are delivered efficiently to the intended recipients.

MQTT Clients: These are the devices or applications that want to exchange data. Clients can either publish messages to specific topics or subscribe to topics to receive messages.

The workflow of MQTT can be summarized as follows:

Publishing Messages: A client (referred to as the publisher) generates data that it wants to share with other clients. It formats this data into a message and associates it with a topic. A topic acts as a label or channel to categorize messages. The publisher sends the message, including the topic, to the MQTT broker.

Subscribing to Topics: Another client (referred to as the subscriber) expresses interest in certain topics and informs the MQTT broker of its subscriptions. The broker maintains a record of which clients are subscribed to which topics.

Message Distribution: When a publisher sends a message to the MQTT broker, the broker examines the topic associated with the message. It then checks its list of subscribers for that topic and delivers the message to all interested subscribers. This process ensures that data is efficiently routed to the right recipients.


In summary, MQTT is a lightweight, efficient, and reliable protocol for facilitating communication between devices, making it ideal for IoT applications. Its use of topics, quality of service levels, and message distribution through a central broker simplifies data exchange and enhances scalability while minimizing network overhead.

### Hardware documentation

#### Photo
![hardware_moken](https://github.com/Moken-DApp-Zeniq/.github/assets/99221221/c1f456e6-17b6-4848-a434-9519500c1bbe)
