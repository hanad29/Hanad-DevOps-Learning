![My Custom Badge](https://img.shields.io/badge/OverTheWire-Bandit-Green)

## Table of Contents 📚

- [My Journey with OverTheWire Bandit](#my-journey-with-overthewire-bandit)
  - [Lessons Learnt So Far](#lessons-learnt-so-far)
  - [Challenges Faced](#challenges-faced)
  - [Why You Should Give It a Try](#why-you-should-give-it-a-try)
  - [Bandit Levels Documented](#bandit-levels-documented)
    - [Bandit Level 0](#bandit-level-0)
    - [Bandit Level 0 → Level 1](#bandit-level-0--level-1)
    - [Bandit Level 1 → Level 2](#bandit-level-1--level-2)
    - [Bandit Level 2 → Level 3](#bandit-level-2--level-3)
    - [Bandit Level 3 → Level 4](#bandit-level-3--level-4)
    - [Bandit Level 4 → Level 5](#bandit-level-4--level-5)
    - [Bandit Level 5 → Level 6](#bandit-level-5--level-6)
    - [Bandit Level 6 → Level 7](#bandit-level-6--level-7)
    - [Bandit Level 7 → Level 8](#bandit-level-7--level-8)
    - [Bandit Level 8 → Level 9](#bandit-level-8--level-9)
    - [Bandit Level 9 → Level 10](#bandit-level-9--level-10)
  - [Command Summary Sheet](#command-summary-sheet)


---
<h1 align="center" style="font-family: 'Press Start 2P', cursive; color: #23FF16;">
  <br>
  <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/bandit.png?raw=true" alt="Bandit logo" width="200">
  <br>
      The OverTheWire Bandit Game
  <img src="https://upload.wikimedia.org/wikipedia/commons/3/35/Tux.svg" alt="Linux Tux Icon" width="50">
  <br>
</h1>

## My Journey with OverTheWire Bandit

In my quest to deepen my Linux skills, I came across the **OverTheWire Bandit** game, and it has been an incredible learning tool. Bandit offers an engaging and interactive way to strengthen practical Linux command-line skills through real-world challenges.

For those unfamiliar, Bandit is a wargame designed to enhance your ability to work with the Linux terminal. Each level presents unique tasks, requiring you to navigate directories, manipulate files, and leverage various commands to uncover hidden passwords and progress to the next stage.

---

## 🎓 Lessons Learnt So Far

- **Building Command Proficiency:**  
  Bandit has been an excellent way to sharpen my skills with the Linux command line. Starting with basic commands like `ls`, `cat`, and `grep`, I’ve gradually tackled more advanced tools like `find`, `xargs`, and `ssh`, gaining hands-on practice with every step.

- **Refining Problem-Solving Skills:**  
  Each level in Bandit presents a unique puzzle that challenges you to think critically, experiment, and approach problems methodically. It has significantly improved my ability to troubleshoot and think strategically in Linux environments.

- **Improving Scripting Abilities:**  
  Some tasks encouraged combining multiple commands or writing simple scripts, providing unexpected but valuable scripting practice. It’s been a great way to develop this crucial skill in a practical setting.

- **Understanding Security Principles:**  
  Bandit incorporates key security concepts, such as file permissions and SSH authentication. These lessons are critical for anyone working with servers or cloud environments, and they’ve been seamlessly woven into the challenges.

---

## 🤔 Challenges Faced

One particularly tricky level for me was Level 6 → Level 7. The challenge involved locating a file with specific properties across the entire server using the find command:

```bash
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
```

---

## 💡 Why You Should Give It a Try

If you’re looking to enhance your Linux command-line skills, OverTheWire Bandit is an invaluable resource. Each challenge pushes you to think critically and expand your knowledge, and the sense of accomplishment after completing a tough level is unbeatable. It’s a rewarding experience for anyone passionate about learning Linux and tackling real-world scenarios.

---

## Bandit Levels Documented

### 🔑 Bandit Level 0

### 🎯 Level Goal
The objective for **Bandit Level 0** was to log into the game server using SSH. The task involved connecting to the provided host with the correct port, username, and password. Upon logging in, I needed to move to the Level 1 page to proceed to the next challenge.

---

### 📝 What I Needed
- **Terminal:** Git Bash  
- **Server Access:**  
  - Host: `bandit.labs.overthewire.org`  
  - Port: `2220`  
  - Username: `bandit0`  
  - Password: `bandit0`

---

### 💻 Steps I Followed:
1. Opened **Git Bash** terminal.
2. Used the following SSH command to connect to the Bandit server:
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

---

<div style="text-align: center; margin: 20px 0;">
  <h2 style="font-family: 'Arial', sans-serif; color: #FF5722; font-size: 24px; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px;">🎥Live Demonstration</h2>
  <div style="width: 400px; margin: 0 auto; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
    <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/Level0.gif?raw=true" alt="Level 0 GIF" width="100%" />
  </div>
</div>

### 🔑 Bandit Level 0 → Level 1

### 🎯 Level Goal
The password for **Bandit Level 1** was stored in a file called `readme` located in the home directory of the Bandit Level 0 server. My objective was to find and retrieve this password and use it to log into Bandit Level 1 via SSH.

---

### 💻 Steps I Followed:
1. First, I logged into the Bandit Level 0 server using the following SSH command:
   ```bash
   ssh bandit0@bandit.labs.overthewire.org -p 2220
2. Once logged in, I listed the files in the home directory using:
```bash
ls
```
3. I then displayed the contents of the readme file to retrieve the password for the next level:
```bash
cat readme
```
4. Finally, I used the retrieved password to log into Bandit Level 1 using this command:
```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```
<div style="text-align: center; margin: 20px 0;">
  <h2 style="font-family: 'Arial', sans-serif; color: #FF5722; font-size: 24px; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px;">🎥Live Demonstration</h2>
  <div style="width: 400px; margin: 0 auto; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
    <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/Level%200-1.gif?raw=true" alt="Level 0-1 GIF" width="100%" />
  </div>
</div>

---

### 🔑 Bandit Level 1 → Level 2

### 🎯 Level Goal
The password for **Bandit Level 2** was stored in a file named `-` located in the home directory of the Bandit Level 1 server. My task was to retrieve the password from this uniquely named file and use it to log into Bandit Level 2 via SSH.

---

### 💻 Steps I Followed:
1. First, I logged into the Bandit Level 1 server using the password retrieved from the previous level:
 ```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```
2. Once logged in, I listed the files in the home directory using:

```bash
ls
```
This revealed a file named -, which required special handling since - is often interpreted as an option in Linux commands.

3. To read the contents of the file without it being interpreted as an option, I used ./ to specify it as a file in the current directory:

```bash
cat./-
```
This command displayed the password for Bandit Level 2.

4. Using the retrieved password, I logged into Bandit Level 2 with the following command:

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```
<div style="text-align: center; margin: 20px 0;">
  <h2 style="font-family: 'Arial', sans-serif; color: #FF5722; font-size: 24px; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px;">🎥Live Demonstration</h2>
  <div style="width: 400px; margin: 0 auto; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
    <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/Level%201-2.gif?raw=true" alt="Level 0-1 GIF" width="100%" />
  </div>
</div>

---

### 🔑 Bandit Level 2 → Level 3

### 🎯 Level Goal
The password for **Bandit Level 3** was stored in a file named `spaces in this filename` located in the home directory of the Bandit Level 2 server. My task was to retrieve the password from this file and use it to log into Bandit Level 3 via SSH.

---

### 💻 Steps I Followed:
1. First, I logged into the Bandit Level 2 server using the password retrieved from the previous level:
  ```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```
2. Once logged in, I listed the files in the home directory using:

 ```bash
ls
```
This displayed a file named spaces in this filename. The file name contained spaces, requiring special handling.
3. To read the contents of the file, I enclosed the file name in double quotes ("):

 ```bash
cat "spaces in this filename"
```
This command successfully displayed the password for Bandit Level 3.

4. Using the retrieved password, I logged into Bandit Level 3 with the following command:

 ```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```
<div style="text-align: center; margin: 20px 0;">
  <h2 style="font-family: 'Arial', sans-serif; color: #FF5722; font-size: 24px; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px;">🎥Live Demonstration</h2>
  <div style="width: 400px; margin: 0 auto; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
    <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/Level%202-3.gif?raw=true" alt="Level 0-1 GIF" width="100%" />
  </div>
</div>

---

### 🔑 Bandit Level 3 → Level 4

### 🎯 Level Goal
The password for **Bandit Level 4** was stored in a hidden file located in the `inhere` directory. My task was to locate this hidden file, retrieve its contents, and use the password to log into Bandit Level 4 via SSH.

---

### 💻 Steps I Followed:
1. First, I logged into the Bandit Level 3 server using the password retrieved from the previous level:
   
  ```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```
2. I listed the files in the home directory to locate the inhere directory:

```bash
ls
```
3. Navigated to the inhere directory using the following command:

```bash
cd inhere
```
4. Since the level specified that the file was hidden, I used the ls command with the -a option to display hidden files:

```bash
ls -a
```
This revealed a hidden file named .hidden.

5. To retrieve the password, I used the cat command to display the contents of the hidden file:

```bash
cat .hidden
```
This command displayed the password for Bandit Level 4.

6. Using the retrieved password, I logged into Bandit Level 4 with the following command:

```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```
<div style="text-align: center; margin: 20px 0;">
  <h2 style="font-family: 'Arial', sans-serif; color: #FF5722; font-size: 24px; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px;">🎥Live Demonstration</h2>
  <div style="width: 400px; margin: 0 auto; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
    <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/Level%203-4.gif?raw=true" alt="Level 0-1 GIF" width="100%" />
  </div>
</div>

---

### 🔑 Bandit Level 4 → Level 5

### 🎯 Level Goal
The password for **Bandit Level 5** was stored in the only human-readable file located in the `inhere` directory. My task was to identify this file, retrieve its contents, and use the password to log into Bandit Level 5 via SSH.

---

### 💻 Steps I Followed:
1. First, I logged into the Bandit Level 4 server using the password retrieved from the previous level:

  ```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```
2. I listed the files in the home directory to locate the inhere directory:

```bash
ls
```

3. Navigated to the inhere directory:

```bash
cd inhere
```

4. To identify the human-readable file, I used the file command to inspect each file in the directory:

```bash
file./*
```
This command displayed the properties of each file. I located the human-readable file based on its type being identified as ASCII text.

5. I used the cat command to display the contents of the human-readable file and retrieve the password:

```bash
cat ./-file07
```
This command revealed the password for Bandit Level 5.

6. Using the retrieved password, I logged into Bandit Level 5:

```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
```
<div style="text-align: center; margin: 20px 0;">
  <h2 style="font-family: 'Arial', sans-serif; color: #FF5722; font-size: 24px; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px;">🎥Live Demonstration</h2>
  <div style="width: 400px; margin: 0 auto; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
    <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/Level%204-5.gif?raw=true" alt="Level 0-1 GIF" width="100%" />
  </div>
</div>

---

### 🔑 Bandit Level 5 → Level 6

### 🎯 Level Goal
The password for **Bandit Level 6** was stored in a file located somewhere within the `inhere` directory. The file met the following conditions:
- Human-readable
- Exactly 1033 bytes in size
- Not executable

My task was to locate this file, retrieve its contents, and use the password to log into Bandit Level 6 via SSH.

---

### 💻 Steps I Followed:
1. First, I logged into the Bandit Level 5 server using the password retrieved from the previous level:

  ```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
```

2. I listed the files in the home directory to locate the inhere directory:

```bash
ls
```
3. Navigated to the inhere directory:

```bash
cd inhere
```
4. To locate the file matching the criteria, I used the find command:

```bash
find . -type f -size 1033c ! -executable
```
-type f: Search for regular files. <br>
-size 1033c: Filter files exactly 1033 bytes in size. <br>
! -executable: Exclude executable files. <br>

The find command identified the file. <br>

5. I then used the cat command to read its contents and retrieve the password:

```bash
cat ./maybehere07/.file2
```

6. Using the retrieved password, I logged into Bandit Level 6:

```bash
ssh bandit6@bandit.labs.overthewire.org -p 2220
```
<div style="text-align: center; margin: 20px 0;">
  <h2 style="font-family: 'Arial', sans-serif; color: #FF5722; font-size: 24px; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px;">🎥Live Demonstration</h2>
  <div style="width: 400px; margin: 0 auto; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
    <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/Level%205-6.gif?raw=true" alt="Level 0-1 GIF" width="100%" />
  </div>
</div>

---

### 🔑 Bandit Level 6 → Level 7

### 🎯 Level Goal
The password for **Bandit Level 7** was stored in a file somewhere on the server. The file met the following criteria:
- Owned by user `bandit7`
- Owned by group `bandit6`
- Exactly 33 bytes in size

My task was to locate this file, retrieve the password, and use it to log into Bandit Level 7 via SSH.

---

### 💻 Steps I Followed:
1. First, I logged into the Bandit Level 6 server using the password retrieved from the previous level:

  ```bash
ssh bandit6@bandit.labs.overthewire.org -p 2220
```
2. To search for the file matching the specified criteria, I used the find command:

```bash
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
```
/: Search the entire file system. <br>
-user bandit7: Filter files owned by user bandit7. <br>
-group bandit6: Filter files belonging to group bandit6. <br>
-size 33c: Filter files exactly 33 bytes in size. <br>
2>/dev/null: Suppress permission error messages for directories I couldn't access. <br>

The command output revealed the file's location. 

3. I used the cat command to read its contents and retrieve the password:

```bash
cat /var/lib/dpkg/info/bandit7.password
```

4. Using the retrieved password, I logged into Bandit Level 7:

```bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
```
<div style="text-align: center; margin: 20px 0;">
  <h2 style="font-family: 'Arial', sans-serif; color: #FF5722; font-size: 24px; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px;">🎥Live Demonstration</h2>
  <div style="width: 400px; margin: 0 auto; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
    <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/Level%206-7.gif?raw=true" alt="Level 0-1 GIF" width="100%" />
  </div>
</div>

---

### 🔑 Bandit Level 7 → Level 8

### 🎯 Level Goal
The password for **Bandit Level 8** was stored in a file called `data.txt` next to the word "millionth." My task was to locate the word "millionth" within the file and retrieve the corresponding password.

---

### 💻 Steps I Followed:
1. First, I logged into the Bandit Level 7 server using the password retrieved from the previous level:

  ```bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
```
2. I listed the directory contents to confirm the presence of data.txt:

```bash
ls
```

3. To find the word "millionth" and its associated password within the file, I used the grep command:

```bash
grep "millionth" data.txt
```
The grep command returned the line containing the word "millionth" and the password for the next level.

4. Using the retrieved password, I logged into Bandit Level 8:

```bash
ssh bandit8@bandit.labs.overthewire.org -p 2220
```

<div style="text-align: center; margin: 20px 0;">
  <h2 style="font-family: 'Arial', sans-serif; color: #FF5722; font-size: 24px; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px;">🎥Live Demonstration</h2>
  <div style="width: 400px; margin: 0 auto; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
    <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/Level%207-8.gif?raw=true" alt="Level 0-1 GIF" width="100%" />
  </div>
</div>

---

### 🔑 Bandit Level 8 → Level 9

### 🎯 Level Goal
The password for **Bandit Level 9** was stored in the file `data.txt` and was the only line of text that occurred exactly once. My task was to identify this unique line and retrieve the password to access the next level.

---

### 💻 Steps I Followed:
1. First, I logged into the Bandit Level 8 server using the password retrieved from the previous level:

```bash
ssh bandit8@bandit.labs.overthewire.org -p 2220
```

2. I listed the directory contents to confirm the presence of data.txt:

```bash
ls
```

3. To sort the lines in data.txt so that duplicate lines would be adjacent, I used the sort command:

```bash
sort data.txt
```

4. I then piped the sorted output to the uniq command with the -u flag to isolate the line that appeared only once:

```bash
sort data.txt | uniq -u
```
The output of the uniq -u command revealed the unique line, which contained the password for the next level.

5. Using the retrieved password, I logged into Bandit Level 9:

```bash
ssh bandit9@bandit.labs.overthewire.org -p 2220
```
<div style="text-align: center; margin: 20px 0;">
  <h2 style="font-family: 'Arial', sans-serif; color: #FF5722; font-size: 24px; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px;">🎥Live Demonstration</h2>
  <div style="width: 400px; margin: 0 auto; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
    <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/Level%208-9.gif?raw=true" alt="Level 0-1 GIF" width="100%" />
  </div>
</div>

---

### 🔑 Bandit Level 9 → Level 10

### 🎯 Level Goal
The password for **Bandit Level 10** was stored in the file `data.txt` among a few human-readable strings, preceded by several `=` characters. My task was to extract the human-readable strings and locate the password.

---

### 💻 Steps I Followed:
1. First, I logged into the Bandit Level 9 server using the password retrieved from the previous level:

```bash
ssh bandit9@bandit.labs.overthewire.org -p 2220
```

2. I listed the directory contents to confirm the presence of data.txt:

```bash
ls
```

3. To extract all human-readable strings from data.txt, I used the strings command:

```bash
strings data.txt
```

4. Since the password was preceded by several = characters, I piped the output from strings to the grep command to filter lines containing =:

```bash
strings data.txt | grep '='
```

5. I identified the password from the filtered output by focusing on the line with multiple = characters.

6. Using the retrieved password, I logged into Bandit Level 10:

```bash
ssh bandit10@bandit.labs.overthewire.org -p 2220
```
<div style="text-align: center; margin: 20px 0;">
  <h2 style="font-family: 'Arial', sans-serif; color: #FF5722; font-size: 24px; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px;">🎥Live Demonstration</h2>
  <div style="width: 400px; margin: 0 auto; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);">
    <img src="https://github.com/hanadisa/Hanad-DevOps-Learning/blob/main/My-DevOps-Journey/Linux/Notes/Images/Level%209-10.gif?raw=true" width="100%" />
  </div>
</div>

---

## To be continued...⏳

--- 

## Command Summary Sheet

Here’s a handy guide to the commands I relied on during the Bandit walkthrough. These tools were essential for tackling the challenges and are equally valuable in other Linux environments.

### 1. Navigation & File Operations:
- `ls`: List directory contents.
- `ls -a`: List all files, including hidden ones.
- `cd <directory>`: Change the current directory.
- `cat <filename>`: Display the contents of a file.
- `cat ./<filename>`: Use `./` to reference a file that starts with special characters (e.g., `-`).
- `file <filename>`: Determine the file type.

### 2. Searching & Sorting:
- `find ./<directory> -type f -size <size>`: Search for files of a specific type and size.
- `find / -user <username> -group <groupname> -size <size>`: Search for files with a specific owner, group, and size.
- `grep <pattern> <filename>`: Search for lines matching a pattern within a file.
- `sort <filename>`: Sort the contents of a file.
- `uniq -u`: Filter and display only the unique lines from sorted output.

### 3. Secure Shell (SSH):
- `ssh <username>@<hostname> -p <port>`: Connect to a remote server via SSH using a specific username and port.

### 4. Data Manipulation:
- `strings <filename>`: Extract human-readable strings from binary data.
- `base64 -d <filename>`: Decode base64-encoded data.
- `tr 'A-Za-z' 'N-ZA-Mn-za-m'`: Use the `tr` command to translate characters, such as decoding ROT13-encoded text.

### 5. Redirection & Suppression:
- `2>/dev/null`: Redirect error messages to suppress them from being displayed.
