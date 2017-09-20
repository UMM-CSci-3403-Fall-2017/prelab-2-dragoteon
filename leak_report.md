# Leak report

The one calloc, on line 41, used in the code to allocate memory is missing something used to free up the allocation. 
To fix the problem, I added a free(result) to the code before the    return result;   in that method. 


