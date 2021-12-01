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

TODO: Explain the setup for your experiment that you ran to characterize the
performance of the different configurations of containment checking algorithms.
For instance, you should consider the following parameters as a part of your
experiment:

- The specific sorting algorithm
- The starting size of the data container: small values (e.g., 1024 numbers) to big
  values (e.g., 1,048,576 numbers)
- The total number of doubles conducted during the experiment (e.g., 5 or 10)

TODO: You may need to design a custom experiment for certain sorting algorithms
due the fact that there may be some algorithms that are inefficient!

TODO: You must justify every part of your experiment design and then furnish
output examples to demonstrate that your program generates correct data!

## Research Questions

RQ 1: When using the sorting algorithms at a starting size of 150, which of the sorting types is the fastest?

RQ 2: When using the sorting algorithms at a starting size of 150 which, with a doubling execution of 8 which of the sorting algorithms is the fastest?

RQ 3: What is the highest data container size that the individual appraoches can run while still producing an output within one minute?

## Performance Analysis

### Empirical Evaluation

TODO: The output data tables provided above of the ones that you should
reference when you are reporting on your empirical evaluation.

TODO: Provide at least three paragraphs that explain which containment checking
algorithm is fastest, by how much it is faster, and how you knew that it was
faster, referencing the data in the aforementioned command outputs and the data
tables to support your response. You should make sure that you answer each of
the at least three research questions that you posed in a previous section.

TODO: Make sure that your responses explain WHY certain configurations are faster!
TODO: It is not sufficient to ONLY explain WHICH configuration is faster!

### Analytical Evaluation

TODO: Using the provided source code for the different containment check
algorithms, your textbook, your experimental results, and any relevant online
resources that you cite in this reflection, define the worst-case time
complexity, using the big-O notation, for the five sorting algorithms. Please
note that you do not need to prove the worst-case time complexity; rather you
may reference existing sources that tell you the worst-case time complexity and
then confirm that they are correct by using your empirical results.

## Professional Development

### What is challenging about designing an experiment to evaluate sorting algorithm's performance?

TODO: Provide a one-paragraph response that answers this question in your own words.

### Overall, what is the fastest sorting algorithm based on your empirical results?

TODO: Provide a one-paragraph response that answers this question in your own words.

### How do the empirical results suggest that you don't yet know the entire story about the performance of sorting algorithms?

TODO: Provide a one-paragraph response that answers this question in your own words.
