# runPHI: A Container RUNtime for Partitioning Hypervisor Integration

<p align="center">
<img src="https://github.com/runphi/runphi_manager/blob/main/logo/runphi_logo_lowres.jpg" width="100">
</p>
----

#### Authors: Marco Barletta, Francesco Boccola, Daniele Ottaviano, Luigi De Simone & other members of DESSERT lab UniNa
#### Università degli Studi di Napoli Federico II
#### marco.barletta@unina.it, francesco.boccola@unina.it
----

runPHI is a container RUNtime for Partitioning Hypervisor Integration. 
What that means? A container runtime is whatever seats below your containerd, docker, or kubelet, and is the tiny program in charge of setting up kernel stuff to start a container.

runPHI does something similar, but with partitioning hypervisors, which are hypervisors designed for industrial scenarios with critical requirements in mind.

runPHI allows you to take your favourite Zephyr, FreeRTOS, or even bare metal code, running on industrial hardware platforms (INCLUDING RPUs!!!!!) and integrate it with your container orchestration system (e.g., Kubernetes).
We call this isolated container ZICs (Zero-Interference Containers).

Why that? We envision an industrial cloud in which critical applications are seamlessly managed along with normal Linux containers, with the same flexbility, allowing you to define the number of replicas, deploying them across a large cluster, while keeping a high standards of non-functional requirements. 

runPHI is OCI compliant (at least, for basic calls like start, stop, kill, and delete). The runtime is still an academic research project, if you have any suggestion to improve it (or even better, you want to contribute!!!) please reach at the emails above.
