# A deeper dive into IoT


## Components of IoT application
- *Internet* and *thing*

    ### The Thing
    - Device that can interact with physical world
    - Small, low-priced computers, running at low speeds and using low power
    - Interact with the physical world:
        * Use sensor to gather data from their surroundings
        * Controlling outputs or actuators to make physical changes
    - E.g: smart thermostat has
        (1) temperature sensor 
        (2) dial or touchscreen: means to set a desired temperature
        (2) connection to a heating or cooling system, which is turned on when the temperature detected is outside the range.

    ### The Internet
    - Consists of application IoT device can connect to send & receive data
    - Other applications that process data from IoT device and help make decision on what requests to send the actuators

    - Typical setup:
        IoT device
        ⇓ ⇑
        Cloud service
        (Security, Receiving messages, Sending message back)
        ⇓ ⇑
        Applications
        (Process or store sensor data, Use sensor data with data from other systems to make decisions) 
    
    - Doesn't always connect directly to Internet via WiFi or wired connections
    - Use mesh networking: Bluetooth
    - Connect via a hub device that has Internet connection

    - E.g: smart thermostat
        * connect using home WiFi to a cloud service running in the cloud
        * send temperature data -> cloud service -> written to a database
        * cloud service (know the desired temperature) -> send back to smart thermostat -> turn the heating system on or off

        Cloud + AI: use data from other sensors of other devices (occupancy sensors detect what rooms are in use, weather and calendar) to set the temperature.
    
    ## Edge Devices
    - Gateway devices run on your local network
    - Run oflline where Internet connectivity is not possible (e.g. ship, disaster area)
    - Keep data private