# PDDS – Statistics for Data Science: Full Practice Paper

**Covers:** Unit 1 (Probability, Sessions 1–3) · Unit 2 (Descriptive Statistics, Sessions 4–5) · Unit 3 (Inferential Statistics, Sessions 6–9) · Unit 4 (Linear Algebra, Session 10)

**How to use this paper:** Attempt every question in Part A cold, without looking at Part B. For each "identify the test/formula" question, you are given only the scenario — deciding *which* rule, distribution or test applies is part of what's being tested. Full worked solutions and model interpretations are in Part B, at the very end.

---

## Concept Checklist (what this paper tests)

**Unit 1 – Probability**
Set operations · sample space/event/classical probability · subjective vs objective (theoretical/empirical) probability · types of events (impossible, sure, independent, dependent, mutually exclusive, exhaustive, complementary) · 5 basic properties of probability · addition law · multiplication rule · conditional probability · marginal/joint/conditional distinction · random variables (discrete/continuous) · probability distributions, validity (Σp=1) · PMF vs PDF · CDF · expected value · naming Binomial/Poisson/Normal/Uniform distributions by scenario

**Unit 2 – Descriptive Statistics**
Population vs sample · parameter vs statistic · sampling methods (probability: simple random, systematic, stratified, cluster; non-probability: convenience, judgment, quota, snowball) · mean/median/mode (raw data and frequency tables) · best measure of central tendency · empirical mode formula · skewness · kurtosis · frequency distributions/histograms · boxplots, five-number summary · range, IQR, quartile deviation · outlier detection (1.5×IQR fences) · population vs sample variance/SD · coefficient of variation · covariance · Pearson correlation coefficient · correlation vs causation

**Unit 3 – Inferential Statistics**
Descriptive vs inferential statistics · sampling distribution of the mean · standard error · Central Limit Theorem · 5-step hypothesis testing process · H₀/H₁ formulation · Type I/Type II error · significance level vs confidence level · one-tailed vs two-tailed tests · choosing Z-test vs t-test · Z-test calculation · one-sample/independent two-sample/paired t-tests (formula + df) · p-value decision rule · measurement scales (nominal/ordinal/interval/ratio) · Chi-square goodness-of-fit · Chi-square test of independence · ANOVA (conceptual) · regression (conceptual)

**Unit 4 – Linear Algebra**
Scalars vs vectors · vector addition/scalar multiplication · dot product · vector magnitude · angle between vectors/orthogonality · cosine similarity · matrix operations (addition, scalar multiplication, multiplication) · transpose · determinant and invertibility · inverse (2×2) · trace and its properties · eigenvectors/eigenvalues (conceptual) · linear algebra in ML (data representation, PCA, gradient descent, neural networks, MSE, confusion matrix, SVD, SVM)

---

# PART A: QUESTIONS

## UNIT 1 — PROBABILITY (Sessions 1–3)

### Section 1D – Simple MCQs (1 mark each, no justification needed)

**Q1.** A set C is a subset of A if:
a) All elements of A are in C
b) All elements of C are also in A
c) A and C share no elements
d) A and C are equal

**Q2.** If P(A) = 0.3, what is P(A′) (the complement of A)?
a) 0.3
b) 0.5
c) 0.7
d) Cannot be determined

**Q3.** Which of the following is an example of a **mutually exclusive** pair of events when rolling a single die?
a) Rolling an even number and rolling a number greater than 3
b) Rolling a 2 and rolling a number less than 3
c) Rolling a 3 and rolling a 4
d) Rolling an odd number and rolling a prime number

**Q4.** A random variable representing "the number of defective items in a batch of 50" is:
a) Continuous
b) Discrete
c) Neither discrete nor continuous
d) Both discrete and continuous depending on context

**Q5.** For a valid discrete probability distribution, the probabilities of all outcomes must:
a) Each equal 0.5
b) Sum to 1
c) Each be greater than 0.5
d) Sum to the sample size

---

### Section 1C – Functional MCQs (2 marks each — justify your answer)

**Q6.** A company classifies 500 leads as follows: 220 came from social media, 180 from referrals, and the rest from cold calls. If a lead is selected at random, what is P(the lead came from cold calls)?
a) 0.22
b) 0.36
c) 0.20
d) 0.44

**Q7.** Events A and B are **independent**, with P(A) = 0.5 and P(B) = 0.4. What is P(A ∩ B)?
a) 0.9
b) 0.1
c) 0.2
d) 0.45

**Q8.** If P(A|B) = 0.6 and P(B) = 0.25, what is P(A ∩ B)?
a) 0.85
b) 0.15
c) 0.24
d) 2.4

---

### Section 1B – Calculation Questions

**Q9.** A courier company's parcels are classified as: 45 arrived on time, 30 arrived late, 25 were lost, out of 100 parcels tracked in a month.
(a) Find P(on time), P(late), P(lost).
(b) Verify these three probabilities satisfy the "sum of probabilities" property.
(c) Find the probability that a randomly selected parcel did **not** arrive late.

**Q10.** A company estimates that P(a new hire stays past 1 year) = 0.68 and P(a new hire completes onboarding) = 0.90, with P(both staying past 1 year AND completing onboarding) = 0.64.
(a) Are "staying past 1 year" and "completing onboarding" independent? Show your reasoning using the appropriate rule.
(b) Find P(staying past 1 year | completed onboarding).

**Q11.** In a survey of 400 employees, 260 work hybrid, and 130 of the hybrid workers also report high job satisfaction. If an employee is selected at random from those who work hybrid, what is the probability that they report high job satisfaction? Interpret your answer in one sentence.

**Q12.** A retail analytics team classifies 350 transactions by payment type and loyalty status:

| | Uses Loyalty Card | No Loyalty Card |
|---|---|---|
| Spent > $100 | 90 | 40 |
| Spent ≤ $100 | 60 | 160 |

(a) Find the probability that a transaction spent > $100, **given** that the customer used a loyalty card.
(b) Find the probability that the customer used a loyalty card, **given** that the transaction was > $100.
(c) Explain, in context, why these two conditional probabilities are different numbers.

**Q13.** A support team receives complaint tickets and finds the following probability distribution for X = number of complaints filed per day:

| X | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| P(X=x) | 2k | 3k | 4k | k |

(a) Find the value of k.
(b) Construct the complete probability distribution table.
(c) Find P(X ≤ 2).
(d) Find P(X > 1).
(e) State which type of function you used to describe this distribution (PMF or PDF) and why.

**Q14.** A logistics manager records X = number of failed deliveries per shift, with the distribution:

| X | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| P(X=x) | 0.1 | 0.3 | 0.4 | 0.2 |

(a) Confirm this is a valid probability distribution.
(b) Calculate the expected number of failed deliveries per shift, E(X).
(c) Interpret E(X) in one sentence in the context of shift planning.

---

### Section 1A – Written / Interpretation Question (identify-the-concept style)

**Q15.** For each of the four scenarios below, name the type of probability distribution (Binomial, Poisson, Normal, or Uniform) that would most naturally model the situation, and briefly justify your choice (you do not need to calculate anything):
(a) The number of login failures recorded on a company server in a given hour.
(b) The heights of 500 employees at a manufacturing plant.
(c) The number of successful conversions out of 20 sales calls, where each call has the same fixed chance of success.
(d) The number that comes up when rolling a fair six-sided die.

**Q16.** *(Long / integrative, ~10 marks)* A telecoms company wants to reduce customer churn. It has data on customer complaints, contract renewals, and service usage patterns.
Explain, using specific probability concepts covered in this unit (sample space, events, types of events, conditional probability, and probability distributions), how the company could use probability to assess the uncertainty around a customer renewing their contract. Use at least one worked example (real or invented) to illustrate conditional probability in this context, and state one limitation of using probability alone for this business decision.


---

## UNIT 2 — DESCRIPTIVE STATISTICS (Sessions 4–5)

