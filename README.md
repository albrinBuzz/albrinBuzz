## Este texto lo generó ChatGPT, porque no se me ocurre un pija

## ¡Hola, peluca! 👋

### Lenguajes más utilizados
Como bien dice Linus Torvalds: **"No eres un verdadero desarrollador hasta que te enfrentas a un segfault"**.

Y como diría el Bananero: **"¡Pero qué hacés, peluca! ¿No sabés ni escribir un 'Hola Mundo' en Python y ya te metés a hacer 'multithreading' en Java? ¡Sos un Trolazo, sape!"**

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=albrinBuzz&layout=compact&theme=dark)

---

### 💥 Segfault Error: A Hacker's Rite of Passage

```bash
$ gcc exploit_craft.c -o breach_tool
$ ./breach_tool
Segmentation Fault (core dumped)

# Debugging with GDB:
$ gdb ./breach_tool
(gdb) run
Starting program: /home/user/breach_tool

Program received signal SIGSEGV, Segmentation fault.
0x0040056f in main () at exploit_craft.c:14
14       strcpy(unsafe_buffer, "This string is way too long for the buffer!");

(gdb) backtrace
#0  0x0040056f in main () at exploit_craft.c:14
#1  0x7ffff7e1c10b in __libc_start_main (main=0x40056e <main()>, argc=1, argv=0x7fffffffde88, 
    init=<optimized out>, fini=<optimized out>, rtld_fini=<optimized out>, stack_end=0x7fffffffde78)
    at ../csu/libc-start.c:308
#2  0x00400539 in _start () at exploit_craft.c:2

(gdb) disassemble 0x0040056f, +32
Dump of assembler code from 0x40056f to 0x40058f:
   0x0040056f <+0>:   mov    rdi,0x0
   0x00400573 <+4>:   mov    rsi,0x0
   0x00400577 <+8>:   mov    rdx,0x0
   0x0040057b <+12>:  call   0x4005f0 <strcpy@plt>
   0x00400580 <+16>:  mov    rdi,0x0
   0x00400584 <+20>:  mov    rsi,0x0
   0x00400588 <+24>:  mov    rdx,0x0
   0x0040058c <+28>:  call   0x4005f0 <strcpy@plt>
   0x00400590 <+32>:  ret    

(gdb) info locals
buffer = "This is a string that exceeds the buffer size by a significant amount."
(gdb) quit
