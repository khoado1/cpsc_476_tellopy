## DJI Tello Drone Connection and Edge AI

The Drone connect project is a simple way to interface software with hardware.  A real device, the DJI Tello Drone is connected by a piece of python code DroneConnect.py.  The relevant parts of is is that it is a great introduction into the world of Edge AI because it demonstrates mobile technolgies such as wireless communication, device control, sensor, and local processing on the drone.

The DJI Tello is a small drone that can be programmed against.  The laptop can connect to this drone via Wi-Fi.  The drone creates its own wireless network and the laptop connects to the drone via that network.  The code in DroneConnect.py can then be executed.

This is an excellent example of Edge AI and is a perfect start to working on projects that demonstrate Edge AI concepts and principles.  Since the drone is capable of creating its own network, there is no absolute reliance on a static Wi-Fi network that cannot be extended wherever a drone travels.  Instead the communication can be done because the drone hosts its own network.  This reduces delays and possible fatal disconnect or network unavailable scenarios.

One of the goals of this project is to, via Pyton establish a connection to the Tello drone.  Once the connection is established, anything can be done on the drone.  One thing that this project does is request for the drone to return the current battery level, a very useful piece of information for a drone.

The DroneConnect.py is deceptively simple but there are many things that must happen.  For imstance on the hardware side, the drone must be presently close by.  It must be able to establish and host a Wi-Fi network.  It must be powered sufficiently to run.  It cannot be in a state where it cannot receive commands.  On the software side, the operating system must be in a state that can actually run Python code.  The Python runtime must be present and running without much trouble.  It must be in a state where Python is not too old.  They DJITello library must be available for DronneConnect.py to run properly.  There can be no malfunction in the connection code via Wi-Fi.  The battery firmware has to function properly in order for the battery code to function.

Because of this, checking the battery level is actually a useful first test. If the program displays the battery percentage, it proves that communication is working in both directions. The computer successfully sends a request to the drone, and the drone sends information back.

This idea is common in many types of hardware projects. Before trying to perform complicated actions, it is usually better to test a very simple operation first. For example, before programming a drone to move, take off, or process camera data, it makes sense to first verify that the connection is working correctly.

The assignment also shows why working with hardware can be different from working with normal software. If a regular program fails, the problem is usually somewhere in the code or the data. With a drone, the code can be correct and the system can still fail because of the Wi-Fi connection, firewall settings, missing Python packages, or the physical device itself.

This is why debugging the program step by step can be helpful. Running the code in Visual Studio Code using debug mode makes it easier to see where a problem occurs. If Python cannot import the required package, that problem can be fixed before testing the network connection. If the program reaches the connection step and then fails, the problem may be related to Wi-Fi or firewall settings instead.

This kind of troubleshooting is an important skill in Edge AI because these systems usually involve several parts working together. There may be software, hardware, sensors, networks, and AI models all operating as one system. A problem in any one of these areas can affect the whole application.

The battery information returned by the Tello is also an example of telemetry. Telemetry is simply information sent from a device about its current condition or activity. A battery percentage is a simple form of telemetry. Other examples could include speed, height, direction, temperature, or sensor readings.

Telemetry becomes very important in intelligent systems because software can use this information to make decisions. For example, a drone program could check the battery level before taking off. If the battery is too low, the program could prevent the drone from flying. A more advanced system could monitor the battery continuously and decide to land automatically if the charge becomes too low.

This is where the project starts to connect more directly with Edge AI. A drone can collect information from the world using sensors and a camera. A nearby computer can then process that information and decide what should happen next.

For example, a future project could use the Tello's camera to detect objects. The drone could send video to a laptop, and an AI model on the laptop could examine the images. If the model detects a certain object, the software could respond by displaying a message, tracking the object, or sending a command back to the drone.

The important point is that the AI does not always have to run in the cloud. In an edge system, the processing can happen locally on a nearby computer or device. This can make the system respond faster because the data does not have to travel across the Internet to a remote server and back.

The Tello project therefore demonstrates a basic Edge AI workflow. The drone acts as the physical device. It collects information and communicates through Wi-Fi. The laptop provides the computing power. Python provides a convenient way to control the device and read information from it. More advanced AI techniques could later be added on top of this basic connection.

Another useful lesson from this project is that advanced systems are often built from very simple steps. A program that only reads the battery percentage may not seem impressive by itself, but it proves that the communication path between the computer and the drone is working. Once that connection is reliable, more complicated features can be added.

These features could include movement commands, camera access, image processing, object detection, or autonomous behavior. Each new feature depends on the basic connection working correctly first.

## Closing Thought

The DJI Tello project is a good introduction to Edge AI because it connects software concepts with a real physical device. The first program is simple, but it demonstrates an important idea: a computer can communicate directly with a nearby smart device, receive information from it, and eventually make decisions based on that information.

Checking the drone's battery level is only the first step. Once communication is established, the same basic setup can be expanded into more advanced projects involving sensors, cameras, AI models, and automated control. In that way, a small drone connection experiment can serve as a useful starting point for understanding how real-world Edge AI systems are built.