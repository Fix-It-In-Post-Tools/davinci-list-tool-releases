# DaVinci List Tool

Lists for turnover, made inside DaVinci Resolve Studio: EDLs, change lists, opticals lists and
marker reports. Free. Currently in beta.

**[Download the latest version](https://github.com/Fix-It-In-Post-Tools/davinci-list-tool-releases/releases/latest)**

| Tab | What you get |
|---|---|
| **EDL Export** | CMX3600, File32 and File129 EDLs from any timeline, with per-track selection, transitions, speed changes and the clip metadata you choose as comment lines. |
| **Change List** | Compare an old cut with a new cut. A change list in the Avid List Tool style with 35mm or 16mm footage, a changed-shots EDL, Avid locators, or markers added to the new cut. |
| **Opticals List** | Dissolves, fades, wipes, speed changes, freezes, superimpositions and repositions. |
| **Markers** | Timeline and clip markers in one table, with optional frame thumbnails. Export to CSV, tab-delimited text, Excel or a PDF report. |

Settings on every tab can be saved as presets.

## What you need

- DaVinci Resolve **Studio**. The free version has no Workflow Integrations.
- macOS, or Windows (experimental).

## Install on a Mac

1. Download `DaVinci List Tool-<version>.pkg` from the latest release and open it. It is signed and
   notarized by Apple.
2. Quit and reopen Resolve.
3. **Workspace > Workflow Integrations > DaVinci List Tool**.

Install Resolve Studio first: the installer copies one file from your Resolve install so the panel
matches your Resolve version. After a major Resolve update, run the installer again if the panel
stops opening.

## Install on Windows

Download `DaVinci List Tool-<version>-Windows.zip`, unzip it, and follow the read-me inside.

## Uninstall (Mac)

Paste this into Terminal, then restart Resolve:

```
sudo rm -rf "/Library/Application Support/Blackmagic Design/DaVinci Resolve/Workflow Integration Plugins/DaVinciListTool"
```

Presets are kept in `~/.davinci-list-tool` and are not removed.

## Known limits

- An EDL cannot describe a variable-speed ramp. A retimed clip is written with its average speed.
- Grabbing marker thumbnails uses Resolve's Gallery and cleans up after itself. "Clear Gallery
  Stills" empties the whole current still album and asks first.

## Problems and requests

Open an [issue](https://github.com/Fix-It-In-Post-Tools/davinci-list-tool-releases/issues) with
your Resolve version, what you did and what you expected. A copy of the list that came out wrong
is the most useful thing you can include.

Please don't attach timelines, lists or media from a production. Describe the problem, or
reproduce it with test media.

---

DaVinci List Tool is an independent tool from Fix It In Post, LLC. It is not a Blackmagic Design
product and is not supported by Blackmagic Design. DaVinci Resolve is a trademark of Blackmagic
Design Pty Ltd. Avid is a trademark of Avid Technology, Inc.
