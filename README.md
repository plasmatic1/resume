# resume

**Note: Due to privacy reasons, I'll be privatizing any further changes to my resume and archiving this repository.**

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
