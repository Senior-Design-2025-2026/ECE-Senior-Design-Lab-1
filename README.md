# ECE-Senior-Design-Lab-1
ECE:4880 – Senior Design 1 at the University of Iowa tasked our team with creating a robust smart thermometer that has internet connectivity and user-friendly functionality.

Our solution provides an easy way for users to view temperature data physically on our box or remotely from a computer.

There are multiple input controls used within the system, such as switches and buttons, along with cable connectors to remove sensors when there is no need for use.

The user receives feedback via an OLED screen, and virtually all data is uploaded to the web.

Authors:
- [Steven Austin]()
- [Zack Mulholland](https://www.linkedin.com/in/zack-mulholland-317914254/)
- [Sage Marks](https://www.linkedin.com/in/sage-marks/)
- [Matthew Krueger](https://www.linkedin.com/in/mattnkrueger/)

## System Architecture
<div align="center">
  <img src="img/image-5.png" alt="System Architecture" width="800">
  <div><em>Figure 1. System Architecture</em></div>
</div>

## Raspberry Pi Pin-Out Diagram
<div align="center">
  <img src="img/image-3.png" alt="Raspberry Pi Pin-Out Diagram" width="800">
  <div><em>Figure 2. Raspberry Pi Pin-Out Diagram</em></div>
</div>

## Finished Product
<div align="center">
  <img src="img/image-10.png" alt="Finished Product - Additional View" width="800">
  <div><em>Embedded System</em></div>
  <br>
</div>

<div align="center">
  <img src="img/image-6.png" alt="Finished Product - Additional View" width="800">
  <div><em>Embedded System + Web Application</em></div>
</div>

## Source Code
**Embedded System:**  
  - [L1-EXTENSION-embedded-thermostat](https://github.com/Senior-Design-2025-2026/L1-EXTENSION-embedded-system)

**Software Application:**
  - Web Application  
    - [L1-EXTENSION-web-application](https://github.com/Senior-Design-2025-2026/L1-EXTENSION-web-application)  
  - Streamer API  
    - [l1-EXTENSION-stream-writer](https://github.com/Senior-Design-2025-2026/L1-EXTENSION-stream-writer)  
  - Asynchronous Task Queue  
    - [L1-EXTENSION-celery-worker](https://github.com/Senior-Design-2025-2026/L1-EXTENSION-celery-worker)  
  - Sqlalchemy ORM  
    - [L1-EXTENSION-postgres-orm](https://github.com/Senior-Design-2025-2026/L1-EXTENSION-postgres-orm)

# Running the Project
We cannot share our physical box, but we can share all you need to run the project in a dummy environment :)

## Prerequisites
This repository contains submodules which must be initialized.

After pulling this repository, run the following command:
```
git submodule update --recursive --init
```

You must also have Docker installed on your computer to spin up the application locally. Please read the [Docker documentation](https://docs.docker.com/) on how to get started.

<div align="center">
  <img src="img/image-7.png" alt="Finished Product - Additional View" width="800">
  <div><em>Running Project</em></div>
</div>

## Starting Docker Containers:
After initializing the submodules and downloading Docker, simply run the command:
```
docker compose up
```

## Viewing the Dashboard
Running the container will expose port 8000 which your mobile device can connect to. 

Within your mobile browser, enter the path:
```
<IP>:8000
```

To find your devices IP, use the following command:

MacOS: $ ipconfig getifaddr en0

Linux: $ ip addr show

Windows: $ ipconfig
