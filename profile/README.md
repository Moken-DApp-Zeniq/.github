# Moken (Decentralized airbnb)
## ZENCON Hackathon 2023
## [Trailer]()

![Moken Mockup](https://github.com/Moken-DApp-Zeniq/.github/assets/99221221/3620b42d-4aea-4054-abbd-c34ac5377805)

## Our solution
🏡🚀 The real estate market, despite its long-standing presence, is grappling with a set of pressing challenges that significantly impact efficiency, transparency, and the financial aspects of real estate transactions. 😟

One glaring issue that plagues the industry is the painful lack of efficiency that permeates every step of the process. 😩 The absence of innovation has led to painfully slow and bureaucratic procedures, turning property access into a time-consuming and labyrinthine ordeal. 😓 But wait, there's more! The excessive presence of intermediaries in the transaction cycle only compounds this problem, making the process even more costly. 😵

But fear not! We're here to introduce you to Moken, a groundbreaking solution that promises to revolutionize the real estate game! 🌟 Moken leverages **cutting-edge blockchain and IoT (Internet of Things)** technologies to provide an elegant solution to these woes. 🚀

Here's how it works: Property owners register their properties on the Moken platform and generate **utility tokens**. 🏠💰 When users acquire these tokens, they gain access to the property for a specified period, and like magic, the token expires after that timeframe. 🕒✨

But wait, there's more! Properties registered on the platform are equipped with a **state-of-the-art IoT system integrated into the door lock**, featuring a nifty microcontroller and an RFID reader. 📡🚪 Accessing the property is as simple as waving your **ZenPass** near the lock, ensuring seamless entry, unparalleled transparency, and top-notch security. 🔐🤩

Moken's mission is clear: to disrupt the real estate market by obliterating deeply-rooted inefficiencies, boosting transparency, and significantly slashing costs. Say goodbye to the old, cumbersome ways and hello to a more efficient, cost-effective, and rewarding real estate experience for everyone involved. 🙌🏡 

#YourJourneyYourRules 🚀💎

## Our repositories

Each repository contains instructions on how to run the code and specific informations.
- frontend: Contains the code related to the application's frontend.
- backend: Repository for the mqtt pubilsher/subscriber scheme that the iot will use to communicate with the blockchain
- foundry: Contains code for the created contracts.
- hardware: The code that has being used in the hardware device

## Architecture

![Architeture (1)](https://github.com/Moken-DApp-Zeniq/.github/assets/99221221/ccd2bd74-e0ab-4870-95d8-648aac435a93)

## Hardware documentation

To communicate with IoT devices, a protocol called MQTT is used. The MQTT, or Message Queuing Telemetry Transport, is a communication protocol designed for efficient data transmission between devices, particularly in the context of the Internet of Things (IoT). It operates on the principles of simplicity, reliability, and scalability.

At its core, MQTT follows a client-server architecture. The participants in MQTT communication include:

MQTT Broker: This is the central hub of MQTT communication. It acts as a server, receiving and distributing messages between clients. The broker ensures that messages are delivered efficiently to the intended recipients.

MQTT Clients: These are the devices or applications that want to exchange data. Clients can either publish messages to specific topics or subscribe to topics to receive messages.

The workflow of MQTT can be summarized as follows:

Publishing Messages: A client (referred to as the publisher) generates data that it wants to share with other clients. It formats this data into a message and associates it with a topic. A topic acts as a label or channel to categorize messages. The publisher sends the message, including the topic, to the MQTT broker.

Subscribing to Topics: Another client (referred to as the subscriber) expresses interest in certain topics and informs the MQTT broker of its subscriptions. The broker maintains a record of which clients are subscribed to which topics.

Message Distribution: When a publisher sends a message to the MQTT broker, the broker examines the topic associated with the message. It then checks its list of subscribers for that topic and delivers the message to all interested subscribers. This process ensures that data is efficiently routed to the right recipients.


In summary, MQTT is a lightweight, efficient, and reliable protocol for facilitating communication between devices, making it ideal for IoT applications. Its use of topics, quality of service levels, and message distribution through a central broker simplifies data exchange and enhances scalability while minimizing network overhead.

### Photo
![hardware_moken](https://github.com/Moken-DApp-Zeniq/.github/assets/99221221/c1f456e6-17b6-4848-a434-9519500c1bbe)
