#README.md

omer kidron and dean bazak 
The selected algorithms are: Bubble Sort,Merge Sort and Quick Sort

<img width="1000" height="600" alt="result1" src="https://github.com/user-attachments/assets/fa0694bb-25e6-481a-ae7d-756a0c586521" />
The graph illustrates the performance of the three algorithms on completely unsorted data
bubble sort- exponential growth o(n^2), Merge Sort & Quick Sort- o(n log n), the gap is massive even at small sizes

<img width="1000" height="600" alt="result2_5_noise" src="https://github.com/user-attachments/assets/3c99637e-b02c-4f60-a395-0ff7f5d3ecfc" />
This experiment tests how the algorithms handle arrays that are almost entirely sorted (only 5% noise) Bubble Sort Improvement: You can notice that Bubble Sort is faster here compared to the random case. but still o(n^2). Efficiency: Merge and Quick Sort remain the superior choice

<img width="1000" height="600" alt="result2_20_noise" src="https://github.com/user-attachments/assets/0562a67f-0d77-4b6b-8102-5a4ad3e2d519" />
With 20% noise, the array is more disordered than the previous case but still significantly better than a random one. The runtime for Bubble Sort increases compared to the 5% noise experiment
Even with partial sorting, o(n^2) algorithms like Bubble Sort struggle to compete with recursive algorithms as o(n) grows.


Performance Comparison:
The primary difference between the plots is the efficiency of Bubble Sort, which is highly dependent on the initial order of the array. The recursive algorithms (Merge and Quick Sort) remain consistently fast across all cases.

-Random Arrays: This represents the "worst-case" scenario for Bubble Sort . Since the data is completely unsorted, the algorithm must perform a maximum number of swaps, leading to the highest runtime (approx. 0.65s at n=3000).

-5% Noise: This is the "best-case" scenario. Since 95% of the array is already sorted, Bubble Sort finds very few out-of-order pairs . This significantly reduces the number of operations, dropping the runtime to approx. 0.38s.

-20% Noise: As the noise increases, the "nearly sorted" advantage diminishes . With more disordered elements, Bubble Sort's runtime climbs back up to approx. 0.42s.
