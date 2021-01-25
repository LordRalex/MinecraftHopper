---
layout: article
title: "Fix Hosts File"
name: "fix-hosts-file"
desc: "Fix Hosts File"
---

# How to Fix Hosts File <small>(Java Only)</small>

The usage of alt account tools, such as MCLeaks, AltDispenser, Altening, etc. (which violate the EULA/ToS) have been causing issues for many Minecraft users.

When such programs are used, they make changes to a system file called 'hosts' that redirects Mojang authentication to their own servers.

As a result, users who have used alt account tools in the past will find that they either are not able to log in to the launcher or the website, or are not able to join servers. They will often get error messages such as:

<table>
  <tr>
    <td>
      <ul>
        <li>"The authentication servers are down for maintenance."</li>
        <li>"Please switch to Mojang mode."</li>
        <li>"Not authenticated with minecraft.net."</li>
      </ul>
    </td>
    <td><img src="/static/images/help/hosts-file/authentication-maintenance-error.png" height=200></td>
  </tr>
</table>

Not only do these settings prevent users from logging in or joining servers, they also function to steal the user's login information, resulting in account theft.

## Step 1: Remove the Tool

First, you will need to delete the tool. If you don't know where it is, try looking in your Downloads folder or any Minecraft folder you have on your computer.

### If You Used TheAltening
<details>
  <summary>Click to show instructions.</summary>
  
  If you used TheAltening, you need to take extra steps to remove the tool completely:
  
  <table style="margin-left:25">
    <tr>
      <td><ol><li>Press <img src="/static/images/help/hosts-file/windows-key.png" height=25> and type <strong>cmd</strong>.</li></ol></td>
      <td></td>
    </tr>
    <tr>
      <td><ol start=2><li>Right click <strong>Command Prompt</strong> and click <strong>Run as Adminstrator</strong>.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/startmenu-cmd-admin-alt.png"></td>
    </tr>
    <tr>
      <td><ol start=3><li>In the black window, type <code>taskkill /IM 'altening.launcher.exe" /F</code> and press enter. If it tells you that it could not find it, move on to the next step.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/cmd-altening-notfound.png"></td>
    </tr>
    <tr>
      <td><ol start=4><li>Press <img src="/static/images/help/hosts-file/windows-key.png" height=25> and <strong>R</strong> at the same time. Then type `%appdata%` and press enter.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/run-appdata.png"></td>
    </tr>
    <tr>
      <td><ol start=5><li>Find a folder called <strong>"Altening"</strong> and delete it.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/appdata-altening.png"></td>
    </tr>
  </table>
</details>

## Step 2: Reset Your Hosts File

You then will need to edit your hosts file to undo the changes made by the alt account tools to be able to log in to Minecraft again. Follow the instructions according to your operating system.

