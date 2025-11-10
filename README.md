Project Title:

Bank Queue Simulation using C

 Project Description:

The following project simulates customer arrivals and services in a bank over an 8-hour working day (480 minutes) for analysis of customers' waiting times.

Customers arrive randomly with a Poisson distribution, reflecting real-life probability of arrivals.

Each customer joins a queue and is served by one of the available tellers; each service takes 2–3 minutes.

At the end of the simulation, the program calculates and reports:

Total customers served

Average waiting time

Maximum wait time

A data-driven approach to inform the bank manager's decision on whether to hire an extra teller in order to reduce waiting times.

Concepts Used:

C Programming Concepts:

for and while loops – to simulate time progression and teller activity

if / else conditions: for decision-making during service and arrivals

Functions – for modular code, e.g. Poisson random generator

Arrays: to store queue data and wait times

Random numbers: rand(), srand(time(NULL)) to simulate random arrivals and service times

Variables and control flow - to manage queue, tellers, and customer tracking

Mathematical Concepts:

Poisson Distribution (λ) - to model random customer arrivals per minute

Mean (Average) – To calculate the average customer waiting time

Maximum (Range) – to find the longest recorded wait time

Probability theory -- for realistic simulation of arrivals

How to Compile:


Open terminal in VS Code and type:

gcc bank_queue.c -o bank_queue -lm

Explanation:

gcc → GNU C compiler

bank_queue.c → your source code file

-o bank_queue → creates an executable named bank_queue

-lm → links the math library (required for exp() function in Poisson calculation)

How to Run:


Compile, then run the program using:

./bank_queue
Then input after the prompts. For example: Enter average customers per minute (lambda, e.g. 0.6): 0.8 Enter number of tellers (1-5): 2
