# ESPHome Minisplit Configuration

This contains the configuration for control of minisplits in ESPHome using the [Smartlight SLWF-01PRO](https://smartlight.me/smart-home-devices/wifi-devices/wifi-dongle-air-conditioners-midea-idea-electrolux-for-home-assistant) board.

You can [get the Smartlight SLWF-01PRO from cloudfree.shop](https://cloudfree.shop/product/ductless-hvac-wi-fi-module/) for about $15 bucks shipped in the USA, or it appears that [there are counterfeit clones on Amazon](https://amazon.com/dp/B0F149XVS1?tag=amz-link-20). However, since the board was originally designed by Smartlight (a small business based in the Ukraine), buying their official product would be a great way to support small businesses and the ESPHome community.

- `yitahome.yaml` works with Yitahome brand mini split units which are rebranded unit produced by Aux. Yitahome appears to sell multiple different units; this has been verified on both the [220v 21 SEER 1.5 ton unit (SKU 5242)](https://www.yitahome.com/products/18000-btu-15-ton-21-seer2-ductless-mini-split-air-conditioner-heating-and-cooling-kit-p-5242.html) and the [220v 21 SEER 1 ton unit (SKU 5244)](https://www.yitahome.com/products/12000-btu-1-ton-21-seer2-ductless-mini-split-air-conditioner-heating-and-cooling-kit-p-5244.html). Other units purchased from Yitahome may be manufactured elsewhere and require a different configuration.

- `pioneer.yaml` works with Pioneer brand mini splits which are rebranded units produced by Midea

Additionally, pre-compiled versions of the above configurations are included which provide a configuration wifi access point called "minisplit-XXXXX" with no password. Once you load the .bin file onto your SLWF-01PRO board and install it in your minisplit, just connect to the new wifi network and visit http://192.168.4.1 in your browser to specify your wifi network credentials.

- `aux-yitahome.bin` works with all Aux minisplits, including Yitahome's rebranded Aux units

- `midea-pioneer.bin` works with all Midea minisplits, including Pioneer's rebranded Midea units