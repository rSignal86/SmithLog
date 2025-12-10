# SmithLog — Universal Cabrillo → ADIF Converter

A lightweight, browser-based tool built *by a ham, for hams* to convert contest logs from **Cabrillo** format to **ADIF**, ready for uploading to QRZ.

---

## Why SmithLog?

I'm not saying that SmithLog is the best program in the world to do this, there are other programs that do a very good job and offer more flexibility.
ADIF Master and Contest LogChecker are better for heavy post-Processing, while my program does something specific like converting data without having a program installed on your computer, plus it's the same program across all devices you use since everything is in a single HTML file.

## Features

- **Automatic contest detection** with provision for comments.
- **Quick and easy**: Paste or upload your Cabrillo log, click **Analyze (F4)**, then **Generate ADIF (F10)**. Done.
- **ADIF 3.1.6 compliant**: Outputs ADIF according to the latest published specification.
- **Smart Contest Detection**: Automatically identifies `CONTEST_ID`. If unknown, the contest name is added as a comment.
- **Interactive Column Mapping**: Click on yellow "unknown" headers to map to the correct ADIF fields (e.g. `STX`, `SRX`, `STX_STRING`, `SRX_STRING`).
- **Propagation and Meta Fields**: Optional global fields for `TX_PWR`, `K_INDEX`, `A_INDEX`, `SFI` and a global comment to be added to the QSO to QRZ.
- **Web-based**: No installation, works on all operating systems and web servers.
- **Global Options**: specify `TX Power`, `K-Index`, `A-Index`, `SFI` and a global comment that is added to all comments at once.
- **QRZ-ready**: ADIF file is uploaded cleanly to QRZ and other services.

--

## Instructions

1. **Load your log**
Upload `.log`/`.txt` or paste Cabrillo content.
2. **Analyze** (**F4**)
SmithLog detects competition and columns.
3. **Check column mapping**
Click on yellow headers to map ADIF fields. Use `STX`/`SRX` for numbers, `STX_STRING`/`SRX_STRING` for text exchanges.
4. **(Optional) Fill in global fields** Add `TX Power`, `K-Index`, `A-Index`, `SFI` and global comment.
5. **Generate ADIF** (**F10**) Download `.adi` ready for upload.

## Comparison with other good tools
There are several excellent tools for Cabrillo → ADIF conversion:
- **ADIF Master (Windows)** – Advanced ADIF editor with import from Cabrillo, CT, TR, etc. Great for batch editing and statistics.
- **LogConv (Windows)** – Simple format converter (Cabrillo ↔ ADIF, CT9/10, EQF, TR Log).
- **CBR2ADIF (CLI)** – Command line tool for Cabrillo → ADIF, good for automation.
- **Contest LogChecker (Windows)** – Powerful validator and converter with additional features.

**Where SmithLog is better:**

1. **Browser-based, no installation** Works on macOS/Linux without admin rights.
2. **Intuitive mapping for contest Exchanges, it only shows you want you need.
3. **ADIF 3.1.6 compliance by design** Ensures modern compatibility with QRZ and other services.
4. **Simple tool that do one thing.

---

## Format references

- **ADIF 3.1.6**: https://adif.org/316/ADIF_316.htm
- **Cabrillo v3**: https://wwrof.org/cabrillo/cabrillo-v3-header/

---

## FAQ

**Does SmithLog include both `STX` and `STX_STRING`?**
Yes, numeric and textual exchanges are preserved.

**Does it run on macOS/Linux?**
Yes, it is browser-based.

**Does it run on a web server?**
Yes, it was designed to run on a web server from the start on the Your Club web server, but it uses reference material from GitHub.

**Can I contribute back to SmithLog?**
Yes you can, make your changes and submit them via GitHub and if I like them I'll add them to main, include your name with the changes.
I also welcome suggestions, you can find my contact information on QRZ.

**Can anyone use it?**
Yes, you can find it useful, you can use it, and it's completely free and open source.

**Support if I make a mistake?
No, I don't offer individual support if you have mapped your data incorrectly and you discover that there is incorrect data on QRZ.
You are responsible for mapping data for export.
---

## Changelog

**GHv1.1 – 2025-12-10** *(latest version)*

- New compact and modern UI – significantly better on laptops, tablets and phones
- Completely redesigned footer with larger Norway badge and prominent GitHub link
- Version checker is now 100 % secure – uses GitHub Releases API (no longer downloads raw HTML)
- Generated ADIF files are tagged with **SmithLog GHv1.1**
- Smaller buttons, fonts and spacing for a cleaner look on smaller screens
- Improved accessibility (ARIA attributes added)
- Scrollable help modal on small devices
- Minor humorous console messages for curious users
- Reduced network usage – update check now checks only every 12 hours

**GHv1.0 – 2025-12-09**

- First public release
- Fully functional Cabrillo → ADIF converter

## ScreenShots

here is some images of the program:

### When you start the program 

![Image alt](https://github.com/rSignal86/SmithLog/blob/main/assets/screenshot/OnBoot.png)


### Before you have analyzed the Cabrillo file 
![Image alt](https://github.com/rSignal86/SmithLog/blob/main/assets/screenshot/BeforeAnalyze.png)


### After you have analyzed the Cabrillo file 

![Image alt](https://github.com/rSignal86/SmithLog/blob/main/assets/screenshot/AfterAnazlye.png)



## License
MIT (see `LICENSE` in the repo).
``
