# Half-Wavelength Dipole for 80m in NVIS Configuration

<p align="center">
<img src="./img/main_picture.jpg" width="500" height="600"/>
</p>

## Introduction
This article summarizes my experiences with building 80m half-wave dipol in NVIS setup.
The main goal of this project was to evaluate how practical is to install dipol antenna as low as 1m above the ground. 
I wanted to test in particular:

- quality of regional coverage (range of 0 to 500km)

- tunning ease

## Design
To build the anntenna I used 4mm2 insulated wire (Lgy4). Rough estimation of dimensions can be found using below formula:

$L_{\text{antenna total length}} = K \cdot \frac{c}{2f}$

where:

K- is shortening factor (K=1 for free space, K=0.9-0.95 for insulated wire antenna setup near the ground)

c - speed of light in free space in m/s (299 792 458 m/s)

f - frequency in Hertz

Assuming K = 0.95:

$L_{\text{antenna total length}} \approx 39m$

so each radiating element length will be:

$l = \frac{L_{\text{antenna total length}}}{2} = 19,5m$

To be on the safe side I used 2 x 20m wires, those dimentions produced SWR minimum slightly below 3.5MHz. Duirng antenna tunning antenna length was reduced (i.e. the length of both radiating elements was reduced by the same amount until SWR lowest point moved to desired frequency - in my case I have chosen 3.7MHz to optimize the setup for phone communication).

It shall be noted that electrical dimensions of the half-wave dipol antenna are shorter if radiating elements are mounted low from the ground. When antenna is elevated its dimensions need to increse to keep SWR minimum at the same frequency.

Photos of the antenna mounting can be seen below:

<p align="center">
<img src="./img/feed_point.jpg" width="400" height="500"/>
<img src="./img/end1.jpg" width="400" height="500"/>
<img src="./img/end2.jpg" width="400" height="500"/>
</p>

## Tunning

Tunning of the antenna was very simple. It was enough to reduce antenna length by about a meter at each end to achieve SWR minimum of 1.8 at 3.7Mhz. At both ends of the band SWR did not exceed 3, which meant that in practice no antenna tunner was required to operate the setup.

<p align="center">
<img src="./img/swr_f0.jpg" width="400" height="500"/>
<img src="./img/swrf0_max.jpg" width="400" height="500"/>
<img src="./img/swr_ll.jpg" width="400" height="500"/>
<img src="./img/swr_rr.jpg" width="400" height="500"/>
</p>

## Coverage Performance

It was possible to establish QSOs with entire Poland starting with stations located just a few kilometers away. The longest QSO was made with station from Bulgaria.

More tests will be carried out to confirm antenna performance especially when it comes to close proximity communication.

# Summary

In summary, I was positively surprised that so low mounted antenna can deliver solid regional coverage. Reports received were always above 57 (I was transmitting with 30-100W power using FT-710 in LSB mode).

## References
[1] Understanding NVIS - Rhode-Schwarz

[2] The NVIS— A Low Antenna for Regional  Communications - Albert L. Pion, KK7XO, QST June 2002

[3] A Look at NVIS Techniques - Ed Farmer, AA6ZM - QST January 1995