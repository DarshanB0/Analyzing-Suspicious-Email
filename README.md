#  Analysing Suspicious Email 

## Task Objective

The goal of this task was to **analyze a suspicious email** using a **public email header analyzer** to:
- Understand the structure of an email header
- Identify signs of spam or phishing
- Check if the email was spoofed or forged
- Learn to trace the route an email takes to reach the inbox


## Tools Used
- **MXToolbox Email Header Analyzer**  
  [https://mxtoolbox.com/EmailHeaders.aspx](https://mxtoolbox.com/EmailHeaders.aspx)

- **ChatGPT**  
  Used to generate a sample spam-like email header for analysis and learning purposes

Result :
 - Suspicious links or attachments
   1. Link: http://paypal-login-secure-help.com/verify
   2. paypal.com is not the real domain
   
 - Urget or Threatening Language
   1. “Your account has been limited!”
      “You must verify your account within 24 hours to avoid permanent suspension.”
      
 - Mismatched URLs
   1. Display text: “Click here to verify your account”
   2. Real URL: http://paypal-login-secure-help.com/verify
      hovering would show the real link
      --- doesn’t match the real PayPal domain
      
 - Spelling or Grammar Errors
   1. Spelling is okay, but a real PayPal email would use:
	Better formatting
	Proper branding
	Personalized greeting like “Hello (username)”
	
- Email
	From: PayPal Security <security@paypal-alerts.com>  
	To: darshan123@gmail.com  
	ubject: ⚠️ Urgent: Your Account Has Been Limited!  
	Date: Wed, 5 Jun 2025 11:42:19 +0000  
	Reply-To: verify@paypal-support-help.com  
	Return-Path: <security@paypal-alerts.com>  
	Message-ID: <d9f4a3f0-c25e-4b9f-b234@example.com>  
	Received: from unknownserver.fake.net ([185.22.55.134]) by smtp.inbox.com with SMTP;

	Dear Customer,

	We noticed some unusual activity in your PayPal account. To protect your account, we have temporarily limited your access. You must verify your account within 24 hours to avoid permanent suspension.

	👉 [Click here to verify your account](http://paypal-login-secure-help.com/verify)

	If you don't verify within the given time, your account will be locked permanently.

	Thank you,  
	**PayPal Security Team**  
	**© 2025 PayPal Inc. All rights reserved.**


	⚠️ **Note:** This is an automated message. Please do not reply.

	
```Email Header
Received: from spammy.mail.com ([185.45.12.87]) by mail.mybusiness.com with SMTP;
	Mon, 05 Jun 2025 10:32:14 +0000
From: "PayPal Security" <security@paypal-alerts.com>
To: john.doe@mybusiness.com
Subject: Important: Your account has been limited!
Date: Mon, 5 Jun 2025 10:31:59 +0000
Message-ID: <A123B456C789D@spammy.mail.com>
Reply-To: verify@paypal-helpcenter.com
Return-Path: <security@paypal-alerts.com>
Received-SPF: fail (paypal.com: domain of security@paypal-alerts.com does not designate 185.45.12.87 as permitted sender)
