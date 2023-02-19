# resume

A fork of `sb2nov/resume` but it's my resume instead.

# Usage

First, you must populate `personalinfo.sty` with your personal information.  Such information is not committed onto GitHub.  The file should look like:

```latex
\ProvidesPackage{personalinfo}

\newcommand{\email}{XXX@XXX.XXX}
\newcommand{\phone}{+X (XXX) XXX-XXXX}
```

Next, just run `build.sh` or `Build.ps1` (depending on OS) to build the PDFs.

# Installation

Doing a full TeXLive installation should be sufficient, but if there are packages you need, you can do the following:

### Linux

```sh
cat texlive_packages.txt | xargs tlmgr install
```

### Windows

```
curl -o xargs.cmd https://raw.githubusercontent.com/DoctorLai/BatchUtils/master/xargs.cmd
cat texlive_packages.txt | ./xargs tlmgr install
```

## Dumping Installed Packages

```sh
tlmgr list --only-installed --data name > texlive_packages.txt
```