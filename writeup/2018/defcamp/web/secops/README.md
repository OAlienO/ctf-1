# Task Info
secops - 20 solves - 316 pts

## Time
3 hours  
For trying different bypass methods

# Solution
The cookie is a json object which has a key `flair` storing the selected ID.
One of my team-mate(@shw) told me that there's SQL injection in item `flair`.
There's a WAF to filter injection payload.
To bypass it, I use:
```
' or #\n [payload]
```
The WAF thinks the payload is comment but it isn't.
Then just bruteforce each bytes to get the flag.

# Additional Notes
There's a better solution to bypass the WAF -- \u unicode encode in json.
