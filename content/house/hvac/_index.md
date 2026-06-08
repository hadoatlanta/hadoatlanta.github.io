+++
date = '2025-03-06T08:32:55-05:00'
draft = false
title = 'House'
+++

## HVAC

| Detail                     |    Location     |
| :------------------------- | :-------------: |
| Furnace Lennox EL180       | 1900 Federal CT |
| Furnace Lennox GS18Q3-75-5 | 1900 Federal CT |
| Ducati                     | 191 Murphy Ave  |

## Capacitor

| Detail                    |           Location            |
| :------------------------ | :---------------------------: |
| RHdeem - 45+5             |        191 Murphy Ave         |
| Lennox - 35+5             |        1900 Federal CT        |
| Blower Unit - 7.5         |        191 Murphy Ave         |
| Blower Unit - 7.5         | 1900 Federal CT - Crawl space |
| Dual Capacitor(12) - 35+5 |         May 19, 2026          |


## Air Filter

| Furnace            |        Size | Replacement Date |    Location     |
| :----------------- | ----------: | ---------------: | :-------------: |
| Lennox EL180       | 16 x 25 x 1 |     20 Dec, 2025 | 1900 Federal CT |
| Lennox GS18Q3-75-5 | 14 x 18 x 1 |     20 Dec, 2025 | 1900 Federal CT |
| Ducati             | 20 x 25 x 1 |     20 Dec, 2025 | 191 Murphy Ave  |

## Water Heater

| Detail                |    Location     |     Flush      |
| :-------------------- | :-------------: | :------------: |
| Electric Water Heater | 1900 Federal CT | April 26, 2026 |
| Ducati                | 191 Murphy Ave  |                |

## Kid DIY workshop

1. Lowe - Third Saturday of Month
   1. https://www.lowes.com/diy-projects-and-ideas/workshops
2. Homedepot - First Saturday of Month
   1. https://www.homedepot.com/c/kids-workshop

## Brother Printer HL-L2390DW

You are going to install following packages.
   hll2390dwpdrv-4.0.0-1.i386.deb
   brscan4-0.4.11-1.amd64.deb
   brscan-skey-0.3.4-0.amd64.deb

wget -T 10 -nd --no-cache https://download.brother.com/pub/com/linux/linux/packages/hll2390dwpdrv-4.0.0-1.i386.deb

dpkg -x hll2390dwpdrv-4.0.0-1.i386.deb /
dpkg-deb: building package 'hll2390dwpdrv' in 'hll2390dwpdrv-4.0.0-1a.i386.deb'.
dpkg -b ./brother_driver_packdir hll2390dwpdrv-4.0.0-1a.i386.deb
dpkg -i --force-all hll2390dwpdrv-4.0.0-1a.i386.deb

hll2390dwpdrv
Will you specify the Device URI? [Y/n] ->Y

0: hp
1: cups-brf:/
2: socket
3: beh
4: ipp
5: http
6: ipps
7: https
8: lpd
9: hpfax
10: dnssd://Brother%20HL-L2390DW._ipp._tcp.local/?uuid=e3248000-80ce-11db-8000-30c9ab1860e8
11: ipp://Brother%20HL-L2390DW._ipp._tcp.local/
12: lpd://BRW30C9AB1860E8/BINARY_P1
13: dnssd://Brother%20HL-L2390DW._printer._tcp.local/?uuid=e3248000-80ce-11db-8000-30c9ab1860e8
14 (I): Specify IP address.
15 (A): Auto. (dnssd://Brother%20HL-L2390DW._ipp._tcp.local/?uuid=e3248000-80ce-11db-8000-30c9ab1860e8)

select the number of destination Device URI. ->10.0.0.116

You are going to install following packages.
   brscan4-0.4.11-1.amd64.deb

wget -T 10 -nd --no-cache https://download.brother.com/pub/com/linux/linux/packages/brscan4-0.4.11-1.amd64.deb

dpkg -i --force-all brscan4-0.4.11-1.amd64.deb

wget -T 10 -nd --no-cache https://download.brother.com/pub/com/linux/linux/packages/brscan-skey-0.3.4-0.amd64.deb

dpkg -i --force-all brscan-skey-0.3.4-0.amd64.deb
Processing triggers for libc-bin (2.35-0ubuntu3.13) ...
 enter IP address ->10.0.0.116

brsaneconfig4 -a name=HL-L2390DW model=HL-L2390DW ip=10.0.0.116
Hit Enter/Return key.

### How to use Brother Scanner

1. Check Borther Scanner on a computer
2. All scanned files store in /home/hadn/brscan.

#### Step to Scan

1. Place a document on scanner.
2. Press Scan Button.
3. Select Scan to PC.
4. Press Ok Button.
5. Select ***Files***.
6. Press Ok Button.
7. Press ***Start*** Button.
8. Press minus***(-)*** Button to send file to PC.