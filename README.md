# NETWORKWALKS-B083-WK3-PM1-PASSWORD-CRACKING-WITH-JTR-Public
#### Password Cracking & PDF Hash Analysis — John the Ripper

# 📌 Project Overview

This project documents the practical process of extracting password-related hash information from a password-protected PDF and attempting password recovery using John the Ripper (JTR).

The lab was performed in a controlled cybersecurity learning environment as part of the NetworkWalks training. It covers the basic workflow of obtaining a crackable hash from an encrypted PDF, preparing the hash for John the Ripper, performing a password-cracking attack, and checking whether the recovered password can successfully unlock the original document.

The project also provided hands-on practice with John the Ripper and Johnny, helping to understand how password-cracking tools work and how weak passwords can be identified through offline attacks.


# 🎯 The main objectives of this practical were to:

Understand the basic concept of password cracking and password hashes.
Learn how password-protected PDF files can be analyzed for their hash information.
Extract the required hash from the protected PDF.
Use John the Ripper to perform an offline password-cracking attempt.
Understand the purpose of wordlists in dictionary-based attacks.
Explore the Johnny graphical interface for John the Ripper.
Verify whether the recovered password can open the original protected PDF.
Understand why weak and predictable passwords are easier to recover.
Gain practical experience with password-auditing tools in a controlled environment.

# Purpose of the Project

This practical was carried out to develop a basic understanding of password security and offline password recovery.

The project helped me to:
Become familiar with John the Ripper and its working environment.
Understand how an encrypted PDF can provide information that can be converted into a crackable hash.
Learn the basic process of moving from a protected file to a hash and then to password recovery.
Understand how dictionary-based password attacks work.
Practice using both command-line and graphical interfaces for security testing.
Understand the importance of strong and less predictable passwords.
Build practical knowledge related to ethical hacking and cybersecurity assessments.

# 🛠️ Tools & Technologies Used
Tool / Technology	Purpose
🐉 Kali Linux	Cybersecurity testing environment
🔓 John the Ripper	Password-cracking and password-auditing tool
🖥️ Johnny	Graphical interface for John the Ripper
📄 PDF Hash Extraction Tool	Extracting password-related hash information
📚 Wordlist	Providing possible password candidates
💻 Windows	Used during the John the Ripper setup process


# 📖  Introduction to Password Cracking

Password cracking is a technique used to recover or test passwords by trying different possible password values against stored password hashes or encrypted data.

Instead of directly seeing the original password, a security tool normally works with a representation of the password, such as a hash or an encryption-related value.

For a protected PDF, the general process can be understood as:

Obtain the password-protected PDF.
Extract the relevant hash information from the file.
Prepare the extracted information in a format that John the Ripper can understand.
Provide possible password candidates through a wordlist or another cracking method.
Allow John the Ripper to compare the generated values against the target.
Check whether a matching password is discovered.
Use the recovered password to verify access to the original PDF.

This practical demonstrated this process using a controlled and authorized PDF file.

# Technical Execution & Methodology

The practical was completed through the following general workflow:

Identify the password-protected PDF used for the lab.
Extract the required hash information from the PDF.
Prepare and save the extracted hash.
Configure John the Ripper / Johnny.
Select the appropriate wordlist.
Start the password-cracking process.
Check the result returned by the tool.
Verify the recovered password against the original PDF.

# Method 1: Password Recovery using John the Ripper :-

# Step 1: Selecting the Protected PDF
Located the password-protected PDF provided for the practical.
Confirmed that the file required a password before its contents could be accessed.
Kept the original PDF available for later verification.
<img width="1910" height="1034" alt="Screenshot 2026-09-26 201200" src="https://github.com/user-attachments/assets/052da5f0-1f9e-40bd-8722-e5e03d7f3b3b" />

# Step 2: Extracting Hash Information
Used the PDF hash extraction process to analyze the protected document.
Extracted the password-related hash information from the PDF.
Copied the generated hash carefully.
Saved the hash in a text file so it could be used with John the Ripper.
The extracted hash must be copied completely because missing or changing even part of the hash can cause the cracking tool to reject or incorrectly interpret it.
<img width="1919" height="1017" alt="Screenshot 2026-09-26 193047" src="https://github.com/user-attachments/assets/94247f09-99aa-46c9-8525-cdc51864e11e" />

## Step 3: Verifying the Recovered Password

- After the password was recovered, I copied the result.
- The original password-protected PDF was opened.
- The recovered password was entered into the PDF.
- The document opened successfully.
- This confirmed that the recovered password was correct.
 
<img width="1899" height="971" alt="Screenshot 2026-09-26 193157" src="https://github.com/user-attachments/assets/007cd6fa-1ef4-4c1d-bdb5-8fbb76253a7f" />

<img width="1911" height="1025" alt="Screenshot 2026-09-26 193222" src="https://github.com/user-attachments/assets/646a4c24-95ec-4b8d-8d4d-abd42bc9264f" />


# Method 2: Web-Based Password Recovery via NETWORKWALKS Tools

The second approach used the **NETWORKWALKS security tools** to perform the password-recovery process through a web interface.

The purpose of this method was to understand that password recovery can also be performed through web-based security utilities when the appropriate hash format is available.

## Step 1: Creating the PDF Hash using NETWORKWALKS

- I opened the **NETWORKWALKS Hash Calculator**.
- The password-protected PDF was uploaded to the tool.
- The tool processed the file and generated the required PDF hash information.
- The generated hash followed the PDF hash format required for password-cracking.
- I copied the complete hash carefully so that no part of the hash was missed.

