# RSA Factoring Challenge

We have sniffed an unsecured network and found numbers that are used to encrypt very important documents. It seems that those numbers are not always generated using large enough prime numbers. Your mission should you choose to accept it, is to factorize these numbers as fast as possible before the target fixes this bug on their server - so that we can decode the encrypted documents.

## Resources

[*RSA](https://en.wikipedia.org/wiki/RSA_(cryptosystem%29)

[*How does HTTPS provide security?](https://stackoverflow.com/questions/3968095/how-does-https-provide-security)

[*Prime Factorization](https://privacycanada.net/mathematics/prime-factorization/)

[*Why RSA?](https://jaredatandi.hashnode.dev/rsa-factoring)

## Requirements

## General

* You can choose the language of your choice.

* OS needs to be Standard Ubuntu 20.04 LTS/

## Tasks

### 0.Factorize all things

Factorize as many numbers as possible into a product of two smaller numbers.

  * Usage: factors <file>

    	   * where <file> is a file containing natural numbers to factor.

	   * One number per line

	   * You can assume that all lines will be valid natural numbers g		reater than 1

	   * You can assume that there will be no empy line, and no space 		before and after the valid number

	   * The file will always end with a new line

  * Output format: n=p*q

    	   * one factorization per line

	   *p and q don’t have to be prime numbers

	   * See example

  * You can work on the numbers of the file in the order of your choice

  * Your program should run without any dependency: You will not be able t    o install anything on the machine we will run your program on

  * Time limit: Your program will be killed after 5 seconds if it hasn’t f    inish

  * Push all your scripts, source code, etc… to your repository
    	 * we will only run your executable factors
julien@ubuntu:~/factors$ cat tests/test00
4
12
34
128
1024
4958
1718944270642558716715
9
99
999
9999
9797973
49
239809320265259
julien@ubuntu:~/factors$ time ./factors tests/test00
4=2*2
12=6*2
34=17*2
128=64*2
1024=512*2
4958=2479*2
1718944270642558716715=343788854128511743343*5
9=3*3
99=33*3
999=333*3
9999=3333*3
9797973=3265991*3
49=7*7
239809320265259=15485783*15485773

real    0m0.009s
user    0m0.008s
sys 0m0.001s
julien@ubuntu:~/factors$