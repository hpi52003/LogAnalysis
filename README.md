The code analyzes a log file to extract insights about IP activity, endpoint usage, and suspicious behaviors. The below procedure indicates step by step process

1. **Read the Log File**:
   - The log file is read line by line and stored as a list of strings.

2. **Analyze the Logs**:
   - **Count Requests per IP**: Extracts all IP addresses using a regular expression and counts how many times each IP appears in the logs.
   - **Find Most Accessed Endpoint**: Identifies and counts the occurrences of HTTP endpoints (e.g., `/home`) to find the most accessed one.
   - **Detect Suspicious Activities**: Searches for log entries indicating failed login attempts and counts them by IP.

3. **Save Results to CSV**:
   - The analysis results are formatted and written into a CSV file. This includes:
     - A table of requests per IP.
     - The most accessed endpoint and its count.
     - A table of failed login attempts by IP.

4. **Execute the Main Function**:
   - The process begins when the script is executed, calling the `main()` function.
   - The log file is analyzed, and results are saved into a CSV file.
