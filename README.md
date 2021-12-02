# Hybrid-OpenMP-MPI-programming


## Compile
```
mpicc -fopenmp hybrid.c -o hybrid
```

## Define the number of thread
```
export OMP_NUM_THREADS=4
```

## Run 
```
mpirun -np 4 -x OMP_NUM_THREAD ./hybrid
```
or
```
mpirun -np 4 -host master,node001,node002,node003 -x OMP_NUM_THREAD ./hybrid
```
