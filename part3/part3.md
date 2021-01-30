# DevTools - Debugging
1. The bug is that the inputs are for `num1` and `num2` are both evaluated as strings. From the watchlist we can see this when the `typeof(result)` is a string after we evaluate the sum. So instead of numeric addition we are concatenating the two inputs as strings.
2. To fix this I would cast `num1` and `num2` to Number when adding them and storing them into `result`. See screenshot.

# DevTools - Network Tab
1. citylots.json
2. part2.js:2
3. 11.7 MB
4. 532ms
5. User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.141 Safari/537.36
6. Apache
7. Last-Modified: Tue, 26 Jan 2021 22:14:13 GMT
8. Content-Type: application/json
9. fetchData