# HAA-IR-Toolkit
Tool to decode HAA IR Captured packets

[![Donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](https://paypal.me/RavenSystem)

The tool helps you decoding captured HAA IR packets into a 2, 4 or 6 bit HAA protocol and protocol command.
URL: https://ravensystem.github.io/haairtoolkit

For example, if we use the HAA IR packets capture below (for a Daikin AC), the tool will analize the packets and identify:

- The protocol bits used in the capture, e.g. ["420-1740","420-660","420-29330","5120-2100"] - 4 bits protocol
- The protocol bits string, e.g.
30111011110100100000101111110011111011111111111111000011123011101111010010000010111111001111111111100110101111111110111101111111111111111111101011110010011111111111111101111100000 - 179 bits
- The HAA IR protocol command: e.g. aCaDaAbAeAaFbEaMAdCnNaCaDaAbAeAaFbKbBaAaIaDaMGaAaDbAbMBaEe
- The HAA IR Protocol: e.g. LbEEAADPAAAwAA(4LbEEAA

The tool will show you accumulated values the bits, protocol command and protocol.
You could for example capture 5 samples, and decode all of them. You can the use a capture where the values matches others.

The HAA IR protocol command and protocol values are used in HAA JSON configuration string.

Sample HAA IR Packet capture:
+ 5119 - 2104 +  414 - 1744 +  416 -  663 +  416 -  664 +  415 -  665 +  414 - 1744 +  415 -  664 +  415 -  664 
+  415 -  664 +  415 -  665 +  414 - 1744 +  416 -  665 +  413 - 1744 +  415 - 1743 +  416 -  672 +  407 - 1743 
+  415 - 1744 +  415 - 1743 +  415 - 1744 +  415 - 1744 +  414 -  664 +  416 - 1743 +  415 -  665 +  414 -  664 
+  415 -  665 +  415 -  664 +  414 -  666 +  414 -  665 +  415 - 1743 +  414 - 1744 +  415 -  665 +  415 -  664 
+  415 -  666 +  413 -  665 +  414 -  665 +  415 - 1743 +  416 -  664 +  414 -  665 +  414 -  665 +  415 -  665 
+  414 -  665 +  414 -  666 +  414 -  665 +  414 -  665 +  414 -  665 +  414 -  665 +  414 -  666 +  414 -  665 
+  414 -  665 +  414 -  667 +  412 - 1745 +  414 - 1744 +  415 - 1744 +  414 - 1745 +  414 -  665 +  414 -  665 
+  414 -  665 +  414 -29328 + 5122 - 2101 +  417 - 1742 +  416 -  663 +  475 -  604 +  417 -  663 +  416 - 1742 
+  417 -  662 +  417 -  663 +  416 -  662 +  418 -  662 +  416 - 1743 +  416 -  663 +  417 - 1741 +  417 - 1742 
+  416 -  663 +  417 - 1741 +  417 - 1742 +  417 - 1742 +  416 - 1742 +  417 - 1742 +  416 -  663 +  417 - 1741 
+  418 -  662 +  416 -  663 +  417 -  663 +  416 -  663 +  416 -  663 +  417 -  662 +  416 - 1743 +  416 - 1742 
+  417 -  663 +  415 -  664 +  417 -  662 +  417 -  662 +  417 -  662 +  418 -  662 +  416 -  663 +  496 -  583 
+  417 -  663 +  416 -  662 +  418 -  662 +  417 - 1742 +  417 - 1740 +  418 -  663 +  416 -  663 +  416 - 1742 
+  417 -  663 +  416 - 1742 +  417 -  662 +  417 -  663 +  416 -  663 +  440 -  639 +  417 -  662 +  417 -  662 
+  417 -  663 +  416 -  664 +  416 -  662 +  417 - 1741 +  417 -  663 +  417 -  662 +  417 -  662 +  417 -  663 
+  416 - 1742 +  417 -  663 +  416 -  663 +  417 -  662 +  417 -  662 +  417 -  662 +  418 -  662 +  417 -  662 
+  417 -  662 +  418 -  662 +  416 -  663 +  417 -  662 +  417 -  663 +  416 -  662 +  418 -  662 +  417 -  745 
+  334 -  663 +  416 -  663 +  416 -  663 +  417 -  662 +  417 -  662 +  418 - 1741 +  417 -  663 +  416 - 1742 
+  417 -  663 +  416 -  662 +  417 -  662 +  418 -  662 +  417 - 1741 +  417 - 1742 +  417 -  662 +  417 - 1742 
+  417 - 1741 +  418 -  661 +  417 -  663 +  417 -  662 +  417 -  663 +  417 -  662 +  417 -  662 +  417 -  663 
+  416 -  663 +  417 -  662 +  416 -  664 +  416 -  662 +  417 -  663 +  417 -  662 +  417 -  662 +  418 -  661 
+  417 - 1742 +  417 -  662 +  417 -  663 +  416 -  662 +  418 -  662 +  417 -  662 +  417 - 1742 +  418 - 1740 
+  417 - 1742 +  417 - 1741 +  419 - 1739 +  418 

Original source: https://github.com/GarzaCon/HAA-IR-Toolkit
