# Probability Basics

*Focus: Probability, Random Variables, Distributions*

## Probability


---

## Random Variables

In probability, a **random variable** is essentially a rule that assigns a numerical value to each outcome of a random process. 

Think of it as a "bridge" between the messy world of random events (like coin flips or weather) and the clean world of math (numbers and equations).

## 1. The Core Idea: Outcomes to Numbers
Imagine you flip two coins. The "outcomes" are combinations of Heads (H) and Tails (T). A random variable lets you focus on a specific number you care about, such as **"the number of heads."**

| Outcome | Random Variable ($X = \text{number of heads}$) |
| :--- | :--- |
| (T, T) | $0$ |
| (H, T) | $1$ |
| (T, H) | $1$ |
| (H, H) | $2$ |

In this case, $X$ is the random variable. It isn't a single number; it is a **function** that can take on the values $0$, $1$, or $2$ depending on what happens.

## 2. Types of Random Variables
There are two main types, categorized by the "kind" of numbers they result in:

### **Discrete Random Variables**
These have gaps between their values—usually things you **count**.
* **Examples:** The number of students in a class, the result of a die roll, or the number of emails you get in a day.
* **Probability Tool:** We use a **Probability Mass Function (PMF)** to say exactly how likely a specific value is (e.g., "The probability of rolling a 4 is $1/6$").

### **Continuous Random Variables**
These can take any value in a range—usually things you **measure**.
* **Examples:** The exact height of a person, the time until the next bus arrives, or the temperature outside.
* **Probability Tool:** We use a **Probability Density Function (PDF)**. Because there are infinite possible values (like $5.1234...$ cm), the probability of hitting one *exact* number is technically zero. Instead, we measure the probability of falling within a **range**.

## 3. Notation (The Math Language)
When you see probability formulas, you’ll notice a specific way of writing things:
* **$X$ (Capital Letter):** Refers to the random variable itself (the "rule").
* **$x$ (Lowercase Letter):** Refers to a specific value the variable could take.
* **$P(X = x)$:** This reads as: "The probability that the random variable $X$ equals the specific value $x$."

> **Example:** $P(X = 2) = 0.25$ means "There is a $25\%$ chance that we will see exactly $2$ heads."

## Summary Table
| Feature | Discrete | Continuous |
| :--- | :--- | :--- |
| **How to get it** | Counted | Measured |
| **Possible Values** | Distinct points (e.g., $1, 2, 3$) | Any value in an interval (e.g., $[0, 10]$) |
| **Example** | Number of rainy days | Amount of rainfall (inches) |

---

## Distributions



