## Git

Command: git --version

Output:2.55.0.windows.5

## VS Code

Command: code --version

Output: 1.135.0

## Java

Command: java -version

Output: java version "21.0.12" 2026-07-21 LTS
Java(TM) SE Runtime Environment (build 21.0.12+7-LTS-205)
Java HotSpot(TM) 64-Bit Server VM (build 21.0.12+7-LTS-205, mixed mode, sharing)

## Python

Command: python3 --version

Output: Python 3.14.7

## pip

Command: pip3 --version

Output: pip 25.0.1

## Docker

Command: docker --version

Output: Docker version 29.7.2

Command: docker compose version

output:Docker Compose version v5.5.0

## Postman

Postman installed successfully and i am able to sign in.

## Reflection

The hardest part of the environment setup for me was installing the Java Development Kit (JDK 21) and getting the system to recognize it. Initially, when I ran the verification check, my terminal threw an error stating that 'java' was not recognized as an internal or external command. 

To resolve this blocker, I researched how Windows handles executable paths. I located the target directory at C:\Program Files\Java\jdk-21\bin, manually opened my System Environment Variables panel, and appended this precise binary folder configuration directly to my local system PATH variable. After restarting my terminal session, the system successfully initialized the compiler, displaying java version "21.0.12" LTS.

This process taught me a critical lesson about how an Operating System routes CLI commands to backend compiler binaries through path environment variables
