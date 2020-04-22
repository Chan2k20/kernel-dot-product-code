#include <stdio.h>
#include <iostream>
#include <stdlib.h>
#include <cuda.h>
#include <math.h>
#include "solution.h"


#kernel function that will be called in main cuda file.
__global__ void kernel(unsigned int rows, unsigned int cols , float *dev_dataT,
	 float *dev_dataV, float *results)
	{
        float dot_product = 0.0;
        int tid  = threadIdx.x + blockIdx.x * blockDim.x;
      
    	for (int i = 0; i < cols; i++)
    	{
    		dot_product += dev_dataT[rows*i +tid]*dev_dataV[i];
    		
    	}
    	results[tid] = dot_product;
    }

