# Probability Basics

*Focus: Probability, Random Variables, Distributions*

## 1. Probability

At its simplest, **probability** is a mathematical tool used to measure how likely an event is to occur. It allows us to turn uncertainty—like the flip of a coin or a weather forecast—into a precise number that we can use to make decisions.

### The Probability Scale
Probability is always measured on a scale from **0 to 1** (or 0% to 100%).

* **0 (Impossible):** The event will definitely not happen (e.g., rolling a 7 on a standard six-sided die).
* **0.5 (Even Chance):** The event is just as likely to happen as not (e.g., a fair coin landing on "Heads").
* **1 (Certain):** The event is guaranteed to happen (e.g., the sun rising tomorrow).

### The Basic Formula
If all possible outcomes are equally likely, you can calculate probability using this simple ratio:

$$P(\text{Event}) = \frac{\text{Number of favorable outcomes}}{\text{Total number of possible outcomes}}$$

#### **Example: Rolling a Die**
What is the probability of rolling an **even number** (2, 4, or 6) on a standard die?
* **Favorable outcomes:** 3 (the numbers 2, 4, and 6)
* **Total outcomes:** 6 (the numbers 1, 2, 3, 4, 5, and 6)
* **Calculation:** $3 / 6 = 0.5$ or **50%**.

### Key Vocabulary
To talk about probability like a pro, it helps to know these terms:
* **Experiment:** Any process with an uncertain result (e.g., spinning a wheel).
* **Outcome:** A single possible result of an experiment (e.g., the wheel landing on "Red").
* **Sample Space:** The complete set of *all* possible outcomes.
* **Event:** A specific outcome or collection of outcomes you are looking for.

### Why Does It Matter?
Probability isn't just for math class; it's the engine behind much of our modern world:
* **Insurance:** Companies calculate the probability of accidents to decide how much to charge for premiums.
* **Weather:** A "30% chance of rain" is a probability based on historical data.
* **Medicine:** Doctors use probability to determine the success rate of a new treatment or the likelihood of a side effect.
* **Technology:** AI and machine learning use probability to predict which words or images you are most likely looking for.

---

## 2. Random Variables

In probability, a **random variable** is essentially a rule that assigns a numerical value to each outcome of a random process. 

Think of it as a "bridge" between the messy world of random events (like coin flips or weather) and the clean world of math (numbers and equations).

### The Core Idea: Outcomes to Numbers
Imagine you flip two coins. The "outcomes" are combinations of Heads (H) and Tails (T). A random variable lets you focus on a specific number you care about, such as **"the number of heads."**

| Outcome | Random Variable ($X = \text{number of heads}$) |
| :--- | :--- |
| (T, T) | $0$ |
| (H, T) | $1$ |
| (T, H) | $1$ |
| (H, H) | $2$ |

In this case, $X$ is the random variable. It isn't a single number; it is a **function** that can take on the values $0$, $1$, or $2$ depending on what happens.

### Types of Random Variables
There are two main types, categorized by the "kind" of numbers they result in:

#### **Discrete Random Variables**
These have gaps between their values—usually things you **count**.
* **Examples:** The number of students in a class, the result of a die roll, or the number of emails you get in a day.
* **Probability Tool:** We use a **Probability Mass Function (PMF)** to say exactly how likely a specific value is (e.g., "The probability of rolling a 4 is $1/6$").

#### **Continuous Random Variables**
These can take any value in a range—usually things you **measure**.
* **Examples:** The exact height of a person, the time until the next bus arrives, or the temperature outside.
* **Probability Tool:** We use a **Probability Density Function (PDF)**. Because there are infinite possible values (like $5.1234...$ cm), the probability of hitting one *exact* number is technically zero. Instead, we measure the probability of falling within a **range**.

### Notation (The Math Language)
When you see probability formulas, you’ll notice a specific way of writing things:
* **$X$ (Capital Letter):** Refers to the random variable itself (the "rule").
* **$x$ (Lowercase Letter):** Refers to a specific value the variable could take.
* **$P(X = x)$:** This reads as: "The probability that the random variable $X$ equals the specific value $x$."

> **Example:** $P(X = 2) = 0.25$ means "There is a $25\%$ chance that we will see exactly $2$ heads."

### Summary Table
| Feature | Discrete | Continuous |
| :--- | :--- | :--- |
| **How to get it** | Counted | Measured |
| **Possible Values** | Distinct points (e.g., $1, 2, 3$) | Any value in an interval (e.g., $[0, 10]$) |
| **Example** | Number of rainy days | Amount of rainfall (inches) |

---

## 3. Distributions

In probability, a **distribution** is a mathematical function that describes all the possible values a random variable can take and how likely each of those values is.

If a **random variable** is the rule for assigning numbers to events, the **distribution** is the "master map" that shows the pattern of those numbers.

### How Distributions Work
Think of a distribution as a summary of an experiment. Instead of just looking at one outcome, you look at the **entire landscape** of what could happen.

For a single six-sided die, the distribution is "Uniform." Every outcome ($1, 2, 3, 4, 5, 6$) has an equal probability of $1/6$. If you graphed this, it would look like six bars of the exact same height.

### Discrete vs. Continuous Distributions
Just like random variables, distributions are divided into two main categories:

#### **Discrete Distributions**
These are used for things you can count. They are often represented by a **Probability Mass Function (PMF)**, which shows the exact probability for each distinct value.
* **Binomial Distribution:** Used for "Yes/No" scenarios (e.g., "If I flip 10 coins, what's the chance I get exactly 7 heads?").
* **Poisson Distribution:** Used for counting events over time (e.g., "How many customers will walk into this store in the next hour?").

#### **Continuous Distributions**
These are used for things you measure. They are represented by a **Probability Density Function (PDF)**. Because there are infinite possibilities, we look at the "density" or area under a curve.
* **Normal Distribution (The Bell Curve):** The most famous distribution. It describes things like height, IQ scores, or measurement errors, where most values cluster around the average.
* **Uniform Distribution:** Where every value in a specific range (like any number between 0 and 1) is equally likely.

### Key Characteristics
To describe a distribution, statisticians look at a few "summary" numbers:
* **Mean ($\mu$):** The center or average value of the distribution.
* **Variance ($\sigma^2$):** How spread out the values are from the center.
* **Skewness:** Whether the distribution is symmetrical or "leans" to one side.

### Summary Comparison

| Feature | Discrete Distribution | Continuous Distribution |
| :--- | :--- | :--- |
| **Visual** | Bar Chart | Smooth Curve |
| **Math Tool** | Summation ($\sum$) | Integration ($\int$) |
| **Common Example** | Rolling a pair of dice | The height of adult men |
| **Probability of a single point** | Can be greater than 0 | Always 0 (must use a range) |


