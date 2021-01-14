# Dyna-q+ implementation in Java

### States
1 -  S1: 0 - 99 points 

2 -  S2: 100 - 199 points 

.
.
.

9 -  S9: 900 - 999 points 

10 - S10: 1000 points 

**Attaining S10 is the goal.**

### Actions
0 - Post the Question 

1 - Post the Answer 

2 - Post the blog 

3 - Post the article 

4 - Post the task 

## Values given as input to the function

## How is the transition probability calculated for every transition
Transition probablity updates every time a faculty's state is changed.
Transition probably from S0 - S1 is calculated as follows:
Number of faculty in 100-200 points range divided by the total number of faculty.

Similarly, transition probability from S0 - S2 is calculated as follows:
Number of faculty in 200-300 points range divided by the total number of faculty.

So on and so forth...

For eg.
To transition from S0 - S1 state, currently out of 50 faculty, 1 has 150 points, 
transition probability is 1 / 50

To transition from S1 - S2 state, currently out of 50 faculty, 2 has 270 points, 
transition probably is 3 / 50.

...

## How to compile

* Download and Install [Gradle][1]
* From the root folder run the following commands
    1.`gradle build`
    2.`gradle run`
    
    
[1]: https://gradle.org/install/