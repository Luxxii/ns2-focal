# NS3 on Ubuntu 20.04 / Focal

Here i provide a container which has a functioning NS3-build on Ubuntu.

This is very similar to [ns3-bionic](https://github.com/Luxxii/ns3-bionic).

I have updated the script, since Ubuntu 20.04 has been released this year. So here we go again!

## Usage

It can be used easily like: 

> docker run "NS3_IMAGE" "./waf --run hello-simulator"


Even debugging is possible:
> `docker run -it "NS3_IMAGE" "./waf --run=hello-simulator --command-template=\"gdb %s --args <args> \""`


Modify this image or provide the source via `-v` to run your own simulations.