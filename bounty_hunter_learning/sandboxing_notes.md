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

fails because Linux systems are case-sensitive. Because Linux manager treats 
uppercase and lowercase differently, the package name 'Firefox' could not be
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

### Purpose
- reduce system exposure
- isolate applications
- safer experimentation
- lightweight alternative to large virtual machines
