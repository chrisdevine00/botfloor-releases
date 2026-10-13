# Botfloor

A small robot on your Mac's desktop for each Claude Code session. Each robot shows its project and what it's doing, hops when it needs your approval, and tells you when it's done.

Requires macOS 14 or later (Apple silicon or Intel) and [Claude Code](https://claude.com/claude-code).

## Install

1. **[Download the latest version](https://github.com/chrisdevine00/botfloor-releases/releases/latest)**: get `Botfloor-<version>.dmg` under Assets.
2. Open the DMG and drag **Botfloor** to **Applications**, then open it.
3. Click **Connect Claude Code** in the welcome window, then restart any Claude Code sessions that are already open.

Drag a robot to move them, double-click one to rebuild it, and right-click for everything else. Botfloor updates itself from this page.

## Remove

1. Right-click a robot and choose **Disconnect Claude Code**.
2. Quit Botfloor and move it to the Trash.
3. Optional: delete what it left behind:

   ```bash
   rm -rf ~/.botfloor ~/Library/Caches/com.imovepixels.botfloor
   defaults delete com.imovepixels.botfloor
   ```

## Privacy

Botfloor keeps project names, session status, and short summaries of prompts and replies in `~/.botfloor`, readable only by your account. Nothing leaves your Mac. Its only network requests are update checks to this repo.
