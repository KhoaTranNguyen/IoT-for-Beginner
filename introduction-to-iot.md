# Introduction to IoT

## What is the 'IoT'?

- Was coined by Kevin Ahston (Who is he?) in 1999
- Describe any device that interacts with the physical world around it:
    1. Via sensors (gathering data)
    2. Via actuators: real-world interactions (e.g turn on switch or light)

## Devices
- Usually custom-made (circut, processors, etc.) -> meet the needs of a particular task.
- Developer kit: general-purpose IoT devices for developer, often with features that you couldn't have on a production device:
    * A set of external pins for sensors and actuators connection
    * Debug supported hardware
    * Addtional resources (add unnecessary cost when doing large manufacturing run)

    💁 Your phone can also be considered to be a general-purpose IoT device:
    * With sensors and actuators built-in
    * With different apps using the sensors and actuators in different ways with different cloud services.

    #### I. Microcontrollers:
    - Microcontrollers unit (MCU), a small computer consisting of:
        * One or more central processing units (CPU)
        * Memory (RAM and program memory)
        * Programmable input/output connections (I/O) - for sensors and actuators
    - Low cost computer devices
    - Limited number of very specific tasks. Can't connect a moniter, keyboard or mouse and use them for general-purpose tasks.
    - Usually come with:
        * Additional sensors and actuators
        * Additional microcontrollers on the board
        * One or more LEDs
        * Standard plugs for adding more sens and act
        * Built-in wireless connectivity
    - Usually programmed in C/C++
    - Example kit: **Adruino, Wio Terminal**

    #### II. Single-board computers
    - Small computing device that has all elements of a complete computer contained on a single small board
    - Have specifications close to a desktop or laptop PC or Mac, i.e run a full operating system but:
        * Are small
        * Use less power
        * Cheaper
    - Programmed in any language. IoT devices are typically in Python.
    - Example kit: **Raspberry Pi 4, Raspberry Pi OS, Remote SSH extension**

    #### III. Virtual single-board computer
    - It runs on your PC or MAc
    - Use a tool to:
        * Simulate hardware providing sensor values
        * Showing the results of actuators on screen 

## Cloud-based services:
- Process sensor data
- Send requests to actuators (that connected to IoT devices)
- Edge devices (don't have or don't need Internet):
    * Process & respond to sensor data themselves (using AI models trained in the cloud?)

## Aplication of IoT
- IoT covers a huge range of use cases, across a few broad groups:
    * Consumer IoT
    * Commercial IoT
    * Industrial IoT
    * Infrastructure IoT

    #### Consumer IoT
    - IoT devices that consumer will buy and use around their home
    - Incredibly useful: Smart speakers, smart heating systems, robotic vacuum cleaners and health monitor
    - Not sure: voice-controlled taps, cannot turn off as the voice controller cannot hear you over the sound of running water :v
    - Empowering people, especially who have a disability
    - Becoming so ubiquitous, even young children are using as a part of their daily lives.

    #### Commercial IoT
    - Commercial IoT covers the use in the workplace
    - Example:
        * Office setting: Manage lighting and heating to reduce cost and carbon emissions
        * Factory: Monitor for safety hazards
            + Workers don't wearing hard hats
            + Noise has reached dangerous levels
        * Retail: Measure the temperature of cold storage
            + Altering shop owner if a fridge or freezer is outside the required temperature range
            + Monitor items on shelves to direct employees to refill produce that has been sold
        * Transport industry: Monitor vehicle locations
            + Track on-road mileage for road user charging
            + Track driver hours and break compliance
            + Notify staff when a vehicle is approaching a deopt to prepare for unloading or unloading
        
    #### Industrial IoT
    - Use of IoT devices to control and manage machinery on a large scale, from factory to digital agriculture
    - Factory:
        * Monitored machinery: track temperature, vibration and roation speed
            -> Allow the machine to stop if it goes outside a certain of tolerances (too hot -> get shut down)
        * This data can be analyzed over time to do predictive maintenance
    - Digital Agriculture:
        * Monitoring temperatures and using **Growing degree days** to predict when a crop will be ready for harvest.
        * Connect soil moisture monitoring to automated watering systems.
        * Using drone, satellite data and AI to monitor growth crop, disease and soil quality over huge areas of framland.

    #### Infrastructure IoT
    - Is monitoring and controlling local and global infrastructure that people use every day
    - **Smart Cities**:
        * Urban areas that use IoT devices to gather data about the city and use that to improve how the city runs.
        * Cities are usually run with collaborations between local governments - academia - local businesses to track and mange things from transport to parking and pollution.
    - **Smart power grids**
        * Allow better analyics of power demand by gathering usage data at the level of individual homes.
        * Guide decisions including where to build new power stations (country level)
        * Giving insights into how much power they are using, when they are using it, suggest to reduce costs (personal level).

## Data
- Data is the key to IoT's success. To be a successful IoT developer:
    1. Understand the data you need to gather
    2. How to gather it
    3. How to make decisions based on it
    4. How to use those decisions to interact with physical world (if needed)

## Examples of IoT devices around you
* Multiple smart speakers
* Fridge, dishwaher
* Oven, microwave
* Smart plugs
* Lights
* Electricity monitor for solar panels
* Video doorbell and security cameras
* Smart thermostat with multiple smart room sensors
* Home entertainment systems and voice-controlled TVs
* Fitness and health trackers
* Garage door opener