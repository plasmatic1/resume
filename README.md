# resume

A fork of `sb2nov/resume` with my own resume and some additional features, including:

* Modularized resume made up of independent, swappable components
* Personal info module that hides information from the web
* GitHub actions to automatically compile anonymized versions of your resume whenever you push

# Usage

1. Install TexLive
    * Default full installation is sufficient
2. Populate a new file `personalinfo.sty` with your personal information, following the format of `presonalinfo_default.sty`
    * `personalinfo.sty` is not committed onto GitHub
3. Run `build.sh` or `Build.ps1` (depending on OS) to build the resume

<!-- # Installation

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
``` -->
