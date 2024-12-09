# Repo for Entanglement Encoding
## Abstract
With the development of quantum communication technology, scientists believe that the quantum network is one of the most critical infrastructures in the future quantum era. However, entanglement degradation caused by noise is one of the most significant difficulties faced by quantum networks. In this paper, we qualitatively and quantitatively analyze the characteristics and shortcomings of Quantum Error Correction (QEC) and Entanglement Purification (EP), two mainstream schemes for resisting entanglement degradation. QEC takes qubits as basic coding units to achieve high noise resistance,  but the resource requirement is enormous. EP uses simple quantum gates to improve entanglement fidelity to resist noise, but the effect is not as significant as QEC. Therefore, we explore a new scheme called Entanglement Encoding (EE) to resist entanglement degradation. The core idea of EE is to use physical entanglements as basic coding units to realize highly robust logical entanglement to resist noise. We theoretically demonstrate the feasibility of EE while discussing its scalability, quantum gate error tolerance, effectiveness, limitations, and potential. Moreover, we propose EE-based Entanglement Distribution (EEBED), which can guarantee obtaining valid long-distance entanglement. The simulation experiment shows that the noise resistance of EE is better than EP and equal to QEC, while the resource efficiency of EE can potentially exceed the QEC; EEBED can guarantee long-distance entanglement validity by sacrificing partial throughput.
## Repository Structure
- `EE`                   source code of EE
	+ `D-CNOT`  the experiment of EE-based D-CNOT
		* `EE Based D-CNOT.ipynb` including the quantum circuit of EE-based D-CNOT, experiment of EE-based D-CNOT performance, and experiment of EE-based D-CNOT under different noise
	+ `EntanglementDistribution` source code of the experiment of EEBED
		* `EEBED(3_nodes).ipynb` including the quantum circuit of 3-hop EEBED and the experiment of EEBED performance
		* `EEBED(4_nodes).ipynb` including the quantum circuit of 4-hop EEBED and the experiment of EEBED performance
		* `EEBED(indirectly throughput test).ipynb` calculating the throughput of EEBED according to the result of EEBED(3_nodes) and EEBED(4_nodes).
- `ComparisonMethods`          source code of Entanglement Purification(EP), Surface Code(SC), Traditional D-CNOT, and Traditonal Entanglement Distribution
	+ `D-CNOT` the experiment of EP-based D-CNOT, SC-based D-CNOT and Traditional D-CNOT
