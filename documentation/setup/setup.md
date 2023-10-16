# Setup the lab environment

For this lab, we will use a virtual machine running Ubuntu Server which will
come preconfigured for us.

We have to make sure that the virtual machine has a bridged network adapter
so that it can be accessed from the host machine. We also have to make sure
that the virtual machine has a static IP address so that we can always access
it from the same address.

Ubuntu Server does not come with a graphical user interface (GUI) by default,
so we will need to use the command line to interact with it. This is a great
opportunity to deepen your knowledge of the Linux command line.

As virtual machines are not the focus of this lab, we will not go into details
on how to set them up. If you are not familiar with virtual machines, you can
find a lot of resources online.

As performance on virtual machines can be quite poor, it is recommended to
ssh into the virtual machine from your host machine. This will allow you to
use your host machine's terminal to interact with the virtual machine.

```bash
ssh <username>@<ip-address>
``` 

Once you are connected to the virtual machine, verify that your system is
indeed Ubuntu Server.

```bash
lsb_release -a
```

Make sure docker is installed on the virtual machine.

```bash
docker --version
```

Make sure docker-compose is installed on the virtual machine.

```bash
docker-compose --version
```

Make sure git is installed on the virtual machine.

```bash
git --version
```

And clone the lab repository (Make sure to clone it in your home directory).

```bash
git clone https://github.com/tinitiuset/lab-grafana.git
```

If these checks succeed, you are ready to start the lab.
