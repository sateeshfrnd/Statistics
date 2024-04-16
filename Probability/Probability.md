# Probability 

Probability is a way to measure of the chance or likelihood of an event occurring. It's a tool we use to understand and quantify uncertainty.It is a numerical value between 0 and 1, where 0 indicates impossibility (the event will not occur) and 1 indicates certainty (the event will occur).

Eg:
1. if you're flipping a fair coin, there are two possible outcomes, heads or tails. The probability of getting heads is 1 out of 2 (or 1/2), and the probability of getting tails is also 1 out of 2 (or 1/2).

2. if you're rolling a fair six-sided die, each face has an equal chance of landing face-up, so the probability of rolling any particular number (like a 3) is 1 out of 6 (or 1/6), since there are six possible outcomes.
 
In probability theory, an event is any outcome or set of outcomes of an experiment or random process. The probability of an event is denoted by P(E), where E is the event.

- **Experiment:** A repeatable procedure with a set of possible results.
- **Event:** One or more obervations of an experiment.

  ```
  Probability = Share of Success / Total No. of possible outcomes.
  ```

## Probability Principles
Probability principles are fundamental concepts that help us understand and quantify uncertainty in various situations. 
  - Exact outcome can't be predicted.
  - All the possible outcomes are known.
  - Equally like outcomes.
  - Repeatable under uniform conditions.

Some key probability principles include:
- **Sample Space:** Set of all possible outcomes of an experiment or random phenomenon. It represents all the different things that could happen.
- **Probability Rule:**
  1. Probability value of an event occuring will be between 0 and 1.
      ```
      0 =< P(E) =< 1 
      0 represents impossibility (the event will never occur)
      1 represents certainty (the event will always occur). 
      ```
  2. Sum of all the probability values should be **1**.
      ```
      P(H) + P(T) = (1/2) + (1/2) = 1

      P(H) = 1 - P(T)  ==> Rule of Subtraction.
      ```
- **Complement Rule:** The complement of an event A represents all outcomes in the sample space that are not in event A.
  The probability of the complement of an event is

  ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/4a69c6b5-c613-445e-9dda-4f9f2ffdeaf0)

- **General Addition Rule:**
   - The addition rule states that the probability of the union of two events A and B is equal to the sum of their individual probabilities minus the probability of their intersection.

     ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/475c9c96-7e78-4692-baa2-c5f389b4d7de)

   - In case of of the disjoin events (never occur together)

     ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/01eeb282-d266-464c-8b5b-75807258c48b)

- **General Multiplication Rule**
     -  The multiplication rule states that the probability of the intersection of two events A and B is equal to the product of their individual probabilities given that they are independent events.

        ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/a526c044-2e22-4d1c-993c-cd35fba97c14)

        - P(A) is the probability of event A occurring.
        - P(B∣A) is the conditional probability of event B occurring given that event A has already occurred.

   - In the case of independent events, the General Multiplication Rule simplifies because the occurrence of one event does not affect the probability of the other event occurring.
   - For two independent events A and B, the probability of both events occurring together (the intersection of A and B) is simply the product of their individual probabilities.

        ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/23ae3aaf-24a7-4343-a4c0-7f88b9039e74)

     This is because the conditional probability P(B∣A) reduces to the marginal probability P(B) when the events are independent.
      
- **Conditional Rule**
    - The probability of an event given that another event has occurred.
    - Probability of an event A occurring given that event B has occurred is equal to the probability of both events A and B occurring together, divided by the probability of event B occurring:
 
      ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/3fd20711-0454-48d3-9c9c-234d4dc98467)

## Problems
**There are 30 students all together in that 16 Students studying French and 21 students studying Spanish. Find the probability of Students studying French, Spanish, Only French, Only Spanish, French or Spanish, French and Spanish**
```
Probability of students studying French P(F) = 16/30 = 8/15 = 0.5
Probability of students studying Spanish P(S) = 21/30 = 0.7
Probability of students studying French or Spanish P(F or S) = P(F) + P(S) = 0.5 + 0.7 = 1.2 (Note: This exceeds 1 because it assumes no students study both French and Spanish.)
Probability of students studying both French and Spanish P(F and S): P(F) + P(S) - P(F or S) =  0 (assuming no students study both)

```