### Section 2D – Simple MCQs

**Q17.** A market researcher records the ages of *all* 40 employees at a small firm. This dataset is a:
a) Sample
b) Population
c) Statistic
d) Parameter

**Q18.** A number that describes a whole population (such as the true average income of every household in a country) is called a:
a) Statistic
b) Sample
c) Parameter
d) Estimate

**Q19.** Selecting every 8th customer who enters a store is an example of:
a) Simple random sampling
b) Stratified sampling
c) Systematic sampling
d) Convenience sampling

**Q20.** If a distribution has mean > median > mode, it is:
a) Symmetrical
b) Negatively (left) skewed
c) Positively (right) skewed
d) Bimodal

**Q21.** A distribution with kurtosis less than 3 (light tails, few outliers) is described as:
a) Leptokurtic
b) Mesokurtic
c) Platykurtic
d) Skewed

---

### Section 2C – Functional MCQs (justify your answer)

**Q22.** A company surveys 5,000 customers and randomly selects 100 for a satisfaction study, drawn separately from each of 5 regional branches in proportion to branch size. This sampling method is:
a) Cluster sampling
b) Stratified sampling
c) Quota sampling
d) Snowball sampling

**Q23.** A dataset's population variance is 64. What is the population standard deviation?
a) 8
b) 32
c) 4096
d) 16

**Q24.** For the same data, dividing by (n − 1) rather than n when calculating variance is done when:
a) The data represents an entire population
b) The data represents a sample and we want an unbiased estimate of the population variance
c) The dataset has an even number of values
d) The mean is exactly zero

---

### Section 2B – Calculation Questions

**Q25.** The number of calls handled by 8 call-centre agents in one hour is: 12, 15, 15, 18, 20, 22, 25, 15.
(a) Calculate the mean.
(b) Calculate the median.
(c) Calculate the mode.

**Q26.** A survey of 50 households recorded the number of children per household:

| Number of children (x) | 0 | 1 | 2 | 3 | 4 |
|---|---|---|---|---|---|
| Frequency (f) | 5 | 12 | 18 | 10 | 5 |

Calculate the mean number of children per household using the frequency table.

**Q27.** The monthly bonuses ($) paid to 8 sales staff are: 200, 220, 230, 240, 240, 260, 270, 1200.
(a) Calculate the mean, median, and mode.
(b) Which measure of central tendency best represents the *typical* bonus? Justify your choice.
(c) Based on the relationship between the mean, median, and mode, what is the shape of this distribution (positively skewed, negatively skewed, or symmetrical)? Explain how you know.

**Q28.** A dataset has a mean of 62 and a median of 58. Using the empirical relationship between mean, median, and mode, estimate the mode.

**Q29.** The weekly sales ($'00) of 11 salespeople, sorted, are: 18, 20, 22, 24, 25, 27, 28, 30, 32, 35, 60.
(a) Find Q1 and Q3.
(b) Calculate the Interquartile Range (IQR) and the Quartile Deviation (QD).
(c) Using the data above, determine whether there are any outliers, showing your fence calculations.

**Q30.** The number of defects found per day on a production line over 5 days is: 3, 5, 4, 6, 2. Treat this as the **entire population** of interest (all 5 days that matter for this analysis).
(a) Calculate the population variance.
(b) Calculate the population standard deviation.

**Q31.** The delivery times (in minutes) for 6 randomly **sampled** orders are: 28, 32, 30, 35, 29, 31.
(a) Calculate the sample variance.
(b) Calculate the sample standard deviation.
(c) Explain, referencing your formula choice, why you divided by (n − 1) rather than n in this case, whereas in Q30 you divided by N.

**Q32.** Two machines fill bottles to a target weight of 500 g. Machine A's fill weights (grams) for a sample of 5 bottles are: 495, 500, 505, 498, 502. Machine B's fill weights for a sample of 5 bottles are: 470, 510, 530, 480, 510.
(a) Calculate the mean and standard deviation for each machine.
(b) Calculate the coefficient of variation (CV) for each machine.
(c) Which machine is more consistent? Justify using the CV values.

**Q33.** A company recorded advertising spend (X, $'000) and website visits (Y, in hundreds) over 6 months:

| Month | 1 | 2 | 3 | 4 | 5 | 6 |
|---|---|---|---|---|---|---|
| Advertising Spend (X) | 3 | 4 | 5 | 6 | 7 | 8 |
| Website Visits (Y) | 22 | 25 | 29 | 33 | 35 | 40 |

(a) Calculate the mean advertising spend and mean website visits.
(b) Calculate the covariance between X and Y (use the population formula, dividing by n).
(c) Calculate the Pearson correlation coefficient.
(d) Interpret the direction and strength of the relationship.

---

### Section 2A – Written / Interpretation Question

**Q34.** *(Long, ~10 marks)* Referring back to your answer in Q33: Does a strong correlation between advertising spend and website visits necessarily mean that increased advertising *causes* more website visits? Explain your reasoning, and suggest one other approach or piece of evidence the company would need to establish causation rather than just correlation. Then, briefly explain how a boxplot of the website-visit data could help the company check for unusual months (outliers) before trusting this correlation result.


---

## UNIT 3 — INFERENTIAL STATISTICS (Sessions 6–9)

### Section 3D – Simple MCQs

**Q35.** Inferential statistics is primarily used to:
a) Organise raw data into tables
b) Describe only the sample collected
c) Draw conclusions about a population using sample data
d) Produce graphs only

**Q36.** According to the Central Limit Theorem, as sample size increases, the sampling distribution of the sample mean:
a) Becomes more skewed
b) Approaches a normal distribution, regardless of the population's shape
c) Becomes identical to the population distribution
d) Has a standard deviation equal to the population standard deviation

**Q37.** A Type I error occurs when:
a) We reject H₀ when H₀ is actually true
b) We fail to reject H₀ when H₀ is actually false
c) We reject H₀ when H₀ is actually false
d) We accept H₁ when H₁ is actually true

**Q38.** If a hypothesis test produces a p-value of 0.03 at a 5% significance level, the correct decision is to:
a) Fail to reject H₀ — result is not significant
b) Reject H₀ — result is statistically significant
c) Increase the sample size before deciding
d) Accept H₁ as definitely true

**Q39.** "Marital status: Single / Married / Divorced" is measured on which scale?
a) Ratio
b) Interval
c) Ordinal
d) Nominal

---

### Section 3C – Functional MCQs (justify your answer)

**Q40.** A population has a standard deviation of 36. A random sample of 144 observations is drawn. What is the standard error of the sample mean?
a) 36
b) 3
c) 0.25
d) 12

**Q41.** A researcher wants to test whether the average commute time in a city is 30 minutes. The population standard deviation is unknown, and a sample of 14 commuters is used. Which test should be applied?
a) Z-test, because the sample size is large
b) t-test, because the population SD is unknown and the sample is small
c) Chi-square test, because commute time is categorical
d) F-test, because two variances are being compared

**Q42.** A quality inspector wants to know whether a machine's average fill weight (known population SD) differs from a 500 g target, using a sample of 60 items. Which test applies, and why?
a) t-test — small sample
b) Z-test — large sample and population SD is known
c) Chi-square test — comparing categories
d) Paired t-test — same items measured twice

---

### Section 3B – Calculation Questions

**Q43.** A population of delivery times has a standard deviation of σ = 45 minutes. A random sample of 81 deliveries is selected.
(a) Calculate the standard error of the sample mean.
(b) According to the Central Limit Theorem, what shape will the sampling distribution of the sample mean approximately follow, and under what condition on sample size does this generally hold?

**Q44.** For each scenario, write the null hypothesis (H₀) and alternative hypothesis (H₁), and state whether the test is one-tailed or two-tailed:
(a) A café claims its average wait time is exactly 4 minutes; a customer group wants to test whether this is true.
(b) A manufacturer claims a new battery lasts *more than* 15 hours on average.
(c) An HR analyst wants to know whether the average salary of two departments is *different*.

