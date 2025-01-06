## Hi there 👋
Welcome to my GitHub profile, where the code flows smoothly... until it doesn't. Sometimes, **segfaults** are just a reminder that even the most carefully crafted code can stumble when you try to reach the forbidden. 

### Most used languages
As every true developer knows: **you're not a real developer until you've faced a segfault**. It’s the moment you realize that, just like a hacker trying to break into a secure system, you have to understand the rules of memory or risk getting caught.

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=albrinBuzz&layout=compact&theme=dark)

---

### 💥 Segfault Error: A Hacker's Rite of Passage

```bash
$ gcc hack_exploit.c -o breach_tool
$ ./breach_tool
Segmentation Fault (core dumped)

# Debugging with GDB:
$ gdb ./breach_tool
(gdb) run
Starting program: /home/user/breach_tool

Program received signal SIGSEGV, Segmentation fault.
0x0040056f in main () at hack_exploit.c:10
10      memcpy(ptr, "access_granted", 19);  // Attempting to hack into the system's hidden vault

(gdb) backtrace
#0  0x0040056f in main () at hack_exploit.c:10
(gdb) quit
