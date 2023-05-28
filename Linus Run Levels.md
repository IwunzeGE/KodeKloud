# LINUX RUN LEVELS

New tools were installed on the app server in a Datacenter. Some of these tools can only be managed from the graphical user interface. Therefore, there are requirements for these app servers. On all App servers in the Datacenter change the default runlevel so that they can boot in GUI (graphical user interface) by default.

## Procedures

1. At first login on all app servers  & Switch to  root user

![1](https://github.com/IwunzeGE/KodeKloud/assets/110903886/3afb8866-30b1-4bea-8c7b-c9427e433318)

2. Check the default run level using `systemctl get-default`.

![2](https://github.com/IwunzeGE/KodeKloud/assets/110903886/45e7e3ba-3919-44d0-a22f-5affbc030393)

3. Change the run level to graphical interface using `systemctl set-default graphical.target` and start the service using `systemctl start graphical.target`

![3](https://github.com/IwunzeGE/KodeKloud/assets/110903886/c838f5d4-d96c-48fb-8b32-d6cf5b3f3aa1)