**Q45.** A researcher wants 99% confidence in a two-tailed hypothesis test. State the level of significance (α), and give the corresponding critical z-value for a two-tailed test at this α (use the standard z-table values from the course: α=0.10 → ±1.645; α=0.05 → ±1.96; α=0.01 → ±2.576).

**Q46.** A supplement brand claims its capsules weigh 500 g on average. A random sample of 36 capsules has a mean weight of 495 g. The population standard deviation is known to be 12 g. Test, at the 5% significance level, whether the average capsule weight differs significantly from 500 g. Show all 5 steps (hypotheses, significance level & critical value, test statistic, comparison, conclusion).

**Q47.** A coaching provider claims the average completion time for its data analytics bootcamp is 40 hours. To test this, a sample of 8 trainees is timed: 42, 39, 41, 44, 38, 40, 43, 45 hours. At the 5% significance level (two-tailed), test whether the sample provides evidence that the true mean differs from 40 hours. (For df = 7, α = 0.05 two-tailed, t-critical = ±2.365.) Show all 5 steps.

**Q48.** A company compares the test scores of employees trained by two independent methods:
Method A: 68, 72, 75, 70, 74
Method B: 60, 65, 63, 67, 62
At the 5% significance level, test whether there is a significant difference between the two methods' average scores. (For df = 8, α = 0.05 two-tailed, t-critical = ±2.306.) Show all 5 steps, including the sample means and standard deviations.

**Q49.** A wellness coach records employee stress scores (lower is better) before and after a mindfulness programme for 5 employees:

| Employee | 1 | 2 | 3 | 4 | 5 |
|---|---|---|---|---|---|
| Before | 58 | 62 | 60 | 65 | 63 |
| After | 63 | 65 | 64 | 68 | 65 |

At the 5% significance level, test whether the programme significantly changed (increased) employee scores. (For df = 4, α = 0.05 one-tailed, t-critical = 2.132.) Show all 5 steps.

**Q50.** A store expects customers to show equal preference across 4 promotional offers. A survey of 120 customers observes the following: Offer A = 40, Offer B = 25, Offer C = 20, Offer D = 35. At the 5% significance level, use a Chi-square goodness-of-fit test to determine whether preferences are equally distributed. (For df = 3, α = 0.05, χ² critical = 7.815.) Show all 5 steps, including your table of O, E, (O−E)², and (O−E)²/E.

**Q51.** A retail analyst investigates whether gender is associated with product preference:

| | Product X | Product Y |
|---|---|---|
| Male | 50 | 30 |
| Female | 20 | 40 |

At the 5% significance level, use a Chi-square test of independence to determine whether gender and product preference are associated. (For df = 1, α = 0.05, χ² critical = 3.841.) Show all 5 steps, including your expected-frequency table.

---

### Section 3A – Written / Interpretation Questions

**Q52.** A company wants to compare average monthly sales across **three** different regional teams (not two). Which technique from this unit would be appropriate, and why would a series of separate t-tests be a weaker choice for this situation? Name the test statistic this technique produces and, briefly, what it compares.

**Q53.** *(Long, ~10 marks)* An online retailer wants to know whether a website redesign increased the average order value. Using the 5-step hypothesis testing process taught in this unit, describe — in your own words and *without* doing the arithmetic — how the retailer would go about testing this claim, including: how they would state H₀ and H₁, what would determine their choice between a Z-test and a t-test, what a Type I error would mean in this specific business context, and how they would use the p-value to reach a business decision.


---

## UNIT 4 — LINEAR ALGEBRA (Session 10)

### Section 4D – Simple MCQs

**Q54.** Which of the following is a vector quantity (has both magnitude and direction)?
a) Mass
b) Temperature
c) Velocity
d) Distance

**Q55.** For matrix A to have an inverse, A must be:
a) Symmetric
b) Square with a non-zero determinant
c) Square with a determinant of zero
d) Any rectangular matrix

**Q56.** An eigenvector of a matrix is a vector that, when transformed by that matrix:
a) Becomes the zero vector
b) Is only scaled (not rotated), by a factor called the eigenvalue
c) Is rotated by exactly 90°
d) Always has magnitude 1

**Q57.** Cosine similarity between two vectors always falls in the range:
a) 0 to 1
b) −1 to 1
c) −∞ to ∞
d) 0 to 100

---

### Section 4C – Functional MCQs (justify your answer)

**Q58.** For matrices A (2×3) and B (3×2), the product AB will have dimensions:
a) 2×2
b) 3×3
c) 2×3
d) The product is undefined

**Q59.** If two vectors' dot product equals zero, the vectors are:
a) Parallel
b) Identical
c) Orthogonal (perpendicular)
d) Undefined

---

### Section 4B – Calculation Questions

**Q60.** Given v = (3, −2, 4) and w = (1, 5, −3):
(a) Calculate v + w.
(b) Calculate 2v − w.

**Q61.** Given a = 3i + 1j + 2k and b = 2i − 1j + 4k, calculate the dot product a · b.

**Q62.** Find the magnitude of the vector c = (6, 8, 0), and separately, the magnitude of d = (1, 2, 2).

**Q63.** Given p = (2, 2) and q = (3, −1):
(a) Calculate the dot product p · q.
(b) Calculate |p| and |q|.
(c) Use the dot product formula to find the angle θ between p and q. Are they orthogonal?

**Q64.** Two employees' skill profiles (Technical, Communication, Problem-Solving), each rated out of 5, are given as vectors: A = (4, 2, 5) and B = (3, 5, 4).
(a) Calculate the dot product A · B.
(b) Calculate the cosine similarity between A and B.
(c) Interpret what this cosine similarity value suggests about the two employees' skill profiles.

**Q65.** Given matrices A = [[2, 3], [1, 4]] and B = [[1, 0], [2, 5]] (each 2×2), calculate the matrix product AB.

**Q66.** Given the matrix M = [[5, 2, 7], [1, 9, 3]] (a 2×3 matrix), write out its transpose Mᵀ and state its dimensions.

**Q67.** Given matrix A = [[4, 3], [2, 5]]:
(a) Calculate the determinant of A.
(b) Based on your answer, state whether A is invertible.

**Q68.** Using the same matrix A = [[4, 3], [2, 5]] from Q67, calculate the inverse A⁻¹.

**Q69.** Given matrices A = [[4, 3], [2, 5]] and B = [[1, 0], [0, 6]]:
(a) Calculate tr(A) and tr(B).
(b) Calculate A + B, then tr(A + B).
(c) Confirm whether tr(A + B) = tr(A) + tr(B) for this example.

---

### Section 4A – Written / Interpretation Question

**Q70.** *(Long, ~10 marks)* A company rates two employees on Response Time and Communication (each out of 5): Employee A = (4, 5) and Employee B = (3, 4). Form a 2×2 matrix A using these two employees as rows (Employee A as row 1, Employee B as row 2).
(a) Calculate the transpose, determinant, trace, and inverse of this matrix.
(b) For each of the four operations, explain in one or two sentences its significance in data analysis or machine learning (e.g. where it is used, such as in linear regression or in studying covariance structures).

---

*(End of Part A — attempt every question above before turning to Part B.)*

---
---

# PART B: ANSWER SHEET

## Unit 1 — Probability: Answers

**Q1. Answer: b)** All elements of C are also in A.
*Why b is right:* This is the definition of a subset — every member of C must be found in A (C can even equal A).
*Why others are wrong:* (a) reverses the definition. (c) describes disjoint sets, not a subset relationship. (d) describes set equality, a special case, not the general subset definition.

