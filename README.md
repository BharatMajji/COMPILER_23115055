💰 Simple Interest & Compound Interest Parser 💰
===============================================

📌 This project is a basic compiler-like application built using Flex (Lex) and Bison (Yacc) in C++ to parse and evaluate Simple Interest (SI) and Compound Interest (CI) instructions.

✨ Features ✨
-------------

✅ Parses user-friendly input like: 

   SI amount = 1000, 5, 2; 
   
   CI final = 1000, 5, 2;
   
✅ Generates three-address code

✅ Shows optimized custom instructions

✅ Displays final calculated result

✅ Outputs pseudo assembly-style code

✅ Supports both Simple and Compound Interest


📂 Project Structure 📂
----------------------

📄 main.cpp        - Main driver program

📄 lexer.l         - Flex lexical analyzer rules

📄 parser.y        - Bison grammar rules

📄 Makefile        - Build automation

📄 README.md       - Documentation


⚙️ Requirements ⚙️
------------------

🔹 g++ - C++ compiler

🔹 flex - for lexical analysis (v2.6+)

🔹 bison - for syntax parsing (v3.0+)


🪟 Windows with MSYS2 🪟
----------------------

💻 Run in MSYS2 terminal:

pacman -Syu

pacman -S mingw-w64-x86_64-gcc flex bison make


🐧 Linux (Debian/Ubuntu) 🐧
--------------------------

💻 Run in terminal:

sudo apt-get update

sudo apt-get install g++ flex bison make


🔨 Build Instructions 🔨
----------------------

💡 To compile everything:

make

This will:

1️⃣ Use Flex to generate lex.yy.c

2️⃣ Use Bison to generate parser files

3️⃣ Compile all source files

4️⃣ Produce executable: mycompiler


🚀 How to Use 🚀
---------------

👉 Run the compiled binary:

./mycompiler

📝 Then enter expressions like:

SI s = 1000, 5, 2;

CI c = 1000, 5, 2;


🛑 Press Ctrl+D (Linux/Mac) or Ctrl+Z (Windows) to exit.


🧮 Interest Formulas 🧮
----------------------

💵 Simple Interest:

SI = (P × R × T) / 100

Where:

🔹 P = Principal amount

🔹 R = Rate of interest (%)

🔹 T = Time period (years)


💹 Compound Interest:

CI = A - P

A = P × (1 + R/100)^T

Where:

🔹 P = Principal amount

🔹 R = Rate of interest (%)

🔹 T = Time period (years)

🔹 A = Amount after interest


🧹 Cleaning the Build 🧹
----------------------

🗑️ To remove all generated files:
make clean

📜 License 📜
-----------

📛 MIT License

💡 Example Output 💡
------------------


📥 Input:

SI s = 1000, 5, 2;

📤 Output:

[Three Address Code]

t1 = 1000.00 * 5.00

t2 = t1 * 2.00

s = t2 / 100


[Optimized Instructions]

SI s = 1000, 2, 5


[Evaluated Result] 

s = 100.00


[Final Code]

STORE s


📥 Input:

CI c = 1000, 5, 2;

📤 Output:

[Three Address Code]

t1 = 5.00 / 100

t2 = 1 + t1

t3 = pow(t2, 2.00)

t4 = 1000.00 * t3

c = t4 - 1000.00


[Evaluated Result]

c = 102.50


[Final Code]

STORE c


📸 OUTPUT 📸
------------------

![Screenshot 2025-04-06 163721](https://github.com/user-attachments/assets/d0f3d600-816c-4bbc-a728-e3746e691e9c)




✍🏻 Author ✍🏻

-----------
Majji Bharat Chandra

🎓 B.Tech CSE, NIT Raipur


