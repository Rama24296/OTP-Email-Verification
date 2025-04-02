# OTP-Email-Verification

This Python script sends **One-Time Passwords (OTPs)** via email using **SMTP (Gmail)** and verifies user authentication.

## 🚀 Features
- ✅ Sends OTPs to user emails using SMTP (Gmail)
- ✅ Allows multiple users to receive OTPs
- ✅ Provides 3 attempts for OTP verification
- ✅ Secure email transmission with TLS encryption

## 📌 Requirements
- Python 3.x
- A Gmail account with App Passwords enabled
- `smtplib` (built-in)
- `email.mime` (built-in)
## 🔧 Installation
**1. Clone the repository:**
   
   git clone https://github.com/your-username/otp-email-verification.git
   cd otp-email-verification

**2.Run the Script:**

python otp_verification.py

⚠️**Security Warning**

❌ **Do NOT hardcode email credentials** in the script.

✅ Use **environment variables** for storing your Gmail credentials securely.

**Example:**

export EMAIL_USER="lingamguntarama@gmail.com"

export EMAIL_PASS=**"hmlz mrbv okeg ufrm"**

**🔍 How It Works**

1. The script asks how many users need OTPs.

2.	For each user:

       	Generates a random 4-digit OTP
   
       	Sends the OTP to the user’s email
   
       	Asks the user to input the OTP
   
       	Provides 3 attempts for verification

3.	If the user enters the correct OTP → Success ✅

4.	If all attempts fail → Verification Failed ❌

**Example Output:**
**************************************
How many users do you want to send OTPs to? 1
**************************************
Enter your Name: Rama

Enter Email Id: lingamguntarama@gmail.com

Enter OTP Received: 7807

✅ OTP Verification Success!
