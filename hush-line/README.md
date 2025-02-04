# **🤫 Hush Line Project Info**

[Read the (in-progress) whitepaper](https://github.com/scidsg/project-info/blob/main/hush-line/whitepaper-draft.md)

## Info

Hush Line is a free and open-source, self-hosted anonymous tip line that makes it easy for organizations or individuals to install and use. It's intended for journalists and newsrooms to offer a public tip line; by educators and school administrators to provide students with a safe way to report potentially sensitive information, or employers, Board rooms, and C-suites for anonymous employee reporting. 

## Ecosystem

<img src="https://github.com/scidsg/project-info/assets/28545431/22069bbe-8bd0-4d1d-bd92-03b840e1d934" width="80%">

### Links

- [Overview Deck](https://docs.google.com/presentation/d/1XLdqN527118WWlS2Idof2wI3ZuxqDg7Vd2CDmxSFKk4/edit?usp=sharing)
- [Website](https://hushline.app/)
- [Demo App](https://try.hushline.app/)
- [Documentation](https://scidsg.github.io/hushline-docs/book/intro.html)
- [Git Repo](https://github.com/scidsg/hush-line)
- [Donations](https://opencollective.com/scidsg/contribute/hush-line-support-55786)
- [Figma](https://www.figma.com/file/0IlWj8IwEgRg8vP1XEdjO2/Hush-Line?type=design&node-id=502%3A673&mode=design&t=Ni2HtEiQcrECy8CC-1)

## Team

Are we missing any roles? Edit this document!

| Role          | Person        | Keybase Contact    |
|---------------|---------------|--------------------|
| Lead          | Glenn         | @glennsorrentino   |
| Lead Engineer | _Glenn_       | _@glennsorrentino_   |
| Engineering   | Sam           | @schlink           |
| Research      | Abbey         | @bodicea           |
| Design        | Glenn         | @glennsorrentino   |
| Social        | _Glenn_       | _@glennsorrentino_   |
| Localization  |               |                    |
| Documentation | _Glenn_<br>Sam  | _@glennsorrentino_<br>@schlink               |

_Italics indicate a temporarily filled role._

## Why Hush Line?

Other tools in this space include SecureDrop and GlobalLeaks, two robust, widely adopted whistleblowing platforms whose installation can be complicated for non-technical users. Some systems require an admin to configure it and special infrastructure for it to operate. The security posture of these platforms is increased because the chances are high that you'll receive malicious and dirty data when you allow people to send you files anonymously. Both require significant time and money to manage. It's not much easier for the person sending a message, either. They might have to create accounts, download new software, or manage PGP keys. It requires a significant commitment. Even tools like Signal or Protonmail require end-users to reveal information about themselves unless they can find disposable phone numbers and email addresses. Not a requirement everyone feels comfortable with.

In contrast, Hush Line is a text-only, one-way messenger that is the first handshake in a relationship where two parties want to exchange information. It's a low-risk method of offering a safe channel for someone to reach you without requiring them to reveal anything about themselves, create an account, manage PGP keys, or acquire a burner phone, email address, or phone number.

The tool deploys to either an onion-only instance or Tor + public web. Hush Line is a web and email server and a Python app that encrypts messages with your public PGP key once a message gets submitted, then saves it, and finally emails the encrypted message to you. Your data never gets saved in an unencrypted state. And since all messages are sent to your email, you never have to log in to the device.

We configure Nginx with hardened security headers so no external and potentially nefarious resources can load, automatically set up renewing Let's Encrypt HTTPS certificates so your data is always transmitted safely, privacy-preserving logging which scrubs IP addresses before saving to server logs, and enable automatic updates by default so you never miss a critical security patch.

You only need a public PGP key on a keyserver and an SMTP-compatible email address. We ask for your key this way because uploading it includes verifying your email address, which helps us know you are who you say.

Built with popular and ubiquitous hardware and software in mind, Hush Line works seamlessly on Raspberry Pi and Debian-based operating systems. You can even add an e-paper display to make your Hush Line address easy to discover.

We offer a solution for those who want to help, who might have reportable or actionable information, but don't want to face retaliation or take on the risks of getting involved. In fact, over 70% of people have witnessed or experienced workplace harassment. Only 15% of those people ever make a formal written complaint. About 1% ever has something done about it. That's a big oversight for employers, which could become a significant liability left unattended. And the reason people don't report? They're afraid of retaliation.

How much better, safer, and more informed could our schools, workplaces, and society be with a safe way to share information that places the privacy of communities first?

## Users

- Journalists and newsrooms can use Hush Line to give the public a safe way to leave a confidential tip.
- Employers and board rooms can use Hush Line to build trust by allowing colleagues to leave suggestions or report concerns anonymously.
- Educators and school staff can use Hush Line to host a safe way for students to share information with someone they trust.

## Use Cases

- As a journalist, I need to provide sources with a trustworthy way to send information, so they have confidence that the methods will protect their privacy.
- As an educator, I need to provide students with a safe way to share information with school staff they trust, so critical information can be received while protecting the student's identity.
- As an employee that has witnessed workplace abuse, I need a secure and private way to share information with company executives, so that my identity is kept secret to avoid provoking a hostile retaliatory response.
- As a student, I want a way to report sensitive information without sharing who I am, so I can help to make change without impacting my educational experience.
- As a business leader, I want to make my team feel like they can share sensitive information without risking their career, so I can build trust in the team with which I work.
- As a source, I need a way to access someone's Hush Line, even if the Tor Network and the original URL are blocked in my country, so I can share information even in the most oppressive environments.

## Locations

- Global
- Areas where censorship is prevalent, including Iran, China, Russia, and Belarus

## Grant History

| **Organization** | **Support Type** | **Vendor** | **Services** | **Status** | **Dates** |
| --- | --- | --- | --- | --- | --- |
| StartSmall, LLC | Financial | Project-Specific | 
| OTF | Services | Red Team Lab | Security Audit | ✅ Awarded | July 2023 |
| OTF | Services | A11y Lab | Accessibility Audit | ✅ Awarded | July 2023 |
