# SmartBracelet

In this repository we put all the code of the IoT project of the course of Politecnico di Milano about "Smart Bracelet".


In this Project we implemented a software using TinyOs and NodeRed.

This software is applied on smart bracelets, which are worn by children and their parents (2 couples), and help parents to keep track of the child's position. When the child goes beyond a communication ratio, an alert notifies the respective parent.

For the simulation we have used Cooja, making sure that every part of the code fulfills the project tasks. According to these tasks the operation of the smart bracelet couple has three modes:
1. **Pairing mode**: Is the phase where the parent's and child's bracelet broadcast a 20 byte random key. After the pairing a message is transmitted to the parent and the communication moves to the next step.
2. **Operation mode**: Has to do with the messages transmitted periodically from the child to the respective parent. These messages contain information about the position of the child and the kinematic status (that can be STANDING 3 WALKING 4 RUNNING 5 or FALLING 6).
3. **Alert mode**: In case of the kinematic status being a FALLING message the parent's bracelet sends a fall alarm. If the parent does not receive any message within a minute, a MISSING alarm is sent.

Each file making the simulation possible is explained in the [**project report**](https://github.com/Rkomi98/SmartBracelet/blob/help/Project_Report.pdf) and the log file is the [simulation.txt](https://github.com/Rkomi98/SmartBracelet/blob/help/simulation.txt) file.

All the simulation is performed in Cooja and it is connected with NodeRed. You can find the code in the file ["NodeRed_Simulation.txt"](https://github.com/Rkomi98/SmartBracelet/blob/help/NodeRed_Simulation.txt).

> It is important to enable the serial port from the settings of the Virtual Machine
![immagine](https://user-images.githubusercontent.com/72648197/187158088-8b16f126-237e-4ded-90c7-69a36eeab314.png)



To see how the simulation works you can download the video provided in this repository, named ["Simulazione.mp4"](https://github.com/Rkomi98/SmartBracelet/blob/help/Simulazione.mp4).