**Q2. Answer: c) 0.7**
*Why right:* Complement rule: P(A′) = 1 − P(A) = 1 − 0.3 = 0.7.
*Why others wrong:* (a) repeats P(A) instead of complementing it. (b) is not derived from any rule here. (d) is impossible since probabilities cap at 1, and 0.3+0.7 must equal 1, not more.

**Q3. Answer: c) Rolling a 3 and rolling a 4**
*Why right:* A single die roll produces exactly one outcome, so getting a 3 and getting a 4 on the *same* roll cannot both happen — P(3 ∩ 4) = 0.
*Why others wrong:* (a) and (d) both describe overlapping events (e.g. 4 is even AND >3; 3 is odd AND prime) so they are not mutually exclusive. (b) also overlaps (2 is less than 3).

**Q4. Answer: b) Discrete**
*Why right:* The number of defective items is a count that can only take whole-number values (0, 1, 2, …, 50).
*Why others wrong:* (a) continuous variables take any value in a range (e.g. weight, time) — a count cannot. (c) and (d) are not valid categories; every random variable taught in this course is one or the other, not both/neither.

**Q5. Answer: b) Sum to 1**
*Why right:* This is the "total probability" property — the probabilities of all possible outcomes in a valid distribution must add to exactly 1.
*Why others wrong:* (a) and (c) impose an incorrect fixed value/threshold with no basis in the definition. (d) confuses probabilities (which are always between 0 and 1) with counts.

**Q6. Answer: c) 0.20**
*Justification:* Cold calls = 500 − 220 − 180 = 100. P(cold call) = 100/500 = 0.20.
*Why others wrong:* (a) 0.22 is P(social media). (b) 0.36 is P(social media)+something unrelated. (d) 0.44 is the combined proportion of social + referral leads, the complement of what's asked.

**Q7. Answer: c) 0.2**
*Justification:* For independent events, P(A ∩ B) = P(A) × P(B) = 0.5 × 0.4 = 0.20.
*Why others wrong:* (a) 0.9 is P(A)+P(B), the wrong rule (that would only be P(A∪B) for mutually exclusive events, which these are not). (b) 0.1 doesn't correspond to any valid operation on 0.5 and 0.4. (d) 0.45 is their average, not their product.

**Q8. Answer: b) 0.15**
*Justification:* P(A|B) = P(A∩B)/P(B) → P(A∩B) = P(A|B) × P(B) = 0.6 × 0.25 = 0.15.
*Why others wrong:* (a) 0.85 sums the two figures instead of multiplying. (c) 0.24 divides in the wrong direction (0.6/0.25 = 2.4, then misplaces the decimal, giving neither a valid nor requested value). (d) 2.4 is P(A|B)/P(B), an invalid probability (over 1) and not what's being asked.

---

**Q9.**
(a) P(on time) = 45/100 = **0.45**; P(late) = 30/100 = **0.30**; P(lost) = 25/100 = **0.25**.
(b) 0.45 + 0.30 + 0.25 = **1.00** ✓ — this confirms the three outcomes form a complete, valid set (they are exhaustive and mutually exclusive), satisfying the total probability property.
(c) P(not late) = 1 − P(late) = 1 − 0.30 = **0.70** (complement rule).
*Interpretation:* There is a 70% chance a randomly selected parcel either arrived on time or was lost — i.e., did not arrive late.

**Q10.**
(a) If the two events were independent, we would expect P(stay ∩ onboard) = P(stay) × P(onboard) = 0.68 × 0.90 = 0.612. The actual given value is 0.64, which is **not equal** to 0.612, so the two events are **not independent** — completing onboarding is associated with (slightly) higher retention than independence would predict.
*Value:* Expected-if-independent = 0.612 vs actual = 0.64 → the events are dependent.
*Explains:* Onboarding completion and 1-year retention move together more than chance would suggest.
*Conclusion:* The company should treat onboarding completion as a meaningful (if modest) predictor of retention, not something to ignore in workforce planning.
(b) P(stay | onboard) = P(stay ∩ onboard) / P(onboard) = 0.64 / 0.90 = **0.711** (71.1%).

**Q11.** P(satisfaction | hybrid) = 130/260 = **0.50**.
*Interpretation:* Among employees who work hybrid, there is a 50% chance that a randomly selected one reports high job satisfaction — hybrid work alone does not strongly predict satisfaction either way in this sample.

**Q12.**
Row/column totals: Loyalty card users = 90+60 = 150; No card = 40+160 = 200; Spent >$100 = 90+40 = 130; Spent ≤$100 = 60+160 = 220; Grand total = 350.
(a) P(>$100 | loyalty card) = 90/150 = **0.60**.
(b) P(loyalty card | >$100) = 90/130 ≈ **0.692**.
(c) These differ because they condition on different totals: (a) asks "of loyalty-card users, how many spend big?" (base = 150 card users), while (b) asks "of big spenders, how many use a card?" (base = 130 big spenders). Conditional probability is not symmetric — P(A|B) ≠ P(B|A) in general.

**Q13.**
(a) Sum of probabilities = 2k+3k+4k+k = 10k = 1 → **k = 0.1**.
(b) P(X=0)=0.2, P(X=1)=0.3, P(X=2)=0.4, P(X=3)=0.1.
(c) P(X≤2) = 0.2+0.3+0.4 = **0.9**.
(d) P(X>1) = 0.4+0.1 = **0.5**.
(e) This is a **PMF (probability mass function)** because X (number of complaints per day) is a discrete random variable — PMFs describe discrete distributions, while PDFs describe continuous ones.

**Q14.**
(a) 0.1+0.3+0.4+0.2 = 1.0 ✓ valid distribution.
(b) E(X) = (0×0.1)+(1×0.3)+(2×0.4)+(3×0.2) = 0+0.3+0.8+0.6 = **1.7**.
(c) *Value:* On average, 1.7 failed deliveries occur per shift. *Explains:* This is the long-run average outcome if the same pattern of failures continues shift after shift. *Conclusion:* The logistics manager should plan resourcing (e.g. a standby driver or buffer time) for roughly 2 failed deliveries per shift rather than assuming zero.

**Q15.**
(a) **Poisson** — this counts how many times an event (a login failure) happens in a fixed time interval (one hour), which is exactly the scenario the Poisson distribution models.
(b) **Normal** — heights are a continuous measurement that tends to cluster around an average in a bell-shaped, symmetric pattern across a large population.
(c) **Binomial** — there is a fixed number of trials (20 calls), each with the same two possible outcomes (success/failure) and a constant probability of success — the textbook Binomial setup.
(d) **Uniform** — each of the six outcomes on a fair die is equally likely, which is the defining feature of a (discrete) uniform distribution.

**Q16.** *Model answer:*
The telecoms company can frame each customer's contract status as an **event** within a **sample space** of all possible renewal/non-renewal outcomes across its customer base. Different customer segments (e.g. "has filed a complaint," "uses more than X GB/month") can be defined as events, and the company can study how these events relate to the event "renews contract" — for instance, are "complained in the last 3 months" and "renews contract" **independent**, or does one make the other more or less likely?

This is where **conditional probability** becomes central: rather than asking the *overall* renewal rate, the company can ask P(renews | filed a complaint) versus P(renews | no complaint). For example, suppose of 500 customers, 120 filed a complaint in the last quarter, and of those, 40 renewed; of the 380 who didn't complain, 300 renewed. Then P(renew | complaint) = 40/120 ≈ 0.33, versus P(renew | no complaint) = 300/380 ≈ 0.79. This large gap tells the company that complaints are strongly associated with churn, and that customer service intervention after a complaint is a high-leverage retention lever.

Beyond a single conditional probability, the company can build a full **probability distribution** for "number of renewals expected next quarter" across its customer base, using observed renewal rates as probabilities, which supports forecasting and resource planning (e.g. how many retention-team calls to budget).

