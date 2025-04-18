<p>
  <img src="https://github.com/runphi/runphi_manager/blob/main/logo/runphi_logo_lowres.jpg" width="80" align="left">
  <h2>runPHI: A Container RUNtime for Partitioning Hypervisor Integration</h1>
</p>

#### Authors

Marco Barletta, Francesco Boccola, Daniele Ottaviano, Luigi De Simone & other members of [DESSERT group](https://dessert.unina.it) at [DIETI](www.dieti.unina.it), Università degli Studi di Napoli Federico II

----

**runPHI** is a container RUNtime for Partitioning Hypervisor Integration. 
What that means? A container runtime is whatever seats below your containerd, docker, or kubelet, and is the tiny program in charge of setting up kernel stuff to start a container.

runPHI does something similar, but with partitioning hypervisors, which are hypervisors designed for industrial scenarios with critical requirements in mind.

runPHI allows you to take your favourite Zephyr, FreeRTOS, or even bare metal code, running on industrial hardware platforms (INCLUDING RPUs!!!!!) and integrate it with your container orchestration system (e.g., Kubernetes).
We call this isolated container **Zero-Interference Containers** (ZICs).

<p align="center">
  <img src="https://github.com/runphi/.github/blob/main/imgs/runphi_zic.png" width="50%">
</p>


Why that? We envision an industrial cloud in which critical applications are seamlessly managed along with normal Linux containers, with the same flexibility. You can define the number of replicas and deploy them across a large cluster while keeping high standards of non-functional requirements. 

runPHI is OCI compliant (at least, for basic calls like start, stop, kill, and delete). The runtime is still an academic research project. If you have any suggestions to improve it (or even better, you want to contribute!!!), please contact this [email](mailto:runphi.dessert.unina@gmail.com).
