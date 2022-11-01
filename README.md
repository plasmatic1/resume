# resume

A fork of `sb2nov/resume` but it's my resume instead.

# Usage

Run `build.sh` or `Build.ps1` to build documents.  MAKE SURE TO DO THIS BEFORE COMMITTING.

## Installing Packages

I just use the LaTeX Workshop extension for VSCode to handle all of the building, but you still have to install the packages.

The required packages in `texlive_packages.txt`.  Installation is below:

### Linux

```sh
cat texlive_packages.txt | xargs tlmgr install
```

### Windows

```
curl -o xargs.cmd https://raw.githubusercontent.com/DoctorLai/BatchUtils/master/xargs.cmd
cat texlive_packages.txt | ./xargs tlmgr install
```

## Dump Installed Packages

```sh
tlmgr list --only-installed --data name > texlive_packages.txt
```

_Note: I'm pretty sure that the installed packages is way more than is required to build the Resume, but I just dumped my current installation of TexLive, which only contains 5 or so packages that weren't already installed by default_