*Limitation:* Probability calculated this way describes **association**, not necessarily **causation** — customers who complain may already be dissatisfied for reasons unrelated to the complaint itself (e.g. price sensitivity), so acting only on the correlation between complaints and churn, without further investigation (e.g. controlled experiments or regression controlling for other factors), risks misallocating retention resources.


---

## Unit 2 — Descriptive Statistics: Answers

**Q17. Answer: b) Population**
*Why right:* "All 40 employees" is the entire group of interest — nothing has been left out — which is the definition of a population.
*Why others wrong:* (a) A sample is a subset; here every employee is included. (c) and (d) — statistic and parameter are numbers *describing* a dataset, not the dataset itself.

**Q18. Answer: c) Parameter**
*Why right:* A parameter describes a whole population (true average income of *every* household), matching the definition exactly.
*Why others wrong:* (a) A statistic describes a sample, not a population. (b) A sample is data, not a descriptive number. (d) An estimate is what you use a *statistic* for, when you don't know the true parameter — it is not the parameter itself.

**Q19. Answer: c) Systematic sampling**
*Why right:* Selecting every kth (here, 8th) individual is the defining feature of systematic sampling.
*Why others wrong:* (a) Simple random sampling gives every individual an equal, independent chance, with no fixed pattern. (b) Stratified sampling requires dividing the population into subgroups first. (d) Convenience sampling selects whoever is easiest to reach, not a fixed interval.

**Q20. Answer: c) Positively (right) skewed**
*Why right:* When mean > median > mode, high-value outliers are pulling the mean up more than the median, which is the signature of a right (positive) skew — matches the empirical ordering taught in the course.
*Why others wrong:* (a) Symmetrical distributions have mean = median = mode. (b) Negative skew shows the reverse order (mean < median < mode). (d) Bimodal describes the number of modes, not skew direction, and isn't implied by this ordering.

**Q21. Answer: c) Platykurtic**
*Why right:* The course defines platykurtic as kurtosis < 3, with light tails and fewer outliers.
*Why others wrong:* (a) Leptokurtic is kurtosis > 3 (heavy tails, more outliers) — the opposite. (b) Mesokurtic is kurtosis ≈ 3 (normal-like tails), not < 3. (d) "Skewed" describes asymmetry, a different property from tail-heaviness.

**Q22. Answer: b) Stratified sampling**
*Justification:* The population is divided into meaningful subgroups (the 5 branches), and a sample is drawn from *each* subgroup in proportion to its size — this is the defining structure of stratified sampling.
*Why others wrong:* (a) Cluster sampling would randomly select a few whole branches and sample everyone within them, not draw proportionally from every branch. (c) Quota sampling is non-random — it fills fixed quotas without random selection within each group. (d) Snowball sampling relies on participants referring other participants, which isn't described here.

**Q23. Answer: a) 8**
*Justification:* Standard deviation = √variance = √64 = 8.
*Why others wrong:* (b) 32 is variance/2, not a valid transformation. (c) 4096 is variance squared (64²), the reverse operation. (d) 16 is variance/4, again not linked to the square-root rule.

**Q24. Answer: b)** The data represents a sample and we want an unbiased estimate of the population variance.
*Why right:* Dividing by (n − 1), sometimes called Bessel's correction, corrects the downward bias that occurs when estimating population variance from a sample.
*Why others wrong:* (a) A full population uses N in the denominator, not n − 1. (c) Whether n is even or odd is irrelevant to this choice. (d) The mean being zero has no bearing on which denominator to use.

---

**Q25.** Sorted data: 12, 15, 15, 15, 18, 20, 22, 25 (n = 8).
(a) Mean = (12+15+15+18+20+22+25+15)/8 = 142/8 = **17.75**.
(b) n is even, so median = average of 4th and 5th values = (15+18)/2 = **16.5**.
(c) Mode = **15** (appears three times, more than any other value).

**Q26.** fx values: 0×5=0, 1×12=12, 2×18=36, 3×10=30, 4×5=20. Σfx = 0+12+36+30+20 = 98. Σf = 50.
Mean = Σfx/Σf = 98/50 = **1.96 children per household**.

**Q27.**
Sorted data: 200, 220, 230, 240, 240, 260, 270, 1200 (n = 8).
(a) Mean = (200+220+230+240+240+260+270+1200)/8 = 2860/8 = **$357.50**. Median = avg of 4th & 5th = (240+240)/2 = **$240**. Mode = **$240** (appears twice).
(b) The **median (or mode), $240**, best represents the typical bonus. The single very high bonus of $1,200 is an outlier that pulls the mean up to $357.50 — well above what 7 of the 8 staff actually received — so the mean is misleading here.
(c) Mean ($357.50) > Median/Mode ($240), matching the mean > median > mode pattern, so the distribution is **positively (right) skewed** — the $1,200 outlier forms a long right-hand tail.

**Q28.** Empirical formula: Mode = 3×Median − 2×Mean = 3(58) − 2(62) = 174 − 124 = **50**.

**Q29.** Data (n=11): 18, 20, 22, 24, 25, 27, 28, 30, 32, 35, 60.
Median position = (11+1)/2 = 6th value = 27 (not needed further here, but confirms the split).
Lower half (first 5): 18, 20, 22, 24, 25 → median of these = **Q1 = 22**.
Upper half (last 5): 28, 30, 32, 35, 60 → median of these = **Q3 = 32**.
(a) Q1 = **22**, Q3 = **32**.
(b) IQR = Q3 − Q1 = 32 − 22 = **10**. QD = IQR/2 = **5**.
(c) Lower fence = Q1 − 1.5×IQR = 22 − 15 = **7**. Upper fence = Q3 + 1.5×IQR = 32 + 15 = **47**. The value **60 exceeds 47**, so **60 is an outlier**; no value falls below 7, so there is no low-end outlier.

**Q30.** Data: 3, 5, 4, 6, 2 (N = 5). Mean = (3+5+4+6+2)/5 = 20/5 = 4.
Deviations from mean: −1, 1, 0, 2, −2. Squared: 1, 1, 0, 4, 4. Sum of squares = 10.
(a) Population variance = 10/N = 10/5 = **2**.
(b) Population standard deviation = √2 ≈ **1.41**.

**Q31.** Data: 28, 32, 30, 35, 29, 31 (n = 6). Mean = (28+32+30+35+29+31)/6 = 185/6 ≈ 30.83.
Sum of squared deviations from the mean ≈ 30.83 (worked precisely: deviations −2.83, 1.17, −0.83, 4.17, −1.83, 0.17; squares sum to ≈30.83).
(a) Sample variance = Σ(x−x̄)²/(n−1) = 30.83/5 ≈ **6.17**.
(b) Sample standard deviation = √6.17 ≈ **2.48 minutes**.
(c) These 6 orders are treated as a **sample** drawn from a larger population of possible orders, so dividing by (n − 1) gives an *unbiased* estimate of the true population variance. In Q30, the 5 days were treated as the *entire population* of interest, so N was used in the denominator instead — the choice of denominator depends on whether your data is the whole population or only a sample of it.

**Q32.**
Machine A: 495, 500, 505, 498, 502. Mean = 500. Population SD ≈ **3.41 g**.
Machine B: 470, 510, 530, 480, 510. Mean = 500. Population SD ≈ **21.91 g**.
(a) Mean of both machines = 500 g (identical). SD: Machine A ≈ 3.41 g, Machine B ≈ 21.91 g.
(b) CV = (SD/mean) × 100. Machine A: (3.41/500)×100 ≈ **0.68%**. Machine B: (21.91/500)×100 ≈ **4.38%**.
(c) *Value:* Machine A's CV (0.68%) is much lower than Machine B's (4.38%). *Explains:* A lower coefficient of variation means less relative spread around the mean, i.e. more consistent fill weights. *Conclusion:* **Machine A is more consistent** and should be preferred (or investigated as the benchmark) for quality control, even though both machines hit the same average target.

