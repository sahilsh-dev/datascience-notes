YARN (Yet Another Resource Negotiator) is Hadoop's resource management layer. It enables multiple applications to run on a shared cluster, ensuring efficient resource utilization.

## Components of YARN

- **Resource Manager:** Manages cluster-wide resources.
- **Node Manager:** Monitors resource usage on individual nodes.
- **Application Master:** Coordinates a single application’s execution.
- **Containers:** Execute tasks with allocated resources. 

YARN receives job requests, negotiates resources through the Resource Manager, and assigns tasks to containers via the Node Managers, ensuring job completion efficiently.

![[Pasted image 20250206034420.png]]