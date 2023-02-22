# Install Dependencies

## Choco

### https://chocolatey.org/install

### 1) Open Window PowerShell With Administrative Permissions
### 2) Run `Get-ExecutionPolicy`. If it returns `Restricted`, then run `Set-ExecutionPolicy AllSigned` or `Set-ExecutionPolic Bypass -Scope Process`.
### 3) Now run the following command:
```Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))```
### 4) Wait a few seconds for the command to complete.
### 5) If you don't see any errors, you are ready to use Chocolatey! Type `choco` or `choco -?`

## ffmpeg 

### use `choco install ffmpeg` in Windows PowerShell With Administrative Permissions if it says "Already installed" try upgrading using `choco upgrade ffmpeg`

## TinyTex  

### use `choco install tinytex` in Windows PowerShell With Administrative Permissions if it says "Already installed" try upgrading using `choco upgrade tinytex`

# Checking LaTeX

## 1) Open cmd run `refreshenv`
## 2) Then run `latex`
## 3) If it returns `This is pdfTeX, Version 3.141592653-2.6-1.40.24 (TeX Live 2022) (preloaded format=latex) restricted \write18 enabled.` You're good

# Installing Optional Dependencies

## 1) Open new terminal(Ctrl+C) and Run the following commands one by one(use the next one after the completion of first):

## `tlmgr install amsmath babel-english cbfonts-fd cm-super ctex doublestroke dvisvgm everysel`
## `tlmgr install fontspec frcursive fundus-calligra gnu-freefont jknapltx latex-bin`
## `tlmgr install mathastext microtype ms physics preview ragged2e relsize rsfs`
## `tlmgr install setspace standalone tipa wasy wasysym xcolor xetex xkeyval`
## `choco install wget git`

# NOTE: Incase tinytex fails to get installed, install MikTex from "www.miktex.org/download". After installing, Open MikTex, go to "Updates" click "Check for updates" and click "Update now"and that's it!

# Installing Python:

## Go to https://www.python.org/downloads/ and download Python version `3.10` or lower(All dependencies ane not compatible with higher versions)
## Download by choosing `Download Windows installer (64-bit)`
## While installing Python, make sure to check the `Add Python (version) to PATH` at the installation dialog box.