**Q33.**
Mean X = (3+4+5+6+7+8)/6 = 33/6 = **5.5**. Mean Y = (22+25+29+33+35+40)/6 = 184/6 ≈ **30.67**.
(a) As above.
(b) Deviations and products (x−x̄)(y−ȳ) sum to 62; population covariance = 62/6 ≈ **10.33**. *(Working: deviations in X are −2.5,−1.5,−0.5,0.5,1.5,2.5; in Y are −8.67,−5.67,−1.67,2.33,4.33,9.33; their products are 21.67, 8.5, 0.83, 1.17, 6.5, 23.33, summing to ≈62.)*
(c) Population SD of X ≈ 1.708; population SD of Y ≈ 6.074. Pearson r = covariance/(SDx×SDy) = 10.33/(1.708×6.074) ≈ **0.996**.
(d) *Value:* r ≈ 0.996. *Explains:* This is extremely close to +1, indicating an almost perfectly linear, **positive** relationship — as advertising spend rises, website visits rise almost in lockstep. *Conclusion:* Advertising spend is a very strong (near-perfect) predictor of website visits **in this sample**, making it a reasonable variable to build forecasts or budget decisions around, subject to the causation caveat discussed in Q34.

**Q34.** *Model answer:*
No — a strong correlation (r ≈ 0.996 from Q33) shows that advertising spend and website visits **move together very closely**, but it does not by itself prove that higher advertising *causes* more visits. Both variables could be driven by a third factor — for example, a seasonal sales period might simultaneously justify higher ad budgets *and* independently attract more visits (e.g. a holiday shopping season), which would produce a strong correlation without spend being the cause. It's also possible the relationship runs partly in reverse: a company might increase ad spend *in response* to early signs of rising interest.
To move from correlation towards causation, the company would need additional evidence such as a **controlled experiment** (e.g. running higher ad spend in one region and a matched control region with unchanged spend, then comparing visit growth), or a regression model that statistically controls for other likely drivers (season, promotions, competitor activity) to isolate advertising's own effect.
Separately, before trusting this correlation at all, the company should draw a **boxplot** of the website-visit data to check for unusual months — a single unusually high or low month (an outlier) can distort both the calculated covariance and the correlation coefficient, since these measures are sensitive to extreme values. Confirming there are no such outliers (or investigating and explaining any that appear) makes the correlation result more trustworthy before it is used to justify spending decisions.


---

## Unit 3 — Inferential Statistics: Answers

**Q35. Answer: c)** Draw conclusions about a population using sample data.
*Why right:* This is the textbook definition given in the course — inferential statistics uses sample information to estimate, predict, or conclude something about a larger population.
*Why others wrong:* (a) and (d) describe descriptive statistics, not inferential. (b) undersells it — inferential statistics goes *beyond* the sample to say something about the population, not just describe the sample.

**Q36. Answer: b)** Approaches a normal distribution, regardless of the population's shape.
*Why right:* This is the precise statement of the Central Limit Theorem taught in the course.
*Why others wrong:* (a) is the opposite of what CLT predicts. (c) confuses the sampling distribution of the *mean* with the population distribution itself — they need not match. (d) is incorrect; the sampling distribution's SD (the standard error) is *smaller* than the population SD, equal to σ/√n.

**Q37. Answer: a)** We reject H₀ when H₀ is actually true.
*Why right:* This matches the course's definition of Type I error exactly.
*Why others wrong:* (b) describes a Type II error. (c) describes a *correct* decision (correctly rejecting a false H₀), not an error. (d) also describes a correct decision, not an error type.

**Q38. Answer: b)** Reject H₀ — result is statistically significant.
*Why right:* The decision rule is p < α → reject H₀. Here 0.03 < 0.05, so H₀ is rejected.
*Why others wrong:* (a) applies the rule backwards. (c) is unnecessary — the test already gives a clear decision at this significance level. (d) overstates the conclusion; rejecting H₀ supports H₁ statistically, it doesn't "prove" it is definitely true.

**Q39. Answer: d) Nominal**
*Why right:* Marital status categories have no inherent ranking or order — "Married" isn't higher or lower than "Single" — which is the definition of a nominal scale.
*Why others wrong:* (a) Ratio scales are numeric with a true zero (e.g. income). (b) Interval scales are numeric with equal spacing but no true zero (e.g. temperature °C). (c) Ordinal scales have categories *with* a meaningful order (e.g. Low/Medium/High), which marital status does not have.

**Q40. Answer: d) 12**
*Justification:* SE = σ/√n = 36/√144 = 36/12 = 12.
*Why others wrong:* (a) 36 is the population SD itself, not the standard error. (b) 3 would result from an arithmetic slip (e.g. 36/12 miscalculated). (c) 0.25 inverts the calculation (√144/36).

**Q41. Answer: b)** t-test, because the population SD is unknown and the sample is small.
*Justification:* The course's decision rule is: use a t-test when σ is unknown and/or the sample is small (n < 30); here both conditions hold (n=14, σ unknown).
*Why others wrong:* (a) Z-tests require σ known and/or a large sample — neither applies. (c) Chi-square tests are for categorical data, not a continuous mean like commute time. (d) F-tests/ANOVA compare variances or 3+ means, not a single mean against a claimed value.

**Q42. Answer: b)** Z-test — large sample and population SD is known.
*Justification:* n = 60 ≥ 30 and σ is stated as known — both are the defining conditions for a Z-test in this course.
*Why others wrong:* (a) t-tests are used specifically when σ is *unknown*, which isn't the case here. (c) Chi-square applies to categorical/count data, not a continuous fill weight. (d) Paired t-tests require the *same* items measured twice (e.g. before/after), which isn't described here.

---

**Q43.**
(a) SE = σ/√n = 45/√81 = 45/9 = **5 minutes**.
(b) The sampling distribution of the sample mean will be **approximately normal**, per the Central Limit Theorem, which generally holds once the sample size is **n ≥ 30** (here, n = 81 comfortably satisfies this).

**Q44.**
(a) H₀: μ = 4 minutes; H₁: μ ≠ 4 minutes. **Two-tailed** (testing for any difference, not a specific direction).
(b) H₀: μ ≤ 15 hours; H₁: μ > 15 hours. **One-tailed** (right-tailed — the claim specifies a direction, "more than").
(c) H₀: μ₁ = μ₂ (no difference between departments); H₁: μ₁ ≠ μ₂. **Two-tailed** (testing for any difference, no direction specified).

**Q45.** For 99% confidence, α = 1 − 0.99 = **0.01**. The corresponding two-tailed critical z-value is **±2.576**.

**Q46.**
Step 1 — Hypotheses: H₀: μ = 500 g; H₁: μ ≠ 500 g (two-tailed).
Step 2 — Significance & critical value: α = 0.05, two-tailed → z-critical = **±1.96**.
Step 3 — Test statistic: z = (x̄ − μ)/(σ/√n) = (495 − 500)/(12/√36) = (−5)/(12/6) = (−5)/2 = **−2.50**.
Step 4 — Compare: |−2.50| = 2.50 > 1.96, so the test statistic falls in the rejection region.
Step 5 — Conclusion: **Reject H₀.** There is sufficient evidence at the 5% significance level to conclude that the average capsule weight differs significantly from 500 g (the sample suggests capsules are, on average, underfilled).

**Q47.**
Data: 42, 39, 41, 44, 38, 40, 43, 45 (n = 8). Mean x̄ = (42+39+41+44+38+40+43+45)/8 = 332/8 = **41.5**. Sample SD s ≈ **2.449**.
Step 1 — Hypotheses: H₀: μ = 40; H₁: μ ≠ 40 (two-tailed).
Step 2 — Significance & critical value: α = 0.05, df = n−1 = 7, two-tailed → t-critical = **±2.365** (given).
Step 3 — Test statistic: t = (x̄ − μ)/(s/√n) = (41.5 − 40)/(2.449/√8) = 1.5/0.866 ≈ **1.73**.
Step 4 — Compare: |1.73| = 1.73 < 2.365, so the test statistic does **not** fall in the rejection region.
Step 5 — Conclusion: **Fail to reject H₀.** There is insufficient evidence at the 5% significance level to conclude the true mean completion time differs from 40 hours — the bootcamp provider's claim cannot be rejected based on this sample.

