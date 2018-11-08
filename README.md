# HPC
--------------------------
  A Introduction to High-Performance-Computing
  
  Basic examples.
  
  
  To compute the value of pi in parallel with MPI and openMP.
  
  -----------------------
    The way to run MPI in linux terminal: 
     mpicc -o dest src       //dest is your excutable file, src is you source file.
     mpirun -np n dest         //n is the number of process you schedule for the program.
    
    eg.
      mpicc -o parallel parallel.c
      mpirun -np 4 parallel
    
    The way to run openMP in linux terminal:
     gcc -fopenmp -o dest src      
     ./dest
    
    eg.
      gcc -fopenmp -o reduction reduction.c
      ./reduction
