# Password-Generator
<h1>🔐 Simple Password Generator</h1>
This is a basic Bash script that generates random secure passwords using openssl. The user provides the desired password length, and the script generates 5 passwords of that length.

🛠️ How it Works
The script prompts the user to enter the desired password length.

It uses the openssl rand -base64 48 command to generate random data.

Then, it cuts the output to the number of characters entered by the user using cut -c1-$PASS_LENGTH.

The loop runs 5 times to display 5 unique passwords.

📄 Script Usage
bash
Copy
Edit
chmod +x PassGen.sh
./PassGen.sh
Sample Output:

pgsql
Copy
Edit
This is a simple password generator
Please enter the length of the password:-
12
bY5qW3fLv0ZG
dK8nH2vBptQw
XvMz39PnZrQJ
9WsGLch0uBV1
EYz3LuO6hHqT
📌 Requirements
Bash shell

openssl installed (comes by default in most Linux distros)

🚀 Tips
Want more passwords? Change seq 1 5 to something else like seq 1 10.

Passwords longer than 48 characters might not work as expected because openssl rand -base64 48 generates ~48 characters only.
