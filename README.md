## Non interactive default installation on anything but Windows

<ol>
<li><tt>cd /tmp</tt> # working directory of your choice

</li><li>
Download: <tt>wget</tt> <a href="https://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz">https://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz</a>
<nobr>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;or:
<tt>curl -L -o install-tl-unx.tar.gz
    https://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz</tt>
</nobr>
<br><small>(or via whatever other method you like)</small>

</li><li><tt>zcat &lt; install-tl-unx.tar.gz | tar xf - </tt>
<tt> # note final - on that command line</tt>

</li><li><tt>cd install-tl-2*</tt>

</li><li><tt>perl ./install-tl --no-interaction  # as root or with
    <a href="#running">writable destination</a></tt>
<br><tt># may take several hours to run</tt>

</li><li>Finally, prepend <tt>/usr/local/texlive/YYYY/bin/PLATFORM</tt> to your
    PATH,<br>e.g., <tt>/usr/local/texlive/2026/bin/x86_64-linux</tt>

</li>
</ol>
