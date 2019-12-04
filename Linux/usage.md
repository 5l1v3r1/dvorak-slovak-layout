- Append the dvorak-ext content to /usr/share/X11/xkb/symbols/us, after the `dvorak` layout description.

- Modify the /usr/share/X11/xkb/rules/evdev.xml accordingly:

```
<variant>
  <configItem>
    <name>dvorak</name>
    <description>English (Dvorak)</description>
  </configItem>
</variant>
<variant>
  <configItem>
    <name>dvorak-ext</name>
    <description>English (Dvorak) Extended (PL, SK, CZ)</description>
  </configItem>
</variant>
<variant>
```

```
setxkbmap us dvorak-ext
```
