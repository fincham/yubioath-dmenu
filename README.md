# yubioath-dmenu

Automate typing a TOTP selected using dmenu. Requires <tt>yubioath>, and <tt>xdotool</tt> if used in typing mode.

## Usage

Add a line like this to your <tt>.config/i3</tt> file:

<pre>
bindsym $mod+t exec "yubioath-dmenu --type"
</pre>

And reload i3. Now when you press <tt>$mod+t</tt> you'll be prompted to select one of your enrolled YubiKey TOTP secrets. If a touch is required a notification will indicate it, otherwise the TOTP will be typed immediately.
