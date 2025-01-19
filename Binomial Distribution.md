This is a simple discrete distribution applied to repeated, independent and random trials without replacement.
> The trials could happen simultaneously also, like rolling a bunch of die, we just choose to look at them as repeated

Also, the only way this works as *binomial* is if there are only two states - success or failure.
The main idea behind this is that if we have a number of successes and failures in a number of independent scenarios, they can be arranged in a number of ways - combinations

mean = np
variance = np(1-p)
where n = number of trials, p = probability of success

## Problems
### Question 1
Heart failure is due to either natural occurrences(87%) or other occurrences(13%). Suppose 20 patients are admitted to an emergency room with heart failure. What is the probability that 3 or more of them have other occurrences based heart failure?

![[Pasted image 20240910100420.png]]