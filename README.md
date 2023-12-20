# MemoryVulnerabilities

In this project I detected and exploited memory vulnerabilities in a series of programs on a virtual machine including identifying locations to insert compromising shell code even with safety mechanisms such as canaries and ASLR enabled. 

Through this project, I exploited the following vulnerabilities:
1. Buffer Overflows (not checking the end length of a buffer in C before loading user input)
2. Stack smashing (overwriting the esp/eip to redirect to an inserted code segment after this stack frame is closed)
3. Format String Vulnerabilities (exploting the printf() variable arguments to print items off the stack like the canary)
4. Integer Conversion Vulnerabilities (signed <-> unsigned errors can be used to buffer overflow)
5. Off by One Vulnerabilities

The design document is provided in the repository and the code can also be provided upon request. 
