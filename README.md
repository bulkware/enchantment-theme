# Enchantment theme

A dark purple colorscheme for XFCE-terminal and VSCodium.


## About

Finding the perfect colorscheme for you is difficult. So I decided to make my
own. And since I primarily use XFCE I included the xfce4-terminal theme too.
Updates are only necessary if something changes ;)

I have no interest in uploading these anywhere else. Feel free to use.


## Color roles

The workbench UI uses a small, deliberate accent palette:

- `#ff00c0` - interactive accent for hover, focus, active borders, and other direct actions.
- `#bf00ff` - primary foreground for readable text, icons, and labels.
- `#4000ff` - structural and inactive accent for boundaries, disabled text, and inactive UI states.


## Installation


**xfce4-terminal colorscheme**

```
mkdir -p ~/.local/share/xfce4/terminal/colorschemes
cp xfce4/terminal/colorschemes/enchantment.theme ~/.local/share/xfce4/terminal/colorschemes
```


**VSCodium theme**

```
mkdir -p /usr/share/codium/resources/app/extensions/
cp -r codium/resources/app/extensions/theme-enchantment /usr/share/codium/resources/app/extensions/
```


# Overriding workbench font family

**IMPORTANT NOTE!**
VSCode and VSCodium doesn't seem to allow the user to set the font family to workbench. For
instance, the file explorer won't change the font family whatever you set in your settings. With
this you can change the font family (among other settings), but it is not generally recommended.

**User installed VSCode and VSCodium:**
C:\Users\<username>\AppData\Local\Programs\<application_name>\<possible_id>\resources\app\out\vs\workbench\workbench.desktop.main.css

**System installed VSCode and VSCodium:**
C:\Program Files\<application_name>\resources\app\out\vs\workbench\workbench.desktop.main.css

```css
/* Override workbench font family */
.monaco-workbench {
  --vscode-font-family: "'Ubuntu Mono'", monospace !important;
}

```
