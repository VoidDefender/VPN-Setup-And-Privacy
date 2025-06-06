# VPN Setup Steps (ProtonVPN on Kali Linux)

## Step 1: Install Required Dependencies

    sudo apt update  
    sudo apt install -y openvpn dialog python3-pip python3-setuptools

---

## Step 2: Install ProtonVPN CLI

    pip3 install protonvpn-cli

---

## Step 3: Initialize ProtonVPN

    protonvpn init

You will be prompted to:

    - Enter your ProtonVPN credentials
    - Select OpenVPN
    - Configure DNS and autoconnect options

---

## Step 4: Connect to VPN

    protonvpn c --sc

Output:

    Connecting to: Netherlands-FREE#21  
    VPN connection successfully established.

---

## Step 5: Check VPN Status

    protonvpn s

Output:

    Connected to Netherlands-FREE#21  
    Public IP: 185.159.157.5  
    Protocol: OpenVPN

---

## Step 6: Disconnect VPN

    protonvpn d
