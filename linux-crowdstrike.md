SE Linux and Falcon
- SE Linux Enforcing and not permissive
- SE Linux will try and block the Falcon process.
- SE Linux Policy
    - Processed based security
    - every process that's spun up.
    - The only way to be granted admin access is to have an auth key granted from ansible server.
    - The server is protected and only handling traffic on specific ports (over SSH).
- Running on permissive mode would allow us to run falcon but in reporting mode with no actions taken.


- No log4j no vulnerabilities
- 