### Screenshot
<img width="1848" height="970" alt="Screenshot 2026-09-26 212655" src="https://github.com/user-attachments/assets/273129d8-5f47-4141-adf2-089ab7bf283e" />

---

## Step 2: Using the NETWORKWALKS Password Cracker

- I opened the NETWORKWALKS Password Cracker in the browser.
- The extracted PDF hash was entered into the required input field.
- The password-cracking process was started.
- The web tool tested possible password candidates against the provided hash.
- After the matching password was identified, the recovered password was displayed by the tool.

### Screenshot

<img width="1809" height="1019" alt="Screenshot 2026-09-26 193700" src="https://github.com/user-attachments/assets/6a31e091-b5eb-4448-95ec-329437663162" />

---

## Step 3: Confirming the Recovered Password

- The password displayed by the NETWORKWALKS tool was copied.
- I opened the original protected PDF.
- The recovered password was entered.
- The PDF opened successfully.
- This confirmed that the password obtained through the NETWORKWALKS method was valid.

### Screenshot

<img width="884" height="955" alt="Screenshot 2026-09-26 213221" src="https://github.com/user-attachments/assets/8d64f950-5cf1-4968-a629-9c40cf5d4749" />

---


# What I Learned:-

This practical gave me hands-on experience with password security and offline password-cracking concepts.
**
1. Understanding Password Hashes**

I learned that password-protected files can contain information that allows security tools to perform password-recovery attempts without directly accessing the original password.

I also understood that the extracted hash has to be maintained in the correct format for the cracking tool to process it.

**
2. Working with John the Ripper**

I learned the basic workflow of using John the Ripper for password recovery.

This included preparing a hash, loading it into the tool, selecting a wordlist, starting the attack, and checking the result.

**3. Understanding Wordlists
**
I learned that wordlists contain possible password candidates and are commonly used during dictionary-based password attacks.

The effectiveness of this type of attack depends heavily on whether the target password appears in the selected wordlist or matches the patterns being tested.
**
4. Using Johnny**

I also learned how Johnny provides a graphical way of interacting with John the Ripper.

It made it easier to observe the cracking process and understand what the tool was doing during an attack.

**5. Password Strength**

The practical showed me how passwords based on common words or predictable patterns can be more vulnerable to password-cracking techniques.

This reinforced the importance of using stronger and less predictable passwords.

**6. Importance of Correct Hash Formatting**

I learned that the complete hash needs to be copied correctly.

If characters are missing, changed, or incorrectly formatted, John the Ripper may fail to recognize or process the hash.


# Issues Faced During the Project:- 
**
1. Difficulty Locating the John Executable**

While setting up John the Ripper on Windows, I initially had difficulty locating the required john.exe file inside the extracted installation folders.

The problem was related to identifying the correct directory containing the executable and the required John files.

After checking the extracted folders and reinstalling the required files, I was able to locate the correct John installation directory.

**2. Hash Recognition
**
Another issue was making sure that the extracted PDF hash was copied correctly.

A hash that is incomplete or incorrectly formatted may not be recognized properly by John the Ripper.

Checking the complete extracted value and saving it correctly helped resolve the issue.
**
3. Wordlist Selection**

The cracking process also depends on the wordlist being used.

A small or unsuitable wordlist may not contain the required password, which means the password may not be recovered through that particular dictionary attack.

This helped me understand that the result of a password-cracking attempt depends not only on the tool but also on the attack method and available password candidates.

**4. Working with Johnny**

While using Johnny, I initially had to understand where to load the hash file and how the graphical interface connects with the John the Ripper engine.

After going through the interface and checking the available options, I was able to continue the cracking process.

----


# Security & Ethical Use

This project was performed for educational and authorized cybersecurity learning purposes.

Password-cracking techniques should only be used on files, systems, accounts, or data for which proper permission has been obtained.

These techniques should not be used to gain unauthorized access to someone else's files, accounts, systems, or information.

The purpose of this practical is to understand password security, hash analysis, and defensive cybersecurity concepts in a controlled environment.

---

# Tools & Resources

### John the Ripper

Used for performing offline password recovery and testing password candidates against the extracted hash.

### Johnny

A graphical interface used to interact with John the Ripper during the password-cracking process.

### PDF Hash Extraction Tool

Used to extract the required hash information from the password-protected PDF.

### NETWORKWALKS Hash Calculator

Used to generate the PDF hash required for the NETWORKWALKS password-recovery workflow.

### NETWORKWALKS Password Cracker

Used to demonstrate password recovery through a web-based interface.

### Protected PDF

Used as the target file for the authorized password-recovery experiment.

---

# Key Takeaways

Through this practical, I gained hands-on experience with:

- PDF password protection
- Hash extraction
- Hash formatting
- John the Ripper
- Johnny
- Wordlist-based password attacks
- NETWORKWALKS security tools
- Offline password recovery
- Web-based password recovery
- Password-strength concepts
- Verification of recovered credentials
- Basic cybersecurity ethics

---

# Author

**Javeriya Tahreem**

---

# Project Information

**Program:** Cybersecurity at NETWORKWALKS  
**Week:** 03  

---

# Conclusion

This project helped me understand the practical workflow behind password recovery instead of treating password cracking as just a single command or tool.

By working with **John the Ripper** and **NETWORKWALKS Tools**, I was able to understand how a protected PDF can be converted into usable hash information, how password candidates are tested, and how the recovered password can finally be verified against the original document.

The purpose of this practical is to understand password security and learn how security professionals test the strength of credentials in a controlled environment.
