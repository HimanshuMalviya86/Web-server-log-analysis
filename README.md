# Web-server-log-analysis
Tools Used:
Python (main language)
Pandas: for data manipulation
Regex (re): for parsing logs
Datetime: for working with timestamps
File I/O & Exception Handling: for robust execution

Approach:
I used Python’s re module with a compiled regex pattern to match fields like host, timestamp, request, status code, and response size. Each line was checked against the pattern, and matched groups were stored in a dictionary, which I later converted to a pandas DataFrame.

Challenges:
Parsing inconsistent or malformed lines was a challenge, which I handled by segregating invalid lines. Also, converting timestamps to timezone-aware datetime was tricky but necessary for accurate grouping and filtering.
