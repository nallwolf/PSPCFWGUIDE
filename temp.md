   <div id="readme" class="Box-body readme blob js-code-block-container p-5 p-xl-6">
    <article class="markdown-body entry-content container-lg" itemprop="text"><h1><a id="user-content-lineageos-160-builds-for-the-nintendo-switch" class="anchor" aria-hidden="true" href="#lineageos-160-builds-for-the-nintendo-switch"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>LineageOS 16.0 builds for the Nintendo Switch</h1>
<p><strong>Installation instructions based on</strong> <a href="https://gitlab.com/ZachyCatGames/shitty-pie-guide" rel="nofollow">https://gitlab.com/ZachyCatGames/shitty-pie-guide</a></p>
<p>Download the build .zip, the boot.img and tegra210-icosa.dts files from the lastest release.</p>
<p>Download hekate and extract it on the root of your SD card.</p>
<p>Put <a href="https://gitlab.com/ZachyCatGames/shitty-pie-guide/-/raw/master/00-android.ini?inline=false" rel="nofollow">https://gitlab.com/ZachyCatGames/shitty-pie-guide/-/raw/master/00-android.ini?inline=false</a> in <code>/bootloader/ini</code> on the SD card. <strong>If it downloads as a .txt rename it to .ini</strong></p>
<p>Put these in <code>/switchroot/android/</code> on the SD card:
<a href="https://cdn.discordapp.com/attachments/667093920005619742/702602200991662210/coreboot.rom" rel="nofollow">https://cdn.discordapp.com/attachments/667093920005619742/702602200991662210/coreboot.rom</a><br>
<a href="https://gitlab.com/switchroot/bootstack/switch-uboot-scripts/-/jobs/artifacts/master/raw/common.scr?job=build" rel="nofollow">https://gitlab.com/switchroot/bootstack/switch-uboot-scripts/-/jobs/artifacts/master/raw/common.scr?job=build</a><br>
<a href="https://gitlab.com/switchroot/bootstack/switch-uboot-scripts/-/jobs/artifacts/master/raw/sd.scr?job=build" rel="nofollow">https://gitlab.com/switchroot/bootstack/switch-uboot-scripts/-/jobs/artifacts/master/raw/sd.scr?job=build</a><br>
and rename sd.scr to boot.scr.</p>
<p>Copy <code>boot.img</code> and <code>tegra210-icosa.dtb</code> to <code>/switchroot/install</code> on the SD card.</p>
<p>Copy <code>lineage-16.0-[date]-UNOFFICIAL-[device name].zip</code> to the root of the SD card.</p>
<p>Download <a href="https://drive.google.com/open?id=1KUaQThm6S2xYPYD98qxZsb4JPeRJAM5K" rel="nofollow">https://drive.google.com/open?id=1KUaQThm6S2xYPYD98qxZsb4JPeRJAM5K</a> &amp; extract <code>twrp.img</code> to <code>/switchroot/install</code> on the SD card.</p>
<p>Launch Hekate as for Pie you need to dump your joycon BT info in Nyx -&gt; Nyx options (Ctcaer credit). Connect your joycon before you dump them. Then navigate to <code>Tools</code> -&gt; <code>Arch bit • RCM • Touch • Partitions</code> -&gt; <code>Partition SD Card</code>.</p>
<p>You can use the <code>Android </code> slider to choose how much storage you want Android to have access too, then press <code>Next Step</code>, then <code>Start</code>.</p>
<p>Once that finishes press <code>Flash Android</code>, then <code>Continue</code>.</p>
<p>Press <code>Continue</code> again and it should reboot to TWRP.</p>
<p>In TWRP tap mount, then check every partition.</p>
<p>Now go back and press <code>Install</code> then navigate to <code>external_sd</code> then to wherever you put <code>lineage-16.0-[date]-UNOFFICIAL-[device name].zip</code> and tap on it.</p>
<p>Swipe to confirm and it should install the rest of Android.</p>
<p>Now just reboot, load hekate again, select the config, and hope it boots</p>
</article>
  </div>
