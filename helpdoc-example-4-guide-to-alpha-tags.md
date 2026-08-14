# Helpdoc Structural Pattern Example: Step-by-Step How-To Article

Source: https://help.clicksend.com/en/articles/44195-guide-to-alpha-tags

This example demonstrates the pattern for a how-to article that mixes conceptual sections, a numbered step-by-step process with an inline screenshot, and a long reference list at the end. Note the image is placed directly after the step it illustrates, not bundled elsewhere.

---

[H1] Guide to Alpha Tags
[ENTER]
[DIVIDER]
[H2] What are Alpha Tags
[ENTER]
An Alpha Tag (short for alphanumeric sender ID) is a custom sender ID name, such as your business name. Alpha Tags are often used by businesses to promote brand recognition and trust. Alpha Tags are limited to 11 characters and cannot include special characters or spaces. Compliance with regional regulations is a must when using Alpha Tags.
[ENTER]
[DIVIDER]
[H2] When to choose them
[ENTER]
Use an Alpha Tag if:
[ENTER]
- You want your messages to come from a recognizable brand name instead of an anonymous number. This builds credibility and helps customers instantly identify your business.
- You only need one-way messaging. Alpha Tags don't support replies from your recipients.
- You send SMS to countries that support Alpha Tags.
[ENTER]
[DIVIDER]
[H2] Register a global Alpha Tag
[ENTER]
Global Alpha Tags can be used in all countries which allow Alpha Tags without additional registration. If you are sending to a country which does not require network registration for Alpha Tags, you can register via the API or via the dashboard. In countries requiring additional verification, registration with local network operators may be necessary — specific conditions and approval processes are outlined on the ClickSend Dashboard.
[ENTER]
Alpha Tags must clearly represent your brand or business name. Avoid generic or unrelated names, as they will be rejected. Tags cannot exceed 11 characters and must not include special characters or spaces.
[ENTER]
1. Log into the Dashboard.
2. Navigate to Sender IDs > Manage Senders > Alpha Tags.
3. In the Alpha Tags section, click the Add button to register a new Alpha Tag.
4. Follow the on-screen prompts.
5. Ensure the Alpha Tag represents your brand or business name, is no longer than 11 characters, and avoids special characters or generic terms — incompatible tags will be rejected.
[ENTER]
[IMAGE: Screenshot of the Add Alpha Tag registration screen in the ClickSend dashboard]
[ENTER]
Once you've submitted your registration, it will be sent to our team to review and approve. This typically takes around 24 hours. Once your Alpha Tag has been approved, you can start using it to send via Quick SMS and SMS Campaign. If the Alpha Tag is rejected, review the reasons provided and make necessary corrections before reapplying. Compliance with submission guidelines greatly improves approval chances.
[ENTER]
We will notify you via email if registration was successful or if we need more information before we can proceed.
[ENTER]
[DIVIDER]
[H2] Using Alpha Tags across multiple countries
[ENTER]
The same Alpha Tag can be used for multiple destinations under certain conditions:
[ENTER]
- Global Alpha Tags are valid in countries that do not mandate additional local registration.
- For regions requiring local registration, like Nigeria, the approval process must be completed first, after which the tag might also apply globally to compatible areas.
- Always verify the specific rules of your target country to ensure compliance.
[ENTER]
[DIVIDER]
[H2] Register a local Alpha Tag
[ENTER]
A local Alpha Tag can only be used in the country you registered it. These Alpha Tags always require additional registration. Examples of such countries include Nigeria and regions in the Middle East, where local registration steps must be followed for usage approval.
[ENTER]
If you are sending to a country which requires network registration for Alpha Tags, simply contact us via our 24/7 chat support and we'll guide you through the process. You may need to provide documentation such as your business details, example messages, and the type of content being sent to ensure compliance. Registration is free of charge, but approval processes and documentation requirements might vary by country. Special provisions apply if registering for third-party brands, such as including proof of authorization and affiliation.
[ENTER]
The information we need varies by country, but some examples include:
[ENTER]
- The Alpha Tag you'd like to use.
- Your business details.
- Your website URL.
- Examples of the messages you'll send.
- The type of content you'll be sending.
- If registering third-party Alpha Tags: authorization letters, proof of affiliation (e.g. co-branded materials), and official contracts.
[ENTER]
[DIVIDER]
[H2] Banned Alpha Tags
[ENTER]
Unfortunately, smishing and phishing are on the rise. To help keep our customers safe, we have put rules and restrictions in place. We don't allow the registration of Alpha Tags that are generic or associated with well-known trademarks.
[ENTER]
If the Alpha Tag you wish to use is on the list but you have a legitimate use case, please contact support.
[ENTER]
Find a list of prohibited generic Alpha Tags below:
[ENTER]
1TimePin, 2FA, Accept, Access, Account, Accounts, Active, Admin, Advice, Alert, Allow, Allowance, Anti-fraud, App, Appointment, Approve, Approved, Assist, Assistance, Auth, AuthMsg, Authorise, Aware, Bank, Banking, Bill, Billing, Call, Card, Caution, Certify, Check, CloudOTP, Code, Collect, Collection, Confirm, Contact, Control, Courier, Delay, Deliver, Delivery, DoNotReply, Energy, FollowUp, Fraud, Help, Important, Info, InfoSMS, ISA, Key, Loan, Logistics, LogMeIn, Logon, Malware, Message, Mobile, Mortgage, MSG, MsgAuth, Network, NoReply, Notice, Notify, OneTimePin, Order, OTP, OTPSMS, Overdue, Package, Parcel, Password, Pay, Payment, PhoneCode, Pin, PinCode, Post, Protocol, Purchase, Ratify, Rebate, Recall, Receipt, Refund, Reminder, Repayment, Reply, Reschedule, Response, Results, Sale, Save, Saving, Scam, Schedule, Secure, Security, Service, Shipping, Sign, Signin, Signon, SMS, SMSAuth, SMSCode, SMSInfo, SMSOTP, SMSVerify, Support, System, Tax, Test, Text, Trace, Track, Tracking, Trust, TXT, Update, Updates, Urgent, Validate, Verified, Verify, VerifyMe, VerifySMS, Virus, Warn, Warning, Wholesale, Winner.
