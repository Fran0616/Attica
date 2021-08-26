# Attica
Attica, a clothing store, has asked you to help them configure their environment.

Task 
=

1. Print the working directory
2. Create and open a file in nano called hello.txt
3. Save the string, "Hello, I am nano' in hello.txt; save the file, exit nano, and clear the terminal. 
4. use nano to open the bash profile
5. In the bash profile, add a greating with the word "Hello" using the `echo` command. Save the file, exit nano, and clear the terminal. 
6. Use the `source` command to make the greating available in the current session. You should see the greating you created. 
7. Open the bash profile, and create two aliases. The first alies should be `p` for `pwd` command and `ll` for the `ls -la` command. Save the file, exit nano, and clear the terminal. 
8. Use the source command to make he alieses avaiable in the current session. 
9. Test out the alieses you created for the `pwd` and `ls -la` command. 
10. Open the bash profile and create and export the `USER` envronment variable, setting it equal to your name. Save the file, exit nano, and clear the terminal. 
11. Echo the `USER` variable. 
12. Open the bash profile and create and export the PS1 environment variable, setting it equal to  `>>`. Save the file, exit nano, and clear the terminal. 
13. Use the `source` command to make the promt available in the current session. 
14. Test out the promt by typing the two aliases you created ealier. 
15. Echo the `HOME` variable. 
16. Echo the `PATH` variable. 
17. Return a list of environment variable. 


Test Data
=
```
$ pwd
/home/ccuser/workspace/clothing
$ nano hello.txt
$ nano ~/.bash_profile
$ source ~/.bash_profile
Hello, I am nano
$ nano ~/.bash_profile
$ source ~/.bash_profile
Hello, I am nano
$ p
/home/ccuser/workspace/clothing
$ ll
total 4
drwxr-xr-x 2 ccuser ccuser 152 Aug 26 15:38 .
drwxrwxr-x 1 ccuser ccuser  22 Aug 26 15:37 ..
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 dresses.txt
-rw-r--r-- 1 ccuser ccuser  17 Aug 26 15:38 hello.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 jackets.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 pants.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 scarves.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 shirts.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 socks.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 sweaters.txt
$ echo USER
USER
$ source ~/.bash_profile
Hello, I am nano
>>p
/home/ccuser/workspace/clothing
>>ll
total 4
drwxr-xr-x 2 ccuser ccuser 152 Aug 26 15:38 .
drwxrwxr-x 1 ccuser ccuser  22 Aug 26 15:37 ..
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 dresses.txt
-rw-r--r-- 1 ccuser ccuser  17 Aug 26 15:38 hello.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 jackets.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 pants.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 scarves.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 shirts.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 socks.txt
-rw-r--r-- 1 ccuser ccuser   0 Aug 26 15:37 sweaters.txt
>>echo $HOME
/home/ccuser
>>echo $PATH
/home/ccuser/.bin:/home/ccuser/node_modules/.bin:/home/ccuser/.gem/ruby/2.3.0/bin:/home/ccuser/.composer/vendor/bin:/home/ccuser/.bin:/home/ccuser/node_modules/.bin:/home/ccuser/.gem/ruby/2.3.0/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
>>env
HOSTNAME=41fc764b5ce0
GEM_HOME=/home/ccuser/.gem/ruby/2.3.0
TERM=xterm
USER=Francisco
EXPIRES_AT=1629995824
NLTK_DATA=/home/ccuser/.nltk_data
PATH=/home/ccuser/.bin:/home/ccuser/node_modules/.bin:/home/ccuser/.gem/ruby/2.3.0/bin:/home/ccuser/.composer/vendor/bin:/home/ccuser/.bin:/home/ccuser/node_modules/.bin:/home/ccuser/.gem/ruby/2.3.0/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
CODEX_RUNNER_PATH=/var/codecademy/codex/runners
PWD=/home/ccuser/workspace/clothing
MPLBACKEND=agg
SESSION_ID=199f6821-588c-4a85-a4df-cd7e62f854bb
LANG=en_US.UTF-8
TZ=Etc/UTC
PS1=>>
HOME=/home/ccuser
SHLVL=2
PYTHONPATH=/var/codecademy/runner_contexts/python:
_=/usr/bin/env
```

Summarry
=
In conclusion I learned to use the bash profile to configure the environment. The environment refers to the preferences and setting of the current user. The nano editor is a command line text editor used to configure the environment. The bash profile is where environment settings are stored, and you can edit this file with nano `nano ~/.bash_profile`. Environment variables are variables that can be used across commands and programs and hold information about the environment. the `export VARIABLE="Value"` sets and expors an environment varaable. `USER` is the name of the current user. `ps1` is the command prompt. `HOME` is the home directory. It is usually not customized. `PATH` returns a collan `:` separated list of file paths. It is customized in advenced cases. `env` returns a list of environment variables. You can redirect the output, using `grep` to select the varaible you want to see. 
