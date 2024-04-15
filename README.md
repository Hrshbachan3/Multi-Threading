# Assignment-7: Multi-Threading

# Information
Name: Hrsh Dhingra\
Roll no.: 102103443\
Branch: B3-CO16

# Methodology
**Note:** my workstation contains 10 cores, 2 efficiency and 8 performance cores. I will utilize all of them for multi-threading in my program.

## Functions made:
1. ```matrix_multiplication()```: This function multiplies 2 matrices using NumPy's function ```np.dot()``` and stores the result in the ```result``` array.
2. ```run_with_threads()```: This functions performs multi-threading, utilisng a specific number of threads to perform matrix multiplication and returning the time taken.
   
## Execution:
1. Define a matrix ```A``` and a list of 100 random matrices.
2. Call the function ```run_with_threads()``` for each number of threads, which records the time taken for each matrix multiplication and stores it in ```results_table```.
3. Display the results using the ```tabulate()``` function.
4. Plot the number of threads along with the corresponding time taken using ```matplotlib.pyplot()```.

# Observation:
The time taken is minimum when the number of threads is 10, since my laptop's CPU contains 10 cores. One thing to note is that time of execution of the program on my computer is higher in comparision to other systems. This is beacause my system utilises an ARM based processor, and the translation of python's calls from x86 to ARM happen simultaneously as the program executes, resulting in a longer execution time. This does not have any effect on the final results, as shown by the graph below:

<p align="center">
  <img src="https://github.com/Hrshbachan3/Multi-Threading/blob/main/graph.png" width="600"/>
</p>

The CPU utilization for 2 program executions is shwon below: (red represents system usage, green represents utilization from current user)

<p align="center">
  <img src="https://github.com/Hrshbachan3/Multi-Threading/blob/main/cores.png" width="600"/>
</p>
