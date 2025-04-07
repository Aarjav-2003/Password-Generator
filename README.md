# Password-Generator
<h2>🔐 Simple Password Generator</h2>
This is a basic Bash script that generates random secure passwords using openssl. The user provides the desired password length, and the script generates 5 passwords of that length.
<hr>
<h2>🛠️ How it Works</h2>
<ol>
  <li>The script prompts the user to enter the desired password length.</li>
  <li>It uses the openssl rand -base64 48 command to generate random data.</li>
  <li>Then, it cuts the output to the number of characters entered by the user using cut -c1-$PASS_LENGTH.</li>
  <li>The loop runs 5 times to display 5 unique passwords.</li>
</ol>
<hr>

<h2>📄 Script Usage</h2>
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
<hr>
<h2>📌 Requirements</h2>
Bash shell
<ul>
  <li>Bash shell</li>
  <li>openssl installed (comes by default in most Linux distros)</li>
</ul>
<hr>
<h2>🚀 Tips</h2>
<ul>
  <li>Want more passwords? Change seq 1 5 to something else like seq 1 10.</li>
  <li>Passwords longer than 48 characters might not work as expected because openssl rand -base64 48 generates ~48 characters only.</li>
</ul>