**Q48.**
Method A: 68, 72, 75, 70, 74 → mean x̄₁ = 71.8, sample SD s₁ ≈ 2.864.
Method B: 60, 65, 63, 67, 62 → mean x̄₂ = 63.4, sample SD s₂ ≈ 2.702.
Step 1 — Hypotheses: H₀: μ₁ = μ₂; H₁: μ₁ ≠ μ₂ (two-tailed).
Step 2 — Significance & critical value: α = 0.05, df = n₁+n₂−2 = 8, two-tailed → t-critical = **±2.306** (given).
Step 3 — Test statistic: SE = √(s₁²/n₁ + s₂²/n₂) = √(2.864²/5 + 2.702²/5) = √(1.640+1.461) ≈ 1.761. t = (x̄₁ − x̄₂)/SE = (71.8 − 63.4)/1.761 = 8.4/1.761 ≈ **4.77**.
Step 4 — Compare: |4.77| = 4.77 > 2.306, so the test statistic falls well within the rejection region.
Step 5 — Conclusion: **Reject H₀.** There is sufficient evidence at the 5% significance level to conclude a significant difference in average scores between the two training methods; Method A (mean 71.8) outperforms Method B (mean 63.4) in this sample.

**Q49.**
Differences (After − Before): 63−58=5, 65−62=3, 64−60=4, 68−65=3, 65−63=2. d̄ = (5+3+4+3+2)/5 = 17/5 = **3.4**. Sample SD of differences, sᵈ ≈ **1.140**.
Step 1 — Hypotheses: H₀: μd ≤ 0 (no increase / decrease in scores); H₁: μd > 0 (scores increased). *(One-tailed, since the coach is testing for an increase specifically.)*
Step 2 — Significance & critical value: α = 0.05, df = n−1 = 4, one-tailed → t-critical = **2.132** (given).
Step 3 — Test statistic: t = d̄/(sᵈ/√n) = 3.4/(1.140/√5) = 3.4/0.510 ≈ **6.67**.
Step 4 — Compare: 6.67 > 2.132, so the test statistic falls in the rejection region.
Step 5 — Conclusion: **Reject H₀.** There is sufficient evidence at the 5% significance level that employee stress scores significantly increased after the mindfulness programme — meaning, since higher scores are worse in this scale, the programme **appears to have made stress scores worse, not better**, and this counter-intuitive result should prompt the coach to check whether "stress score" is scaled correctly or investigate the programme design before drawing further conclusions.

**Q50.**
Expected frequency per category = 120/4 = **30** for each of A, B, C, D.

| Offer | O | E | (O−E) | (O−E)² | (O−E)²/E |
|---|---|---|---|---|---|
| A | 40 | 30 | 10 | 100 | 3.33 |
| B | 25 | 30 | −5 | 25 | 0.83 |
| C | 20 | 30 | −10 | 100 | 3.33 |
| D | 35 | 30 | 5 | 25 | 0.83 |
| **Total** | 120 | 120 | | | **8.33** |

Step 1 — Hypotheses: H₀: preferences are equally distributed across the 4 offers; H₁: preferences are not equally distributed.
Step 2 — Significance & critical value: α = 0.05, df = k−1 = 3 → χ² critical = **7.815** (given).
Step 3 — Test statistic: χ² = Σ(O−E)²/E ≈ **8.33**.
Step 4 — Compare: 8.33 > 7.815, so the calculated value exceeds the critical value.
Step 5 — Conclusion: **Reject H₀.** There is sufficient evidence at the 5% significance level that customer preferences are **not** equally distributed across the four promotional offers — Offer A is notably over-preferred and Offer C under-preferred relative to an equal split, which should inform which promotion the store leads with.

**Q51.**
Row totals: Male = 80, Female = 60. Column totals: Product X = 70, Product Y = 70. Grand total = 140.
Expected frequencies (E = Row Total × Column Total / Grand Total): E(Male,X) = 80×70/140 = 40; E(Male,Y) = 80×70/140 = 40; E(Female,X) = 60×70/140 = 30; E(Female,Y) = 60×70/140 = 30.

| Cell | O | E | (O−E)² | (O−E)²/E |
|---|---|---|---|---|
| Male, X | 50 | 40 | 100 | 2.50 |
| Male, Y | 30 | 40 | 100 | 2.50 |
| Female, X | 20 | 30 | 100 | 3.33 |
| Female, Y | 40 | 30 | 100 | 3.33 |
| **Total** | 140 | 140 | | **11.67** |

Step 1 — Hypotheses: H₀: gender and product preference are independent; H₁: gender and product preference are associated.
Step 2 — Significance & critical value: α = 0.05, df = (r−1)(c−1) = (2−1)(2−1) = 1 → χ² critical = **3.841** (given).
Step 3 — Test statistic: χ² = Σ(O−E)²/E ≈ **11.67**.
Step 4 — Compare: 11.67 > 3.841, so the calculated value clearly exceeds the critical value.
Step 5 — Conclusion: **Reject H₀.** There is sufficient evidence at the 5% significance level that gender and product preference are significantly associated — men in this sample show a stronger preference for Product X, and women for Product Y, which the retail analyst could use to inform targeted marketing.

**Q52.** **One-way ANOVA (Analysis of Variance)** is appropriate here, since the company wants to compare means across **three or more** groups at once. Running separate pairwise t-tests (A vs B, A vs C, B vs C) instead would **inflate the overall Type I error rate** — each individual test carries its own 5% chance of a false positive, so running multiple tests raises the *combined* chance of wrongly finding at least one "significant" difference well above 5%. ANOVA avoids this by testing all groups simultaneously in a single test, producing an **F statistic**, which compares the variance *between* group means to the variance *within* groups to determine whether at least one group mean differs significantly from the others.

**Q53.** *Model answer:*
The retailer would begin by stating a **null hypothesis (H₀)**: that the redesign made no difference to average order value (μ_after = μ_before, or equivalently μ_after ≤ μ_before if only testing for improvement), against an **alternative hypothesis (H₁)** that average order value increased after the redesign — likely a one-tailed test, since the retailer's specific interest is whether the redesign *improved* order value, not simply changed it in either direction.

The choice between a **Z-test and a t-test** would depend on whether the population standard deviation of order values is known and on the sample size: if the retailer has a very large volume of historical order data with a well-established population SD, a Z-test would be appropriate; more realistically, since the true population SD of order values is unlikely to be known precisely and the comparison may involve a moderate sample of orders (e.g. from a limited testing period), a **t-test** would be used — most naturally a paired t-test if the same set of customers' before/after behaviour is tracked, or an independent two-sample t-test if before/after refer to two different, unrelated groups of customers.

A **Type I error** in this specific context would mean concluding the redesign increased order value when it actually had no real effect — this could lead the retailer to permanently roll out a costly redesign, or to credit the redesign for a change that was really due to seasonality, promotions, or chance.

Finally, the retailer would compare the resulting **p-value** to their chosen significance level (commonly α = 0.05): if p < α, they would reject H₀ and conclude the redesign significantly increased order value, giving them evidence-based grounds to keep the redesign; if p ≥ α, they would fail to reject H₀, meaning the observed increase (if any) is not statistically distinguishable from random variation, and the retailer should be cautious about attributing any change to the redesign itself.


---

## Unit 4 — Linear Algebra: Answers

