
# Mission Reflection

This laboratory activity helped me understand why containerization is becoming an important part of cloud-native computing. Before doing the activity, I mainly understood a Virtual Machine as a computer running inside another computer. After using Docker, I learned that containers work differently because they share the host operating system kernel instead of requiring a complete guest operating system. Because of this, starting a container can be much faster than installing and booting an operating system on a Virtual Machine. In the KillerCoda environment, I was able to pull and run an Nginx image with only a few Docker commands.

The port mapping `-p 8080:80` was also an important concept that I learned. The Nginx application listens on port 80 inside the container, but I needed a way to access it from the host environment. Mapping port 8080 on the host to port 80 inside the container allowed me to send a request using `curl http://localhost:8080` and receive the Nginx welcome page.

I also learned that removing a container using `docker rm` removes the container itself and its writable container filesystem. Important data should therefore be stored using appropriate persistent storage such as Docker volumes when it needs to survive container removal.

Containerization can also improve collaboration between developers and IT operations teams. Developers can package an application together with its required environment, while operations teams can deploy the same container in different environments. This supports more consistent workflows and is an important concept in DevOps.

Finally, my GitHub portfolio is evolving from simple documentation into a collection of practical cloud computing activities. Each laboratory adds new technical skills, commands, screenshots, and explanations that demonstrate my progress and understanding.
