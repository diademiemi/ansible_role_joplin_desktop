# Ansible Role Joplin Desktop
This is an Ansible role that installs Joplin Desktop on Linux. It can use the AppImage or Flatpak package.  

Tested on Fedora 36 and Ubuntu 22.04, should work on any Linux distribution that the Joplin Desktop AppImage or Flatpak package supports.  

## Requirements

### Base requirements
None  

## Variables
| Variable | Default | Description |
|----------|---------|-------------|
| `joplin_desktop_version` | `0.18.0` | Version of Joplin Desktop to install. |
| `joplin_desktop_package_format` | `appimage` | How to install the package. To use `flatpak` you need `flatpak` installed. Options: `[appimage, flatpak]` |
| `joplin_desktop_appimage_package` | `https://github.com/laurent22/joplin/releases/download/v{{ joplin_desktop_version }}/Joplin-{{ joplin_desktop_version }}.AppImage` | URL to the AppImage package. |
| `joplin_desktop_flathub_package` | `https://dl.flathub.org/repo/appstream/net.cozic.joplin_desktop.flatpakref` | The Flatpak package to install. |