**Q54. Answer: c) Velocity**
*Why right:* Velocity has both a magnitude (speed) and a direction, which is the definition of a vector quantity.
*Why others wrong:* (a) Mass, (b) Temperature, and (d) Distance are all scalar quantities — they have magnitude only, no direction (note: distance is a scalar; its directional counterpart, displacement, would be the vector).

**Q55. Answer: b)** Square with a non-zero determinant.
*Why right:* This is the precise condition given in the course: a matrix must be square, and det(A) ≠ 0, for A⁻¹ to exist.
*Why others wrong:* (a) Symmetry is unrelated to invertibility — symmetric matrices can be singular, and non-symmetric matrices can be invertible. (c) A zero determinant means the matrix is **not** invertible — the opposite of what's needed. (d) Rectangular (non-square) matrices don't have a standard inverse at all.

**Q56. Answer: b)** Is only scaled (not rotated), by a factor called the eigenvalue.
*Why right:* This matches the course's definition exactly — an eigenvector's *direction* is unchanged by the transformation; only its magnitude changes, by the eigenvalue.
*Why others wrong:* (a) The zero vector is a trivial/excluded case, not the definition of an eigenvector. (c) A 90° rotation would change the vector's direction, which contradicts the definition of an eigenvector. (d) Eigenvectors are not required to have magnitude 1 (they can be scaled to any length and remain eigenvectors).

**Q57. Answer: b) −1 to 1**
*Why right:* This matches the course's stated range for cosine similarity, with +1 meaning same direction, 0 meaning orthogonal, and −1 meaning opposite direction.
*Why others wrong:* (a) 0 to 1 is too narrow — it excludes the valid negative-similarity case. (c) −∞ to ∞ is the range of an unbounded quantity, not cosine, which is always bounded. (d) 0 to 100 confuses cosine similarity with a percentage scale.

**Q58. Answer: a) 2×2**
*Justification:* For A (m×n) multiplied by B (n×p), the result is (m×p). Here A is 2×3 and B is 3×2, so the result is 2×2. Critically, the **inner dimensions must match** (3 = 3 here), which they do, so the product is defined.
*Why others wrong:* (b) 3×3 would result if the matrices were multiplied in the reverse order (BA instead of AB). (c) 2×3 incorrectly keeps A's own dimensions. (d) The product **is** defined, since the inner dimensions (3 and 3) match.

**Q59. Answer: c) Orthogonal (perpendicular)**
*Why right:* A dot product of zero is precisely the algebraic test for perpendicularity between two vectors, as taught in the course.
*Why others wrong:* (a) Parallel vectors have a dot product equal to ±(|v||w|), not zero (unless one vector is the zero vector). (b) Identical vectors have a dot product equal to the square of their magnitude, not zero. (d) The dot product is always defined for vectors of matching dimension — a zero result is a valid, meaningful outcome, not an error.

---

**Q60.** v = (3, −2, 4), w = (1, 5, −3).
(a) v + w = (3+1, −2+5, 4+(−3)) = **(4, 3, 1)**.
(b) 2v = (6, −4, 8). 2v − w = (6−1, −4−5, 8−(−3)) = **(5, −9, 11)**.

**Q61.** a·b = (3×2) + (1×−1) + (2×4) = 6 − 1 + 8 = **13**.

**Q62.** |c| = √(6² + 8² + 0²) = √(36+64+0) = √100 = **10**.
|d| = √(1² + 2² + 2²) = √(1+4+4) = √9 = **3**.

**Q63.**
(a) p·q = (2×3) + (2×−1) = 6 − 2 = **4**.
(b) |p| = √(2²+2²) = √8 ≈ **2.828**. |q| = √(3²+(−1)²) = √10 ≈ **3.162**.
(c) cos θ = (p·q)/(|p||q|) = 4/(2.828×3.162) = 4/8.944 ≈ **0.447**. θ = cos⁻¹(0.447) ≈ **63.4°**. Since cos θ ≠ 0 (and θ ≠ 90°), **the vectors are not orthogonal**.

**Q64.**
(a) A·B = (4×3)+(2×5)+(5×4) = 12+10+20 = **42**.
(b) |A| = √(4²+2²+5²) = √45 ≈ 6.708. |B| = √(3²+5²+4²) = √50 ≈ 7.071. Cosine similarity = 42/(6.708×7.071) = 42/47.44 ≈ **0.885**.
(c) *Value:* Cosine similarity ≈ 0.885, close to +1. *Explains:* This indicates the two employees' skill profiles point in a very similar "direction" — their relative strengths and weaknesses across Technical, Communication, and Problem-Solving are patterned similarly, even though their raw scores differ slightly. *Conclusion:* For tasks needing a specific skill *pattern* (rather than raw skill level), these two employees could likely be considered close substitutes for one another, or grouped together for similar training/role assignments.

**Q65.** A = [[2,3],[1,4]], B = [[1,0],[2,5]].
Row 1 of A times columns of B: (2×1 + 3×2, 2×0 + 3×5) = (2+6, 0+15) = (8, 15).
Row 2 of A times columns of B: (1×1 + 4×2, 1×0 + 4×5) = (1+8, 0+20) = (9, 20).
AB = **[[8, 15], [9, 20]]**.

**Q66.** M = [[5, 2, 7], [1, 9, 3]] is 2×3. Its transpose interchanges rows and columns:
Mᵀ = **[[5, 1], [2, 9], [7, 3]]**, which is **3×2**.

**Q67.** A = [[4,3],[2,5]].
(a) det(A) = (4×5) − (3×2) = 20 − 6 = **14**.
(b) Since det(A) = 14 ≠ 0, **A is invertible**.

**Q68.** For A = [[4,3],[2,5]], det(A) = 14 (from Q67). Using the 2×2 inverse formula A⁻¹ = (1/det(A)) × [[d, −b], [−c, a]] for A = [[a,b],[c,d]]:
A⁻¹ = (1/14) × [[5, −3], [−2, 4]] = **[[5/14, −3/14], [−2/14, 4/14]]** ≈ [[0.357, −0.214], [−0.143, 0.286]].

**Q69.** A = [[4,3],[2,5]], B = [[1,0],[0,6]].
(a) tr(A) = 4+5 = **9**. tr(B) = 1+6 = **7**.
(b) A+B = [[4+1, 3+0],[2+0, 5+6]] = [[5,3],[2,11]]. tr(A+B) = 5+11 = **16**.
(c) tr(A) + tr(B) = 9 + 7 = 16 = tr(A+B). **Confirmed** — this illustrates the general property tr(A+B) = tr(A) + tr(B) taught in the course.

**Q70.**
Matrix: A = [[4, 5], [3, 4]] (Employee A = row 1, Employee B = row 2; columns = Response Time, Communication).
(a)
- **Transpose:** Aᵀ = [[4, 3], [5, 4]].
- **Determinant:** det(A) = (4×4) − (5×3) = 16 − 15 = **1**.
- **Trace:** tr(A) = 4 + 4 = **8**.
- **Inverse:** Since det(A) = 1 ≠ 0, A is invertible: A⁻¹ = (1/1) × [[4, −5], [−3, 4]] = **[[4, −5], [−3, 4]]**.

(b) *Significance of each operation:*
- **Transpose** rearranges the data so that, for example, features become rows and observations become columns (or vice-versa); this reshaping is essential for matrix multiplication to line up correctly, and expressions like XᵀX appear directly in the normal equation for linear regression.
- **Determinant** tells us whether this matrix can be inverted at all (non-zero here, so it can) — in general it signals whether a system built from this data has a unique solution, which matters when solving for model coefficients.
- **Trace** (the sum of the diagonal) is used in areas like covariance matrices and dimensionality-reduction techniques, where the diagonal often represents each feature's own variance, so the trace summarises total variance captured.
- **Inverse** allows us to "undo" the matrix — in machine learning this is what lets a linear regression model solve directly for its coefficients (weights) from the input data, rather than searching for them iteratively.

---
*(End of Answer Sheet.)*
