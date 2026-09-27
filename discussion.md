## DJI Tello Drone Connection and Edge AI

The DJI Tello drone project is a simple way to learn how software can communicate with a real physical device. Even though the first program only connects to the drone and checks the battery level, it introduces several ideas that are important in Edge AI, including wireless communication, device control, sensor data, and local processing.

The DJI Tello is a small programmable drone that can connect directly to a laptop through Wi-Fi. In this setup, the drone creates its own wireless network. The laptop connects to that network, and Python code is then used to communicate with the drone.

This is a good example of an edge computing setup because the laptop and the drone can communicate directly without depending on a remote cloud server. The computing happens close to the device itself. In many Edge AI systems, this is useful because it can reduce delay and allow the system to continue working even when Internet access is limited or unavailable.

The first goal of the assignment is to establish a connection between the Python program and the drone. The sample program creates a Tello object, connects to the drone, and asks for the current battery level.

At first, this may look like a very basic program. However, several things must work correctly for the battery percentage to appear. The laptop must be connected to the Tello Wi-Fi network. Python must have the correct package installed. The operating system must allow the program to communicate through the network. The drone also has to be powered on and ready to receive commands.

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