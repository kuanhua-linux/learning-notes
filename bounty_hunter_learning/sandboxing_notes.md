# Firejail Notes

## Installing Firejail

```bash
sudo apt install firejail
```

### Observation
Linux package names are usually lowercase.

Example:

```bash
sudo apt install Firefox
```

fails because Linux systems are case-sensitive. Because Linux package manager
treats uppercase and lowercase differently, the package name 'Firefox' could not be
found.


The correct way:

```bash
sudo apt install firefox
```

---

## Running Firefox Sandboxed

```bash
firejail firefox
```

# What is Firejail used for?

It is useful for:
-scripts
-unknown binaries
-testing tools 
-isolated applications
-research environment 
-reducing exposure
-lightweight alternative to large virtual machines
-safer experiment 


Example:

### For suspicious python file

```bash
firejail python3 sus_script.py

```

### for mp4 

VLC stands for Video LAN Client.

```bash
firejail vlc weird_video.mp4
```

### suspicious  docx

```bash
firejail libreoffice suspicious.docx
```

note: most of the file or executable, look normal, and in today's technology
AI can make perfect email, phishing, and those malicious actors often exploit
human psychology and trust. So be careful downloading malicious file on the
internet and workplaces.
 
##AI-Assisted Social Engineering

AI tools can imitate:
-voices
-writing styles
-emails
-phone calls

For example:

An attacker could imitate a company executive or manager using AI-generated 
voice cloning.

An employee might trust the fake request because:
-the voice sounds familiar
-the person appears authoritative
-the request sounds urgent

This can lead to:
-credential theft
-data leaks
-unauthorized access
-financial scams

attackers often exploit human trust more than technical vulnerabilities.
