# Sorting Algorithms

## Evelyn Griffith

## Program Output

### Report at least five examples of program output to demonstrate that your `listsorting` program works correctly

#### One output from running the `listsorting` program

```
✨ Conducting an experiment to measure the performance of list sorting.
The chosen sorting algorithm:quick
Starting size of the data container: 1024
Number of doubles to execute: 5
Here are the results from running the experiment:

  Input Size    Min time (s)    Max time (s)    Avg time (s)
------------  --------------  --------------  --------------
        1024         0.03083         0.03149         0.03115
        2048         0.06429         0.06542         0.06504
        4096         0.13147         0.13326         0.13226
        8192         0.26137         0.27138         0.2665
       16384         0.5151          0.56056         0.5332
```

#### One output from running the `listsorting` program

```✨ Conducting an experiment to measure the performance of list sorting.
The chosen sorting algorithm:merge
Starting size of the data container: 1024
Number of doubles to execute: 5
Here are the results from running the experiment:

  Input Size    Min time (s)    Max time (s)    Avg time (s)
------------  --------------  --------------  --------------
        1024         0.06285         0.06299         0.06291
        2048         0.14006         0.14574         0.14235
        4096         0.30893         0.31109         0.3101
        8192         0.67531         0.69421         0.68285
       16384         1.48643         1.55971         1.51117
```

#### One output from running the `listsorting` program

```✨ Conducting an experiment to measure the performance of list sorting.
The chosen sorting algorithm:insertion
Starting size of the data container: 124
Number of doubles to execute: 5
Here are the results from running the experiment:

  Input Size    Min time (s)    Max time (s)    Avg time (s)
------------  --------------  --------------  --------------
         124         0.00803         0.00838         0.00821
         248         0.03112         0.03136         0.03127
         496         0.13558         0.14168         0.13785
         992         0.67773         0.7925          0.73595
        1984         2.58553         2.85783         2.76101
```

#### One output from running the `listsorting` program

```
✨ Conducting an experiment to measure the performance of list sorting.
The chosen sorting algorithm:tim
Starting size of the data container: 124
Number of doubles to execute: 5
Here are the results from running the experiment:

  Input Size    Min time (s)    Max time (s)    Avg time (s)
------------  --------------  --------------  --------------
         124         0.01132         0.01143         0.01138
         248         0.04423         0.04581         0.04482
         496         0.17841         0.21593         0.19316
         992         0.68284         0.76916         0.7211
        1984         2.90319         2.96192         2.92864
```

#### One output from running the `listsorting` program

```
✨ Conducting an experiment to measure the performance of list sorting.
The chosen sorting algorithm:bubble
Starting size of the data container: 124
Number of doubles to execute: 5
Here are the results from running the experiment:

  Input Size    Min time (s)    Max time (s)    Avg time (s)
------------  --------------  --------------  --------------
         124         0.01719         0.02496         0.02025
         248         0.06994         0.08718         0.08079
         496         0.28988         0.30155         0.29424
         992         1.32909         1.50191         1.40307
        1984         5.45098         5.47907         5.4631
```

## Experiment Design

RQ 1: The experiment that I am hoping to do for the first RQ will have a starting size container of 150 and will run through each sorting algorith to determine which one is fastest. This means that I will be running the algorithms with a doubling experiment number of 5. This is an important experiment to do becuase it will give me an idea of which algorithm is the fastest when using a common starting point for the data containers.

RQ 2: The experiment that I will do for this question will be to change the data container size to 19. I chose this number because I want the program to run up to as close to the same data container size when it does the doubling experiment as possible, but I want it to do the doubling experiment more times than it did in the previous RQ. This will tell me how the doubling experiment effects the run time of the program.

RQ 3: For the third and final question experiment, I will be locating the highest data container size that each individual approach can run in under one minute. This will tell me which one is the most efficient. I will keep the doubling experiment number as 5 for this experiment.

## Research Questions

RQ 1: When using the sorting algorithms at a starting size of 150, which of the sorting types is the fastest?

RQ 2: When using the sorting algorithms at a starting size of 150 which, with a doubling execution of 8 which of the sorting algorithms is the fastest?

RQ 3: What is the highest data container size that the individual appraoches can run while still producing an output within one minute?

## Performance Analysis

### Empirical Evaluation

RQ 1:

- When running the experiment for this RQ, I was able to find some very interesting data which Is displayed in the table below.I chose to keep the numbers small for this experiment because I wanted to see how fine the differences are between the algorithms even when working with less data. I also chose to keep the container starting size as well as the Doubling experiment size the same because I think that eliminating the variables makes the data cleaner. Now, as for what I learned through this experiment, I think the fastest algorithm is the Quick-Sort algorithm. Not only is this algorithm faster, but after further investigation, it is also able to run larger data containers than the other sorting algorithms.

|Sorting Alg.|Container Starting Size|Doubling|Avg. Time for Input Size|Size Largest Container|Avg. Time for Largest Contianer Size|
|Bubble      |150                    |5       |0.02662                 |2400                  |7.53503                             |
|Insertion   |150                    |5       |0.01128                 |2400                  |3.7856                              |
|Merge       |150                    |5       |0.00869                 |2400                  |0.16748                             |
|Quick       |150                    |5       |0.00427                 |2400                  |0.07807                             |
|Tim         |150                    |5       |0.01762                 |2400                  |4.0565                              |

RQ 2:

