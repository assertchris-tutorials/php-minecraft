# Looking for code in all the wrong places

These are the slides and the code for my #SCD18 talk. 

## Getting started

1. Buy and download a legal version of Minecraft.
2. Copy the contents of `minecraft-client` to your `Application Support` or `%appdata%` Minecraft folder. It's ok to overwrite the contents there - there's nothing reinstalling that legal version of Minecraft can't fix, if anything is messed up.
3. Launch Minecraft, and run the "forge" version.
4. Make sure the Sphax PureBDCraft and "slides" resource packs are enabled.
5. Launch the "forge" minecraft server, found in `minecraft-server`. You can launch it with `java -Xmx2024M -Xms2024M -jar forge-1.12.2-14.23.2.2611-universal.jar`.
6. Wait until the server has finished loading, and you see the "RCON" listening/connected log message.
7. Launch the PHP daemon, found in `php-daemon`. You can launch it with `php index.php`.

> The PHP daemon will attempt to connect to the dedicated "forge" server. If it can't connect, you will see an ugly error message. Some commands also depend on a running Shopware v5.4.* application, running at `http://127.0.0.1:8080`. If that is not set up correctly, some of the custom commands will fail.

8. Connect to the "forge" dedicated server, from the Minecraft client. An address of `127.0.0.1` should suffice.
9. If all resource packs are correctly configured, and you're running the "forge" versions of the Minecraft client and server; then you should be able to see the "slides" from the talk. If the PHP daemon is working, and the Shopware instance is working; then you should also be able to run the custom commands.

## Custom commands

1. `!ping` - this checks that hte daemon is running, you should see "pong"
2. `!email your@email.com` - this sets the email associated with your Minecraft username
3. `!shop` - this opens the shop door, if you have set your email
4. `!refresh` - this loads the 4 most recently updated Shopware articles (from that local isntance), onto the signs in the shop

## Help

There are a lot of moving parts to this. If you have trouble setting things up, [ask me for help](https://twitter.com/assertchris).
