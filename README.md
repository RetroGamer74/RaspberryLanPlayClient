# Raspberry Super Lan Play Client

This client is based on command line. Command line is the best approach for a device like raspberry.

First off all, install the required libraries using next command:

```
sudo apt install libpcap0.8-dev libuv1-dev
```

Once finished download from this repository lan-play binary and give execution permissions using next command:

```
chmod 755 lan-play
```

You're ready to go. Start the program with sudo to get permissions to use the libraries. Use the --relay-server-addr parameter with one of our servers, depending on you want to play switch or PS4. You will get a list of your network interfaces. Choose the right one in your case. You have to choose the one connected to internet.

So for switch it should be:

```
sudo ./lan-play --relay-server-addr lanplay.retrogamer.tech:11451
```

If you want to play PS4 it should be:

```
sudo ./lan-play --relay-server-addr lanplayps.retrogamer.tech:11451
```

# Credits

This lan-play client has been built for Raspberry based on @imspace original source code for lan-play.

https://github.com/spacemeowx2/switch-lan-play

