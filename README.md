Bundy’s Backdoor
Bundy’s Backdoor is a powerful Linux-based web penetration testing tool designed for security professionals and bug bounty hunters. This tool integrates multiple essential pentesting features into one sleek package, aimed at discovering hidden vulnerabilities.

Key Features
Subdomain Finder
Purpose: Unearth hidden subdomains of a target domain.
How It Works: Utilizes a customizable wordlist to probe potential subdomains, identifying active ones that could expand your attack surface.
Directory Brute-forcing
Purpose: Discover hidden directories and files on a target server.
How It Works: Employs a wordlist to brute-force common and obscure directories, revealing potentially vulnerable or sensitive paths.
Fuzzing and Brute-forcing
Purpose: Test web applications for vulnerabilities using fuzzing techniques.
How It Works: Replaces placeholders in target URLs with payloads from a wordlist, identifying potential security flaws like injection points or access issues.
JWT Content Inspection
Purpose: Inspect the content of a JWT token to uncover hidden data or potential vulnerabilities.
How It Works: Decodes the JWT token and displays its content without verifying the signature.
DoS Attack
Purpose: Perform a Denial-of-Service attack to test the resilience of a target server.
How It Works: Sends multiple requests to the target URL using multithreading to overwhelm the server.
Usage
Subdomain Enumeration
bash
Copy code
python3 web_pentest_tool.py -d example.com -s subdomains.txt
Directory Brute-forcing
bash
Copy code
python3 web_pentest_tool.py -u http://example.com -df directories.txt
Fuzzing
bash
Copy code
python3 web_pentest_tool.py -u "http://example.com/login?username=FUZZ&password=pass" -f fuzz.txt
JWT Content Inspection
bash
Copy code
python3 web_pentest_tool.py -jwt "your_jwt_token_here"
DoS Attack
bash
Copy code
python3 web_pentest_tool.py -u http://example.com -dos 10
Installation
Clone the Repository

bash
Copy code
git clone https://github.com/bhavya681/Bundys_Backdoor.git
Navigate to the Directory

bash
Copy code
cd Bundys_Backdoor
Install Dependencies

bash
Copy code
pip install -r requirements.txt
Run the Tool

bash
Copy code
python3 web_pentest_tool.py
Disclaimer
This tool is intended for ethical use in penetration testing and security assessments. Unauthorized use on systems you do not own or have explicit permission to test is illegal and unethical.

Contributing
Contributions are welcome! Please submit a pull request or open an issue if you have suggestions or improvements. For detailed contribution guidelines, refer to the CONTRIBUTING.md file.

License
This project is licensed under the MIT License. See the LICENSE file for more details.

Git Commands
If you haven't set up the repository yet, follow these commands:

Create the README file and initialize the repository:

bash
Copy code
echo "# Bundy’s Backdoor" > README.md
git init
Add and commit the README file:

bash
Copy code
git add README.md
git commit -m "Initial commit with updated README and functionality"
Create the main branch and set the remote repository:

bash
Copy code
git branch -M main
git remote add origin https://github.com/bhavya681/Bundys_Backdoor.git
Push the changes to GitHub:

bash
Copy code
git push -u origin main
