# HackItAll_Contest_App

Application: File Manager

Description:

In the IoT world, it helps to be able to manage a multitude of Edge devices from a central point.
The idea of the application is to have a frontend and a backend to manage the filesystem of multiple devices.
On each device, there would be an agent (also built by us), which would communicate with the backend, to get/set the required information.

Objective:

Create an web application that is able to manage the filesystem of multiple devices.
Operations that must be included:
- list files and folders
- view file contents
- search for files/folders
- create new file/folder
- copy files to/from the machine
- list processes
- sort processes by cpu/ram
- view files in a continuous pipeline (similar to tail -f)

Architecture:

- frontend for the above operations
- backend
- an agent component (will run on the machines and communicate with the backend)

Basically, the flow would be:

- the frontend requires something (list files, create file etc.)
- the backend receives the information
- the backend tells the agent what it wants (how it does that it is up to you)
- the agent gets or sets the information required by the backend
- the agent sends back to the backend the response (again the how is up to you)
- the backend tells the frontend the response
- the frontend shows the user the response in the UI

![HackItAll](https://user-images.githubusercontent.com/100564136/163218010-1671237f-48ee-45af-aede-cdeac341bbe5.png)

