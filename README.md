# INTERNSHIP TASK - 01

# FILE-HANDLING-PROGRAM

 COMPANY: CODTECH IT SOLUTIONS

 NAME: YUKTA ANAND

 INTERN ID: CT04DN1416

 DOMAIN: C PROGRAMMING

 DURATION: 4 WEEKS

 MENTOR: NEELA SANTOSH



 
#  🔍 Overview of the Program:
 

# 📁 File Used:
The program works on a file named  sample.txt.

# ✅ FUNCTION EXPLANATIONS

1. void writeFile(const char *filename)

i) Purpose:- Creates a file (or overwrites if it already exists) and writes a line of text into it.

ii) Mode Used:- "w" (write mode)
   If the file exists, it overwrites it.
   If it doesn’t exist, it creates a new one.
   
iii) Operation:-
      
      c
      fprintf(fp, "This is the initial content.\n");
Writes a line to the file.

iv) Error Handling:-
   If file opening fails, it uses perror() to print the system error.

2. void readFile(const char *filename)
   
i) Purpose:- Opens and reads the content of the file, character by character, and prints it to the console.

ii) Mode Used:- "r" (read mode)
   The file must exist, or it will give an error.
   
iii) Operation:-

     c
     while ((ch = fgetc(fp)) != EOF) {
          putchar(ch);
    }
Reads and prints each character until the end of the file.

3. void appendFile(const char *filename)
   
i) Purpose:- Opens an existing file and appends new content at the end without modifying existing content.

ii) Mode Used:- "a" (append mode)
   Opens the file and appends data at the end.
   If the file doesn’t exist, it will be created.
   
iii) Operation:-

       c
       fprintf(fp, "Appended line added.\n");


🚦 main() Function Flow
    
       c
       const char *filename = "sample.txt";
Uses a constant filename for all operations.


# Step-by-step Execution:

1. Create & Write File
Calls writeFile() → creates sample.txt with one line.

2. Read File (First Time)
Calls readFile() → prints:

       csharp
               This is the initial content.

3. Append File
Calls appendFile() → adds another line at the end.

4. Read File (Second Time)
Calls readFile() again → prints:

        scss
               This is the initial content.
                Appended line added.


# 📌 Summary


          Operation            File Mode	                          Behavior

    a)    writeFile()          	"w"                    	Creates or overwrites the file
    b)     readFile()           	"r"                     	Reads the file from the beginning
    c)    appendFile()	         "a"                   	Appends content at the end of the file


# 🧠 Key Concepts Demonstrated:

 a) File handling in C
 
 b) Modes of fopen: "w", "r", "a"
 
 c) Error checking using if (fp == NULL)
 
 d) Reading character-by-character using fgetc()


 # OUTPUT
 
 ![Image](https://github.com/user-attachments/assets/77b774f9-5c38-4939-aa42-551b8f60fff2)

 [sample.txt](https://github.com/user-attachments/files/20546023/sample.txt)


 
