# DISC 2024 - 38th International Symposium on Distributed Computing
Codes and sample data for experiments - DISC 2024 - 38th International Symposium on Distributed Computing

In the context of quantum computing, a resource estimator is a tool or framework used to predict and analyze the resources required to execute a quantum algorithm on a quantum computer. These resources typically include the number of qubits, gates, memory, execution time, and other computational resources needed for the algorithm to run successfully. Resource estimation plays a crucial role in the development and optimization of quantum algorithms and circuits, as it allows researchers and engineers to assess the feasibility and scalability of their algorithms on existing or future quantum hardware.

Here are some key concepts related to resource estimation in the context of quantum computing:

1. **Qubit Count**: The number of qubits required to encode and process the input, perform intermediate computations, and store the output of the quantum algorithm. Qubit count estimation is essential for understanding the quantum volume and scalability of the algorithm.

2. **Gate Count**: The number of quantum gates (such as single-qubit gates and two-qubit gates) required to implement the quantum operations specified by the algorithm. Gate count estimation helps quantify the computational complexity of the algorithm and assess its feasibility on available quantum hardware.

3. **Execution Time**: The total time required to execute the quantum algorithm on a quantum computer. This includes the time taken for quantum gate operations, qubit initialization, measurement, error correction, and other overheads. Estimating execution time helps evaluate the algorithm's efficiency and performance.

4. **Memory Requirements**: The amount of memory or storage space needed to store intermediate results, quantum states, error correction codes, and other data during the execution of the algorithm. Memory estimation is crucial for assessing the memory constraints of the quantum hardware and optimizing memory usage.

5. **Error Rates**: The error rates associated with quantum gates, qubit operations, and measurements. Error rate estimation helps account for the noise and imperfections in the quantum hardware, allowing researchers to optimize error correction strategies and mitigate the impact of errors on algorithm performance.

6. **Parallelism and Partitioning**: The degree of parallelism achievable in the quantum algorithm and the potential for partitioning the algorithm into smaller sub-circuits or segments. Parallelism and partitioning analysis enable researchers to distribute computational tasks across multiple qubits or quantum processing units (QPUs) efficiently, improving overall performance and scalability.

7. **Communication Overhead**: The overhead associated with communication between qubits, partitions, or processing units in distributed quantum computing systems. Communication overhead estimation helps identify bottlenecks and optimize communication protocols to minimize latency and maximize throughput.

Overall, resource estimation provides valuable insights into the computational requirements and performance characteristics of quantum algorithms, guiding algorithm design, optimization, and hardware development in the rapidly evolving field of quantum computing.

In the context of quantum circuit partitioning, a resource estimator could provide the following set of results:

1. **Number of Qubits**: The total number of qubits required for the partitioned quantum circuit, including both logical and ancillary qubits.

2. **Gate Count**: The count of quantum gates in each partitioned segment of the circuit, indicating the computational complexity of each segment.

3. **Depth**: The depth of each partitioned segment, representing the number of quantum gates in the critical path of execution.

4. **Execution Time**: An estimate of the execution time for each partitioned segment, considering factors such as gate delays and communication overhead.

5. **Communication Cost**: The cost associated with inter-partition communication, quantifying the number of entangled bits (ebits) or qubits dedicated to communication between partitions.

6. **Qubit Topology**: Information about the arrangement of qubits within each partitioned segment, including their connectivity and layout.

7. **Constraint Violations**: Any violations of constraints specified for the partitioning process, such as maximum duration, logical depth, or maximum number of partitions.

8. **Telemetry Data**: Real-time data on the performance of each partitioned segment during execution, including error rates, gate fidelity, and operational metrics.

9. **Mapping**: Mapping information indicating how logical qubits are mapped to physical qubits within each partitioned segment, considering constraints and optimization strategies.

10. **Partitioning Strategy**: Details about the chosen partitioning strategy, including the rationale behind the selection and any trade-offs considered.

These results collectively provide insights into the resource requirements, performance characteristics, and constraints associated with partitioned quantum circuits, enabling informed decision-making and optimization in the quantum computing workflow.

Experiments realized:
-----------------------------------------------------------------------------------------------------------
1) n2-10e-8o
python chemistry.py -f https://aka.ms/fcidump/n2-10e-8o
fcidump file - n2-10e-8o: 11 KB
-----------------------------------------------------------------------------------------------------------
(base) PS C:\Users\wcamb\qsharp\samples\estimation\df-chemistry> python chemistry.py -f https://aka.ms/fcidump/n2-10e-8o
Downloading https://aka.ms/fcidump/n2-10e-8o to n2-10e-8o...
Algorithm runtime: 19 mins
Number of physical qubits required: 207.60k
For more detailed resource counts, see file resource_estimate.json
(base) PS C:\Users\wcamb\qsharp\samples\estimation\df-chemistry>
-----------------------------------------------------------------------------------------------------------
2) polyyne-24e-24o
python chemistry.py -f https://aka.ms/fcidump/polyyne-24e-24o
fcidump file - polyyne-24e-24o: 3.009 KB
-----------------------------------------------------------------------------------------------------------
Downloading https://aka.ms/fcidump/polyyne-24e-24o to polyyne-24e-24o...
Algorithm runtime: 9 hours
Number of physical qubits required: 656.30k
For more detailed resource counts, see file resource_estimate.json
-----------------------------------------------------------------------------------------------------------
3) fe2s2-10e-40o
python chemistry.py -f https://aka.ms/fcidump/fe2s2-10e-40o
fcidump file - fe2s2-10e-40o: 11.142 KB
-----------------------------------------------------------------------------------------------------------
Downloading https://aka.ms/fcidump/fe2s2-10e-40o to fe2s2-10e-40o...
Algorithm runtime: 3 days
Number of physical qubits required: 830.76k
For more detailed resource counts, see file resource_estimate.json
-----------------------------------------------------------------------------------------------------------
4) XVIII-cas4-fb-64e-56o
python chemistry.py -f https://aka.ms/fcidump/XVIII-cas4-fb-64e-56o
fcidump file - XVIII-cas4-fb-64e-56o: 52.305 KB
-----------------------------------------------------------------------------------------------------------
Downloading https://aka.ms/fcidump/XVIII-cas4-fb-64e-56o to XVIII-cas4-fb-64e-56o...
Algorithm runtime: 8 days
Number of physical qubits required: 1.30M
For more detailed resource counts, see file resource_estimate.json
-----------------------------------------------------------------------------------------------------------
5) nitrogenase-54e-54o
python chemistry.py -f https://aka.ms/fcidump/nitrogenase-54e-54o
fcidump file - nitrogenase-54e-54o: 31.935 KB
-----------------------------------------------------------------------------------------------------------
Downloading https://aka.ms/fcidump/nitrogenase-54e-54o to nitrogenase-54e-54o...
Algorithm runtime: 268 days
Number of physical qubits required: 1.38M
For more detailed resource counts, see file resource_estimate.json
