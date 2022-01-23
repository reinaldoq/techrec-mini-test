# Redsift Python Software Engineer (Product) mini-test

This is a quick test consisting of 3 tasks that should take no longer than 15 minutes to complete.

What skills are we looking for?

- Analytic Skills - How can you think through problems and analyze things?
- Coding Skills - Do you code well, by writing clean, simple, organized, readable code?
- Technical knowledge - Do you know the fundamentals and understand code performance?

## Task 1

Count how many Apples, Pears, Lemons, Oranges, Pineapples, Tomatoes, Mangos and Bananas are in the list.

```
Expected output:
Apple: 2,
Pear: 3
Lemon: 2,
Orange: 1,
Pineapple: 2,
Tomato: 1,
Mango: 1
Banana: 0
```

```python
task1 = [
  "apple",
  "pear",
  "lemon",
  "orange",
  "pineapple",
  "tomato",
  "lettuce",
  "mango",
  "apple",
  "pineapple",
  "lemon",
  "pear",
  "pear",
]
```

## Task 2

a) What is the performance, in terms of, Big O notation, of the below code? 
b) Write a solution that has better performance
c) What is the performance of your new solution?

Tip: To show your thinking, write the performance of each line of the function.

```python
# Example to show data shape only.
domains = {
   "one.com": dict(policy="block"),
   "two.com": dict(policy="none"),
   "three.com": dict(policy="none"),
   "four.com": dict(policy="block")
}

def getBlockPolicyState(domains):
  policyArr = []
  numDomains = len(domains.keys())
  for x in range(numDomains):
    policy = domains.values()[x]["policy"]
    policyArr.append(policy)
  oneDomain = [True for policy in policyArr if policy == "block"]
  allDomains = all(policy == "block" for policy in policyArr)
  return dict(oneDomain=oneDomain, allDomains=allDomains)
```

## Task 3

Find the first recurring character of the below lists

```python
task3 = [
  [2,5,1,2,3,5,1,2,4], # Should return 2
  [2,1,1,2,3,5,1,2,4], # Should return 1
  [2,3,4,5], # Should return None
  [2,5,5,2,3,5,1,2,4] # Should return 5
]
```