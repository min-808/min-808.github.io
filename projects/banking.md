---
layout: project
type: project
image: img/banking/banking-square.png
title: "Banking Application"
date: 2024
published: true
labels:
  - C
  - C++
  - Vi
summary: "A simple terminal-based bank application that I developed for ICS 212."
---

<img class="img-fluid" src="../img/banking/banking-header2.png">

This banking application was our final project for ICS 212. The first iterations of the application were coded in C, but we migrated the project to C++ for the final. The banking app is very straightforward. Upon launch, it welcomes the user, and asks them to choose an option. Some of the options include adding a record to the bank database, deleting a record from the database, printing all the records, and finding a specific record given an account number. After quitting the application, the records are saved for the next time the app is launched.

This project was an individual project and I was responsible for all of the code. However, some of the function headers and what the methods were supposed to do were given by the instructor. Each option was created one-by-one, and I had to test and trace every if-statement. I ran into many problems regarding memory allocation issues, file reading errors, and broken linked lists. Since the project was coded in C, a pretty low-level language, the functions provided in the standard library are quite archaic. I had to go through the C and C++ documentation multiple times to debug.

This experience taught me a lot about the C languages. It's a really big contrast from most of the high-level languages out there, like Javascript and Python. I had to learn about memory allocation and garbage collection since those processes aren't automatic like they are now. Additionally, since our teacher required the use of Vi, I learned how to navigate the code editor and memorized a few important shortcuts when developing the application. Also, the files were hosted on Unix, rather than a modern cloud storage system like Google Drive. This meant that I had to figure out how to navigate Unix and memorize the commands to enter directories, edit files, and delete files. Overall, although difficult to learn at first, I was able to pick up the language and terminal and it made for a smooth developing experience.

Here's a code snippet from the **printAllRecords()** method in the llist class:

```cpp
void llist::printAllRecords()
{
  struct record* current = this -> start;

  #ifdef DEBUG
  cout << "\n**DEBUG**: Calling the printAllRecords method\n";
  #endif

  if (this -> start == NULL)
  {
    cout << "\nNo records found\n\n";
  }
  else
  {
    cout << "\nRecords:\n\n";
  }

  while (current != NULL)
  {
    cout << "Account Number: " << current -> accountno << endl;
    cout << "Name: " << current -> name << endl;
    cout << "Address: " << current -> address << endl << endl;
    current = current -> next;
  }
}
```

This code first assigns the variable current to the address of the starting record. From there, if the address is NULL, then there must be no records. However, if it is not NULL, then the records are shown using a while loop. This code uses the typical linked list iteration while loop, where while the current address is not NULL, then print out the number, name, and address of the current record. Then, move onto the next record.

Source: <a href="https://github.com/min-808/project2">Project 2 | Github</a>