- When running the experiment for RQ2, I was able to find some very interesting data that I can use to compare with the previous data. This RQ was meant to address the idea that the doubling of an experiment can also affect the run time of a program. I wasn't sure if the doubling itself was taking up time so I wanted to run this experiment to the best of my ability to see if this was adding time just like the container size was. The numbers that I got are not ideal because I would have hoped to get a final container size of 2400 just like the previous doubling experiment. However in order to do that, I would have had to have a starting container size of 18.75 which causes the program to crash. This makes sense because you cant have .75 of a peice of a container. So in order to remedy this, I chose to start at 19. This gives a final container size of 2432 which isn't perfect for the idea of this experiment, but still should be close enough numbers to see whether or not the actual action of doubling takes up time for the program.

When running this program I found that for Bubble, the actual doubling takes about 8.40246-7.53503 = .29 seconds.
When running this program I found that for Insertion, the actual doubling takes about 3.99956-3.7856 = .07 seconds.
When running this program I found that for Merge, the actual doubling takes about 0.19847-0.16748 = .01 seconds.
When running this program I found that for Quick, the actual doubling takes about 0.09066-0.07807 = .0033 seconds.
When running this program I found that for Tim, the actual doubling takes about 4.66351-4.0565 = .203 seconds.

This is interesting because it suggests that the Merge-Sort and the Quick-sort (which previous data already proved to be the fastest) is faster at actually doing the doubling experiment.

|Sorting Alg.|Container Starting Size|Doubling|Avg. Time for Input Size|Size Largest Container|Avg. Time for Largest Contianer Size|
|Bubble      |19                    |8       |0.00073                  |2432                  |8.40246                             |
|Insertion   |19                    |8       |0.0003                   |2432                  |3.99956                             |
|Merge       |19                    |8       |0.0008                   |2432                  |0.19847                             |
|Quick       |19                    |8       |0.0006                   |2432                  |0.09066                             |
|Tim         |19                    |8       |0.00031                  |2432                  |4.66351                             |

RQ 3:

For this RQ I do not have any collected data. I did collect a little bit of data, but after running my experiment for a while I realized that it wasn't going to work the way that I had intended. In order to run this experiment, I was planning to put a number in for the starting size of my data container, set a timer for two minutes, and then adjust the data container starting size until I was able to find the point where that particular algorithm was able to produce an output in just under two minutes. This was meant to tell me which of the algorithms can run the largest data container in the same amount of time as the others. 

However, when I was running the Bubble-Sort algorithm, the first algorithm that I tried to do this with, I realized that this was not going to function correctly. Here is why: When I was running the algorithm, I was able to get the data container up to a starting size of 260 and this would leave about 15 seconds left on my timer when the program was able to produce an output. This would have been fine, but it wasn't as close to the mark as I was hoping to get (I was shooting for somewhere around 5 seconds or less for the function to produce an output). However, I ended up getting impatient and instead of running for the two minute mark, I decided to start running for the 1 minute mark. I naturally decided to split the 260 in half and start from there expecting to have about 15 seconds left on the timer for the program to produce an output. When the program produce an output in with 31 seconds to spare, I knew that my experiment plan wasn't going to work because in order to test in this manner, the number that I really needed to be concerned with is the largest size that the container would be doubling to and this number is exponentially found through the starting size. That's what leads me to believe that my experiment design was flawed for question three. 

However, I was still able to gain the knowledge needed from the two previous questions to ascertain that the Quick-Sort function is indeed the fastest.

### Analytical Evaluation

In order to complete the analytical evaluation for this assignment, I decided to use the already given doubling data to determine the doubling ratios for each sorting algorithm.

For Bubble-sort:

- I took the data from the above example of a Bubble Sort and divided the example for a container size of 2048/1024. This gave an output of 0.08079/0.02025 = 3.99, which can be rounded to 4.

For Quick-Sort:

- I took the data from the above example of a Quick Sort and divided the example for a container size of 2048/1024. This gave an output of 0.06504/0.03115 = 2.09, which can be rounded to 2.

For Merge-Sort:

- I took the data from the above example of a Merge Sort and divided the example for a container size of 2048/1024. This gave an output of 0.14235/0.06291 = 2.26, which can be rounded down to 2.

For Insertion-Sort:

- I took the data from the above example of a Insertion Sort and divided the example for a container size of 2048/1024. This gave an output of 0.03127/0.00821 = 3.81, which can be rounded to 4.

For Tim-Sort:

- I took the data from the above example of a Tim Sort and divided the example for a container size of 2048/1024. This gave an output of 0.04482/0.01138 = 3.94, which can be rounded to 4.

The analysis that these mathematical equations give us actually makes a lot of sense. Whenver I ran either the Insertion, Tim, or Bubble sort algorithms at the size container of 1024, they were unable to complete. Even if I ran them at half of that size they were not able to finish running, however the Merge, and Quick sorts were able to. I think it makes sense that the Merge and Quick sort algorithms have a linear worst case becuase they were much much faster than the other three.

## Professional Development

### What is challenging about designing an experiment to evaluate sorting algorithm's performance?

I think one of the most challenging aspects is finding a way to set every algorithm on common ground so that you can test a certain variable. One of the things I struggled with was making sure that the container size I picked was a small enough container that Tim, Bubble, and Insertion could run it in a relatively quick amount of time, but make sure that it was a big enough container size that I was still collecting data on the Merge and Quick sort algorithms.

### Overall, what is the fastest sorting algorithm based on your empirical results?

I think the fastest function is the Quick-sort function. Not only was this notable through the doubling experiment which could be done in my analytical analysis, but it was also apparent when working through my experimental analysis because the times were able to speak for themselves.

### How do the empirical results suggest that you don't yet know the entire story about the performance of sorting algorithms?

I am interested in learning more about how the exponential aspect of the doubling experiment effects the run time of the algorithms. I am also curious as to why the Quick-Sort function is so much faster than the others.