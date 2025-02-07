# Max's Custom LARB Scripts (McLARBS)

McLarbs is a personalised version of Luke Smith's Auto-Rice Bootstrapping Scripts ([LARBS](https://github.com/LukeSmithxyz/LARBS))

## Installation:

On an Arch-based distribution as root, run the following:

```
curl -LO maxfleming.xyz/McLarbs.sh
sh McLarbs.sh
```


## Main Addititions
- Custom [DWM build](https://github.com/MaxFleming23/dwm)
- Custom [Max-imised Voidrice](https://github.com/MaxFleming23/Max-imised_Voidrice) dot files, including:
  - spreadsheet and word doc file previews
  - extensions for librewolf and codium
  - integration of the below programs...

Programs:
- **Neovim**: *Better than emacs ;)*
	- Luke's defaults for `vim-surround`, `nerdtree`, `goyo`, `vimagit`, `vimwiki`, `airline`, `commentary`, `css-color`.  
	- `vimtex`: use with `:VimtexCompile`, set to read `%! TeX program = lualatex` headers for `tikz-feynman` and related. 
- **VSCodium** + extensions: *VS Code without MS branding/telemetry/licensing*
	- General Enhancements:
		- file-icons: *File-specific icons in the editor.*
		- obsidian-dark: *Dark theme for VSCodium.*
		- markdown-all-in-one: *All-in-one Markdown support.*
		- code-spell-checker: *Spell checker for code.*
	- **Python**: Assorted extensions including jupyter support
	- **LaTeX**:
		- latex-snippets-jeff: *LaTeX snippets for faster coding.*
		- latex-workshop: *Comprehensive LaTeX support.*
	- Other Languages:
		- octaveexecution: Octave language support.
- **Thunderbird**: *Libre email client ...or you could always wrestle with Mutt ;)*
- **Obsidian**: *Knowledge management working on top of local Markdown files ...NON-LIBRE!!!*
- **LibreOffice-Fresh**: *Libre office suite.*
- **Syncthing**: *For cross-pc file syncing*
- **Transmission-cli**: *lightweight CLI torrent client.*
- **Rclone**: *CLI program to manage traditional cloud storage.*

Smaller Packages:
- **neofetch**: *Displays system information in a visually appealing way.*
- **vrms-arch-git**: *Reports non-free packages installed on Arch Linux.*
- **gotop**: *A terminal-based graphical activity monitor writen in go.*
- **zathura-djvu**: *A DjVu plugin for the Zathura document viewer.*
- **djvulibre**: *A software suite for creating and viewing DjVu documents.*
- **gnome-epub-thumbnailer**: *Generates thumbnails for EPUB files.*
- **imagemagick**: *A software suite for creating, editing, and converting images.*
- **odt2txt**: *Converts OpenDocument texts to plain texts.*
- **rsync**: *A fast file copying and synchronization tool.*
- **oath-toolkit**: *Provides tools for OATH-based two-factor authentication.*
- **networkmanager**: *Manages network connections.*


## Other Tips

### PC Dependent Hicups
- Video: for NVIDIA laptops likely needs `xorg` install (as opposed to minimal) with proprietary Nvidia drivers. 
- Audio: may need to play with pulsemixer and the sb-volume script... (pulseaudio?)
- Brightness: play with the sb-brightness script...
- Bluetooth: use `bluetoothctl`...

### Personal Setup
- Librewolf: enable plugins
- SyncThing: connect to devices, set auto-run:
```
systemctl --user enable syncthing.service
systemctl --user start syncthing.service
```
- Codium: run `codium-init.sh`
- Thunderbird: email signin
- Cronie and setup script for calcurse, newsboat...
```
sudo systemctl enable cronie
sudo systemctl start cronie
```
