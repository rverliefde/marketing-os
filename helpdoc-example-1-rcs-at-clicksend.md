# Helpdoc Structural Pattern Example: Overview / Feature Explainer Article

Source: https://help.clicksend.com/en/articles/68247-rcs-at-clicksend

This example demonstrates the pattern for a broad "what is this feature" overview article: an intro, several major H2 topics (some with hidden H3 sub-structure), reference tables, and a closing FAQ block.

---

[H1] RCS at ClickSend
[ENTER]
This guide provides an overview of Rich Communication Services (RCS) at ClickSend, including its features, benefits, and how to get your business set up.
[ENTER]
[DIVIDER]
[H2] What is RCS?
[ENTER]
Rich Communication Services (RCS) is the next generation of business messaging. It is designed to create a more trustworthy, engaging, and measurable communication experience compared to traditional SMS.
[ENTER]
With RCS, your business can send messages from a verified, branded sender profile and receive read receipts. This helps your customers feel confident that your messages are legitimate and allows you to better understand their engagement.
[ENTER]
If you want to get RCS via API please reach out to our friendly sales team who can help qualify you and guide you through the set-up process (sales@clicksend.com).
[ENTER]
[DIVIDER]
[H2] Why RCS is powerful
[ENTER]
RCS offers two significant advantages over standard SMS.
[ENTER]
[H3] Verified & trusted sender identity
[ENTER]
RCS messages come from a branded profile that immediately tells customers who you are.
[ENTER]
[IMAGE: Example of a verified RCS Sender ID profile showing the checkmark, company name and logo]
[ENTER]
The verification tick is issued by Google and un-fakeable. This means that your customers can trust your messages and that there is a reduced chance of your messages being mistaken as spam.
[ENTER]
Your branded RCS Sender ID will include:
[ENTER]
- Verified Sender Badge: a checkmark indicating your business is verified by Google, Sinch ClickSend and the participating carriers.
- Company Name: your business name is displayed as the Sender ID.
- Company Logo: your logo appears next to your business name.
- Business Details: a brief summary of what your business does, as well as your website and business contact details.
[ENTER]
[IMAGE: Example of a full RCS Sender ID profile card with business details]
[ENTER]
[H3] Read receipts & engagement visibility
[ENTER]
RCS supports read receipts, so you can see when your messages have been opened.
[ENTER]
[IMAGE: Screenshot of a read receipt appearing on an RCS message]
[ENTER]
This delivers:
[ENTER]
- Better engagement measurement: understand what content works.
- More accurate timing for follow-up messages: fine-tune your strategy.
- Stronger performance insights than SMS alone: make data-driven decisions.
[ENTER]
[DIVIDER]
[H2] Available features at ClickSend
[ENTER]
Our current RCS solution focuses on providing a trusted sender identity and enhanced reporting via read receipts for API customers.
[ENTER]
What's available now:
[ENTER]
- API access for integration.
- A simple, no-code setup process: send through your usual SMS API endpoints (successful RCS application required).
- Verified sender profile with your brand name and logo.
- Read receipts to track engagement.
- Two-way messaging capabilities.
- Automatic SMS fallback for devices that do not support RCS.
[ENTER]
Coming soon:
[ENTER]
- RCS messaging in the public dashboard.
- RCS registration via self-service.
[ENTER]
If you want to try RCS via API please reach out to our friendly sales team who can help qualify you and guide you through the set-up process (sales@clicksend.com).
[ENTER]
[DIVIDER]
[H2] Best use cases for RCS
[ENTER]
RCS is most effective in scenarios where trust and delivery confirmation are critical.
[ENTER]
| Use Case | Description |
|---|---|
| OTP & Verifications | Securely send one-time passcodes and verification messages from a trusted source. |
| Appointment Reminders | Reduce no-shows with branded reminders that customers can trust. |
| Confirmations & Alerts | Send order confirmations, shipping alerts, and other important notifications. |
| Critical Customer Updates | Ensure your most important messages are seen and acknowledged. |
| High-Trust Marketing | Build confidence in your marketing campaigns with a verified sender profile. |
[ENTER]
[DIVIDER]
[H2] RCS availability & requirements
[ENTER]
RCS availability is dependent on the recipient's country, mobile carrier, and handset. Android phone operating systems have wider coverage than iOS. The mobile handset must be RCS capable to receive RCS messages.
[ENTER]
| Support Level | Support Definition | Regions |
|---|---|---|
| Fully Supported | All carriers and phone operating systems supported | France, Germany, Spain, United Kingdom, United States |
| Partially Supported | Not all carriers and/or phone operating systems are supported (often Android only) | Austria, Belgium, Brazil, Canada, Czech Republic, Denmark, Finland, Italy, Mexico, Netherlands, Norway, Poland, Portugal, Singapore, Slovakia, Sweden |
| Not Currently Supported | RCS not supported for A2P (application to person, i.e. business messaging) | Australia and most other regions |
[ENTER]
[DIVIDER]
[H2] How to apply for an RCS Sender Profile
[ENTER]
To send RCS messages, your business must complete a Sender Agent application with Google and network carriers. The process can take up to 12 weeks to complete.
[ENTER]
Please get in touch with our friendly sales team to help qualify you at sales@clicksend.com.
[ENTER]
[H3] Application requirements
[ENTER]
Requirements differ on a country basis, but at a minimum you will need to provide the company brand details for your customer-facing RCS Sender ID, your company's business verification details, and your RCS usage details for the application with Google and Sinch.
[ENTER]
[CALLOUT]
Customer-facing details cannot be edited after your RCS Sender ID is verified. Each change will require you to launch a new application.
[ENTER]
| Information | Requirements |
|---|---|
| Company or brand name | 40 character limit. Best kept to 15–25 alphanumeric characters to avoid truncation on-device. |
| Logo | 224 x 224 pixels, max 50KB. |
| Company or brand description | 100 character limit, shown when a customer clicks your RCS Sender ID profile. |
| Banner background image | 1440 x 448 pixels, max 200KB. |
| Brand colour | Must have a contrast ratio of at least 4.5:1 against white (#FFFFFF). |
| Business contact phone / email / website | Displayed in your RCS Sender ID profile. |
| ClickSend user ID | The account you want to send RCS messages on. |
| Legal company name, owner/representative details, company address | Used for business verification with Google & Sinch. |
| Privacy policy & Terms & Conditions | Live, working URLs required. |
| Region, country, use case | Choice of Europe, US, Asia, South America; a separate application is required per region. Use case is one of Promotional, OTP, Transactional or Multi-use, and traffic is restricted to the approved use case. |
| Message triggers & customer interactions | How messages are triggered and how customers interact with you afterwards. |
| Opt-in mechanism & visual proof | How customers opt in, plus a URL or screenshot showing the mechanism. |
| Opt-out messaging | The message customers receive when they opt out. |
| RCS test number | A number to test RCS ahead of final approval. |
| SMS fallback number | The Sender ID used to send an SMS if the recipient's handset can't receive RCS. Defaults to any available, compliant Sender ID on your profile if not provided. |

[FAQ]

[EXPANDABLE]
Question: Can my phone receive RCS messages?
Answer: Yes, if you're in an RCS approved country, on an RCS approved carrier, with an RCS approved operating system (Android or iOS), and your handset is RCS capable.

[EXPANDABLE]
Question: My phone is RCS capable but I can't see RCS, what do I do?
Answer: Check that RCS is turned on in your native messaging app — Google Messages on Android, or Messages on iOS.

[EXPANDABLE]
Question: Why aren't URLs hyperlinked in the RCS messages I receive?
Answer: This is usually related to the handset or third-party apps/VPNs interfering with RCS functionality (for example, iPhone 13 mini). Try restarting the phone, toggling RCS Messaging off and on in Settings > Apps > Messages, performing a force restart, or long-pressing the message to signal to iOS that the sender is trusted.

[EXPANDABLE]
Question: Can I continue to send messages while my RCS application is being processed?
Answer: Yes. You can continue to send from Alpha Tags, Dedicated Numbers and shared numbers (if available for your country) while your RCS application is being processed.

[EXPANDABLE]
Question: What is my SMS fallback number?
Answer: This is the default Sender ID you specified via Smart Senders (e.g. a shared number, dedicated number or alpha tag). When RCS can't be delivered due to the recipient's handset or carrier network, your message is delivered as an SMS from this fallback Sender ID.

[EXPANDABLE]
Question: Can I send RCS messages via the dashboard?
Answer: RCS is an API-only product for now. Dashboard support is planned for the future.
