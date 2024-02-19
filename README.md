---


---

<h1 id="node-running-guide-dusk-itn">Node Running Guide Dusk ITN</h1>
<h1 id="membuat-wallet">Membuat Wallet</h1>
<p>➖ Buat New Wallet : <a href="https://wallet.dusk.network/setup/">https://wallet.dusk.network/setup/</a><br>
➖ Back Up Pharse dan Masukan Lagi (Backup)<br>
➖ Next Next Aja dan Copy Address<br>
➖ Claim Faucet : <a href="https://t.me/bangpateng_airdrop/49158">https://t.me/bangpateng_airdrop/49158</a></p>
<h2 id="openport">OpenPort</h2>
<blockquote>
<pre><code>sudo ufw allow 22 
sudo ufw allow 8080/tcp 
sudo ufw allow 9000:9005/udp
sudo ufw enable
</code></pre>
</blockquote>
<h2 id="install-github">Install Github</h2>
<blockquote>
<p><code></code>curl --proto ‘=https’ --tlsv1.2 -sSfL <a href="https://github.com/dusk-network/itn-installer/releases/download/v0.1.0/itn-installer.sh">https://github.com/dusk-network/itn-installer/releases/download/v0.1.0/itn-installer.sh</a> | sudo sh</p>code></p>
</blockquote>
<h2 id="import-pharse-wallet">Import Pharse Wallet</h2>
<blockquote>
<p>rusk-wallet restore</p>
</blockquote>
<p>Paste Pharse Kalian (Pastikan Huruf Kecil Semua)<br>
Masukan Password Bebas 2x</p>
<h2 id="jalankan-kode-di-bawah">Jalankan Kode di Bawah</h2>
<blockquote>
<p>rusk-wallet export -d /opt/dusk/conf -n consensus.keys</p>
</blockquote>
<p>Masukan Password Lagi 2x</p>
<blockquote>
<p>sh /opt/dusk/bin/setup_consensus_pwd.sh</p>
</blockquote>
<p>Masukan Password Lagi Samain Aja</p>
<h2 id="start-node">Start Node</h2>
<blockquote>
<p>service rusk start</p>
</blockquote>
<h1 id="check-log-node">Check Log Node</h1>
<blockquote>
<p>grep “block accepted” /var/log/rusk.log</p>
</blockquote>
<p>atau</p>
<blockquote>
<p>tail -f /var/log/rusk.log</p>
</blockquote>
<h2 id="check-wallet">Check Wallet</h2>
<blockquote>
<p>rusk-wallet</p>
</blockquote>
<p>➖ Pilih Acces Your Wallet dan Enter<br>
➖ Masukan Password (Pastikan Address Kalian Sama Dengan Yang di Website)<br>
➖ Gunakan Arah Atas Bawa Untuk Pindah Menu dan Enter Untuk Eksekusi</p>