## Windows
<details>
  <summary>Click for instructions</summary>
  
  <table>
    <tr>
      <td><ol><li>Press <img src="/static/images/help/hosts-file/windows-key.png" height=25> and <strong>R</strong> at the same time.</li></ol></td>
      <td></td>
    </tr>
    <tr>
      <td><ol start=2><li>In the Run box, copy and paste the <strong>entire</strong> command: <code>powershell -command "Start-Process notepad $env:windir\system32\drivers\etc\hosts" -Verb runas</code></li></ol></td>
      <td><img src="/static/images/help/hosts-file/run-powershell.png"></td>
    </tr>
    <tr>
      <td><ol start=3><li>A blue window will briefly appear, then a UAC window. Click <strong>Yes</strong> in the UAC window that pops up. A Notepad window should open with text.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/win-hosts-initial.png"></td>
    </tr>
    <tr>
      <td><ol start=4><li>Look for 2 lines that contain the word "mojang" and delete those two lines completely.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/win-hosts-edited.png"></td>
    </tr>
    <tr>
      <td><ol start=5><li>Save the notepad file (make sure Notepad does not ask you where to save the file; if that happens, start over and make sure you type the whole command in #2 above).</li></ol></td>
      <td><img src="/static/images/help/hosts-file/win-hosts-save.png"></td>
    </tr>
    <tr>
      <td><ol start=6><li>Try Minecraft again. If it works now, close Notepad.</li></ol></td>
      <td></td>
    </tr>
    <tr>
      <td><ol start=7><li>Be sure to change your Minecraft password to something strong. Also change your email's password if it is the same as your Minecraft password.</li></ol></td>
      <td></td>
    </tr>
  </table>
  
  ### Alternate Method <small>(Including Windows 7 users)</small>
  
  If the above steps don't work, usually because of the UAC window not popping up in Step #3 above or Windows 7 not having Powershell, the hosts file can be restored manually.
  
  <table>
    <tr>
      <td><ol><li>Press <img src="/static/images/help/hosts-file/windows-key.png" height=25> and <strong>R</strong> at the same time.</li></ol></td>
      <td></td>
    </tr>
    <tr>
      <td><ol start=2><li>In the Run box, type <code>%systemroot%\system32\drivers\etc</code> and press Enter.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/run-etc.png"></td>
    </tr>
    <tr>
      <td><ol start=3><li>In the File Explorer window, if nothing shows up, click on <strong>View</strong> on the top, then check the bos for <strong>Show Hidden Files</strong>.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/etc.png"><br><img src="/static/images/help/hosts-file/show-hidden-files.png"></td>
    </tr>
    <tr>
      <td><ol start=4><li>Hold down <strong>Ctrl</strong> while dragging the <strong>hosts</strong> file to your desktop.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/copy-hosts-desktop.jpg"></td>
    </tr>
    <tr>
      <td><ol start=5><li>Double-click the hosts file on the desktop and open with Notepad.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/openwith-notepad.png"></td>
    </tr>
    <tr>
      <td><ol start=6><li>Look for 2 lines containing 'mojang' and delete those two lines completely. Save and close Notepad.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/win-hosts-initial.png"></td>
    </tr>
    <tr>
      <td><ol start=7><li>Look at the icon for the hosts file on your desktop. It should look like a blank sheet of paper. If it looks like a sheet of paper with lines on it, start over and be sure to follow the instructions <strong>exactly as written</strong>.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/hosts-after-saving.jpg"></td>
    </tr>
    <tr>
      <td><ol start=8><li>Drag the hosts file back into the 'etc' folder. Click <strong>Replace the file...</strong> then <strong>Continue</strong> in the windows that pop up.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/move-back-etc.jpg"><br><img src="/static/images/help/hosts-file/move-back-etc-replace.png"><br><img src="/static/images/help/hosts-file/move-back-etc-uac.png"></td>
    </tr>
    <tr>
      <td><ol start=9><li>Try Minecraft. If Minecraft now works, delete the hosts file from your desktop. Change your Minecraft password right away. Also change your email's password if it is the same as your Minecraft password.</li></ol></td>
      <td></td>
    </tr>
  </table>
</details>

## Mac
<details>
  <summary>Click for instructions</summary>
  
  <table>
    <tr>
      <td><ol><li>Open the Terminal:<br>
        <ul>
          <li>In the Finder, go to Applications > Utilities > Terminal.</li>
          <li>Or, in the Finder, press <strong>Cmd-Space</strong> to bring up Spotlight search, then type <strong>terminal</strong> and press Enter.</li>
        </ul></li></ol>
      </td>
      <td><img src="/static/images/help/hosts-file/mac-spotlight-terminal.png"></td>
    </tr>
    <tr>
      <td><ol start=2><li>In the Terminal, type <code>sudo nano /private/etc/hosts</code> and press Enter.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/mac-terminal-nano.png"></td>
    </tr>
    <tr>
      <td><ol start=3><li>You will be prompted for your password. Type in your <strong>Mac</strong> password carefully. Nothing will show up as you type your password. Press Enter when you are done.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/mac-terminal-nano-password.png"></td>
    </tr>
    <tr>
      <td><ol start=4><li>The hosts file will appear in the terminal. Use the arrow keys to navigate the file.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/mac-terminal-hosts-open.png"></td>
    </tr>
    <tr>
      <td><ol start=5><li>Go down to the bottom of the file. There should be 2 lines containing "mojang."</li></ol></td>
      <td></td>
    </tr>
    <tr>
      <td><ol start=6><li>Using the arrow keys and the Backspace key, delete those two lines entirely.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/mac-terminal-hosts-edited.png"></td>
    </tr>
    <tr>
  <td><ol start=7><li>Press <strong>Ctrl-O</strong> (not Cmd-O) then <strong>Enter</strong> to save the file. Leave the window open then try Minecraft again. If Minecraft is still open, close and reopen it.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/mac-terminal-hosts-save.png"></td>
    </tr>
    <tr>
      <td><ol start=8><li>If Minecraft works, close the Terminal window and change your Minecraft password right away. Also change your email's password if it is the same as your Minecraft password.</li></ol></td>
      <td></td>
    </tr>
  </table>
</details>

## Linux
<details>
  <summary>Click for instructions</summary>
  
  <table>
    <tr>
      <td><ol><li>Open the Terminal:<br>
        <ul>
          <li><i>Ubuntu</i>: Press Ctrl + Alt + T</li>
          <li><i>Other Debian</i>: Open the start menu and type 'terminal' in the search bar, then click on Terminal</li>
          <li><i>Arch</i>: </li>
        </ul></li></ol>
      </td>
      <td><img src="/static/images/help/hosts-file/linux-deb-terminal.png"></td>
    </tr>
    <tr>
      <td><ol start=2><li>In the terminal, type <code>sudo nano /etc/hosts</code> and press Enter.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/linux-terminal-nano.png"></td>
    </tr>
    <tr>
      <td><ol start=3><li>You will be prompted for your password. Type in your <strong>Linux user</strong> password carefully. Nothing will show up as you type your password. Press Enter when you are done.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/linux-terminal-nano-password.jpg"></td>
    </tr>
    <tr>
      <td><ol start=4><li>The hosts file will appear in the terminal. Use the arrow keys to navigate the file.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/linux-nano-open.jpg"></td>
    </tr>
    <tr>
      <td><ol start=5><li>Go down to the bottom of the file. There should be 2 lines containing "mojang."</li></ol></td>
      <td></td>
    </tr>
    <tr>
      <td><ol start=6><li>Using the arrow keys and the Backspace key, delete those two lines entirely.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/linux-nano-edited.jpg"></td>
    </tr>
    <tr>
      <td><ol start=7><li>Press <strong>Ctrl-O</strong> then <strong>Enter</strong> to save the file. Leave the window open then try Minecraft again. If Minecraft is still open, close and reopen it.</li></ol></td>
      <td><img src="/static/images/help/hosts-file/linux-nano-save.jpg"></td>
    </tr>
    <tr>
      <td><ol start=8><li>If Minecraft works, close the Terminal window and change your Minecraft password right away. Also change your email's password if it is the same as your Minecraft password.</li></ol></td>
      <td></td>
    </tr>
  </table>
</details>
