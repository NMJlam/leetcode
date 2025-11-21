## Describe the question
The question is asking me to return the longest common prefix in a list of words

# Test cases
```python
arr = ["nathan", "natalie", "natasha"]
return "nat"
```

```python
arr = ["cat", "dog", "turtle"]
return ""
```

## Approach
1) Assume that the first word is the longest common prefix
2) Iterate through the rest of the list
		- If there is a mismatch: reduce the lcp by 1
		- If there is a match: beyond the lcp extend it by 1
Complexity: $O(N * L)$, where $L$ is the length of each word

