# PDP
pdp lab assessments related to masters in computing science


assement 2 
Lab 2

Given below is a sequential program that calculates the frequency of even values in a large array. Your task is to write a parallel solution that distributes all of the workload over the number of processors on the machine executing your program. The work should be distributed so that each thread deals with block segments that do not differ in size by more than 1.

 public static void main(String[] args) {
          int f[] = new int[1000000];
          for(int j = 0; j < f.length;j++) f[j] = (int)(Math.random()*100000);
          int freq = 0;
          for(int j = 0; j < f.length; j++)
        	  if(f[j] % 2 == 0) freq++;
          System.out.println(freq);
      }


Output like :

 Running Time = 24 millisecs (0.024) 
Number of Threads = 10 
Number of even values = 500273
