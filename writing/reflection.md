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

