 
<!--- the previous line with a space is needed for github pages
      the title is not needed here, as it is taken from the project description in Github 
--->

In this project, we developed a solution for end-to-end delay monitoring of SRv6 based services.
The proposed solution leverages the Simple Two-way Active Measurement Protocol (STAMP) and its extensions to monitor the
delay of an SRv6 path between two measurement nodes, called STAMP Session-Sender and Session-Reflector.

The measurement architecture also includes an SDN controller, as shown in the following figure.

![stamp-reference-scenario-web-page.png](<./images/stamp-reference-scenario-web-page.png>)

We first implemented the STAMP Session-Sender and STAMP Session-Reflector with a user space application based on Scapy, then we developed an eBPF version.

The delay monitoring solution has been integrated in the EveryWAN architecture for SRv6 based SD-WANs.

We have assessed the packet processing performance of our delay monitoring solution.

### Walkthrough

Walkthrough for delay monitoring with EveryWAN 
https://docs.google.com/document/d/1-yNLrOOyxbPK_pSDFfqv5Xzzf1Ligm2lGMQVLapeql4

Walkthrough for SRv6 STAMP delay monitoring experiments (performance assessment)
https://docs.google.com/document/d/1bG24Ja-Xr11BtYydMI2yrMxpP5aZ18DXBdf3LTek-b0


### Source code

- User space implementation of STAMP Session-Sender, STAMP Session-Reflector and SDN controller : https://github.com/everywan-io/srv6pm-delay-measurement
- eBPF based implementation of STAMP Session-Sender, STAMP Session-Reflector : https://github.com/netgroup/hikepkg-stamp

### Scientific papers

- C. Scarpitta, G. Sidoretti, A. Mayer, S. Salsano, A. Abdelsalam, C. Filsfils, <br>
"[High Performance Delay Monitoring\\for SRv6 Based SD-WANs]()", <br>
Submitted paper, December 2022

<!--- example of figure
      always put the link to the img source (e.g. gslide):
      https://docs.google.com/presentation/d/1rV0ViQYk9lYUnJH16zvf5qBDUK4yTWAeHoryo6Fe0jo/edit#slide=id.g7f4100c2bd_6_0 
      export the slide as .png, and upload in docs/images with the same name
![example.png](<./images/example.png>)
     
--->
