# Welcome to Free Resources Collections!

Hi! I thought that why not share my small resources collection with others at the end of 2021. As an **open sources** lover, I should do it. This is just a Begin. If You also want to contribute to this collection then **send a pull request** with a proper description of your request and then if all is okay I will merge the request.

# Basic Linux Command Cheet Sheet Based On MFU Distro

|Descriptions        |Arch               |Red Hat/Fedora      |Debian/Ubuntu       |SLES/openSUSE       |Gentoo             |
|--------------------|-----------------|-----------------------------|-----------------|----------------|-------------------|
|Install a 
package(s) by name|`pacman -S`  |`Idnf install`  |`apt install` | `zypper install` or `zypper in` | `emerge [-a]`|
| Remove a Packages by name | `pacman -Rs`    | `dnf remove`   | `apt remove` | `zypper remove` or `zypper rm`   | `emerge -a[a]vc`|
| Search for package(s) by searching the expression in name, description, short description.What exact fields are being searched by default varies in each tool. Mostly options bring tools on par.|`pacman -Ss` |`dnf search` |`apt search`| `zypper search` or `zypper se [-s]` | `emerge -S`|
| Upgrade Packages - Install packages which have an older version already installed | `pacman -Syu`| `dnf upgrade`|`apt update` and then `apt upgrade`|`zypper update` or `zypper up`|`emerge -[a]uDN @world`|
| Upgrade Packages - Another form of the update command, which can perform more complex updates -- like distribution upgrades. When the usual update command will omit package updates, which include changes in dependencies, this command can perform those updates. | `pacman -Syu` | `dnf distro-sync` | `apt update` and then `apt dist-upgrade` | `zypper dup` | `emerge -[a]uDN @world` | 
| Clean up all local caches. Options might limit what is actually cleaned. | `pacman -Sc` or `pacman -Scc` | `dnf clean all` |`apt autoclean` removes only unneeded, obsolete information or `apt clean` | `zypper clean` | `eclean distfiles`|
| Remove dependencies that are no longer needed, because e.g. the package which needed the dependencies was removed. | `pacman -Qdtq \| pacman -Rs -` |` dnf autoremove` |`apt autoremove	`|`zypper rm -u`  (just for removing a package) or `zypper packages --unneeded` (listing only and without recursion) |`emerge [-a] --depclean` |
| Remove packages no longer included in any repositories. | `pacman -Qmq \| pacman -Rs -` |`dnf repoquery --extras`|`aptitude purge '~o'`|
|Mark a package previously installed as a dependency as explicitly required.| `~pacman -D --asexplicit`| `dnf mark install` | `apt-mark manual` | `zypper install --force` (workaround which needs to reinstall the package)|`emerge --select`|
| Install package(s) as dependency / without marking as explicitly required.| `pacman -S --asdeps`| `dnf install` and then `dnf mark remove` |`apt-mark auto`| |`emerge [-a] --oneshot` or `emerge [-a] -1`|
|Only downloads the given package(s) without unpacking or installing them|`pacman -Sw`|`dnf download`|`apt install --download-only`(into the package cache) or`apt download`(bypass the package cache)|`zypper --download-only`|`emerge [-a] --fetchonly`|
