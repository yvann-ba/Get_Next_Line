# Get_Next_Line

## 📜 Description
"Get_Next_Line" is a project I completed at 42 School. The goal is to create a function that reads a line from a file descriptor, allowing efficient file input handling. This function helps manage dynamic memory and works with various file descriptors simultaneously.

#### ⭐ My 42 score for this project:
![image](https://github.com/yvann-ba/Get_Next_Line/assets/97234242/8c9961c4-94a7-4582-8cf6-8441c28fb425)

#### 📄 Official 42 School Subject:
https://github.com/rphlr/42-Subjects/blob/main/common-core/get_next_line/en.subject.pdf

## 🌟 Features
- Read lines from a file descriptor
- Handle multiple file descriptors at once
- Efficient dynamic memory management

## ⚙️ Installation

To clone and compile this project, follow these steps:

```bash
git clone https://github.com/your-username/Get_Next_Line.git
cd Get_Next_Line
make
```
## 🚀 Usage
Include the function in your projects:
```c
#include "get_next_line.h"
```
Use the get_next_line function to read lines from a file:
```c
int fd = open("file.txt", O_RDONLY);
char *line;
while (get_next_line(fd, &line) > 0) {
    printf("%s\n", line);
    free(line);
}
close(fd);
```
