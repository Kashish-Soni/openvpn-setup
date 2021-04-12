# openvpn-setup

## Usage

First, get the script and make it executable:

```bash
curl -O https://raw.githubusercontent.com/angristan/openvpn-install/master/openvpn-install.sh
chmod +x openvpn-install.sh
```

Then run it:

```sh
./openvpn-install.sh
```

You need to run the script as root and have the TUN module enabled.

The first time you run it, you'll have to follow the assistant and answer a few questions to setup your VPN server.

Once OpenVPN is installed, you can run the script again, and you will get the choice to:

Add a client
Remove a client
Uninstall OpenVPN
In your home directory, you will have .ovpn files. These are the client configuration files. Download them from your server and connect using your favorite OpenVPN client.

- the VPN Created will have a subnet of 10.8.0.0/16 by default. Make sure to not have this subnet already occupied to avoid IP and Subnet Collissioning.
