# Cables & Connectors

### Cooper cables

* Shielded cooper - implemented a metail braided mesh that wrapped around the internal core wires to help protect against EMI
* Unshielded cooper

Vulnerability known as Electromagnetic Interference (EMI) - if that cable is being run too close to a very strong source of power or maybe a very strong radio source or anything magnetic then this can interfere with the signal on that cable

#### Shielded Twisted-pair (STP) Cable

* Was common in token ring networks in 1980s and 1990s, but have been replaced by Ethernet networks

#### Unshielded Twisted Pair (UTP) Cable

* Less expensive
* Lower transmission capabilities, in token ring networks the architecture itself never got faster than 16 megabits per second

UTP Categories

* Cat 1 - telephone cabelling
* Cat 2 - could carry data but only up to about 4 mb/s
* Cat 3 - could carry up to 10 mb/s and it could run a longer distance (up to 100 m)
* Cat 4 - could carry up to 16 mb/s
* Cat 5 - could carry up to 100 mb/s (Fast Ethernet)
* Cat 5e (enhanced) could carry up to 1GB/s
* Cat 6 and 6a - could also carry up to 1GB/s somewhere about 50 m range they could get 10 GB/s, 6a had a little more insulation to offer better protection against EMI
* Cat 7 - could carry 10 GB/s over 100 m, it's not yet common, but it's available

#### Coaxial (Coax) Cable

* Early LANs
* Thick Ethernet nicknamed Thick Net (10BASE5)
  * 10 reffered to the speed 10 mb/s
  * BASE refers to Baseband (signal on the cable has full access to the entire bandwidth of the cable) Transmissions verses broadband
  * 5 is up around 500 m
* Thin Ethernet (10BASE2)
  * 2 refer that it could go about twice as far as standard unshielded twisted pair in Ethernet (around 185 m)

#### Twin-axial (Twinax) Cable

* Similar to coax cable
* Use two conductors vs. one
* Cost-efficient

### Cooper Termination Standards

Wiring Standards

* TIA/EIA-568A
* TIA/EIA-568B

It's 8 cables in it, 4 are responsible for sending and 4 are receiving - you can do both at the same time in Ethernet transmission

#### Straight-through vs Crossover wiring cable

**Straight-through cable**&#x20;

* Swtich to router
* Swithc to computer
* Hub to computer

**Crossover cable**

* Switch to switch
* Switch to hub
* Hub to hub
* Router to router
* Computer to computer

### Singlemode and Multimode Fibre Cabling

**Fiber Cabling Construction**

* Cable jacket
* Strength members - strengthen the cable
* Primary coating - protect the inner components
* Cladding - is from plexiglass so it is flexible
* Core

Cabling Application Differences

* Single mode
  * Carry a single mode of light at any one time, single source and frequency
  * For long distance
* Multimode
  * Carry multiple modes of light at the same time
  * For short distance
  * Less expensive

**Source of light:**

* LED
* Light emitting diode
* Laser

**Single-mode Fiber Categories:**

* OS1(Optical Service) indoor applications - 10 km in ideal condition, (2-5 km)
* OS2  - in theory 200km

**Multimode Fiber Categories:**

* OM1 (Optical Mode) - 10 Gbps up to 33 m
* OM2 - 10 Gbps up to 82 m
* OM3 - 40 Gbps up to 300 m
* OM4 - 40 Gbps up to 550 m
* OM5 - 28 Gbps per channel over 4 channels

### Common Cable Connector Types

**Cable Connector Components:**

* Ferrule (supporting a core)
* Connector body - plastic, metal or ceramic structure that holds the ferrule
* Coupling mechanism

**Connector Types:**

* Local Connector (LC)
* Straight Tip (ST)
* Subscriber Connector (SC)
* Mechanical Transfer Registered Jack (MTRJ)

**UPC vs. APC Connectors:**

* Ultra-physical Contact (UPC)
* Angled Physical Contact (APC)

**Registered Jack (RJ) Connectors:**

* RJ11 - for telephones
* RJ45 - for UTP ethernet cabling

**F-Type Connector:**

* For coaxial cable (for TV)
* Ground to satelite links

### Common Transceiver Types

**Common types of optical transceivers:**

* Small form-factor pluggable (SFP)
* Enhanced form-factor pluggable (SFP+)
* Quad small form-factor pluggable (QSFP)
* Enhanced quad small from factor pluggable (QSFP+)

**SFP and SFP+ characteristics:**

SFP

* Upgraded version of GBIC (gigabit interface converter)
* 1/2 volume of GBIC
* Data rate from 100 Mbps to 4 Gbits/s

SFP+

* Enhanced version of SFP
* 8 Gbit/s Fibre Channel
* 10 Gigabit Ethernet and Optical Transport Network

**QSFP and QSFP+ Characteristics:**

QSFP

* 4 channels simultaneously
* 1 Gbit/s data rate per channel

QSFP+

* 4x10 Gbit/s channels
* 1x10 Gbit/s Ethernet link

### Cable Management

Patch panels:

* Cables are stripped down to their bare wire and use punchdown blocks to connect those wires and that hard wires them, on the other side would be standard RJ45 connector, then you can run cables to a switch

Cable trays:

For simply run all of the cables somewhere out of the way

* Overhead&#x20;
* Under-floor&#x20;
* Tray for data cables
* Tray for power cables

**Uninterruptible Power Supply (UPS):**

* Power backup and protection
* Can be a significant source of EMI

### Cooper Ethernet Standards

10BASE-T - supports ethernet's 10 Mbps transmission speed

100BASE-TX - CAT5 UTP straight-through cable

1000BASE-T - 1Gbps, Cat 5e

GBASE-T - data center

* 10GBASE-T Cat 6, Cat 7
* 40GBASE-T

### Fiber Ethernet Standards

100BASE-FX - 100Mbps, F stands for fiber

100BASE-SX - lower cost, uses a shorter wavelength, only travels a shorter distance, LEDs as lasers, S stands for shorter distance and L stands for longer distance

1000BASE-SX - 1Gbps, uses multimode fiber-optic cabling, 220 or 500 m depending on cable grade

1000BASE-LX - L longer distance, supports distance up to 5 km for single mode cable

10GBASE-SR - SR stands for short-range standard&#x20;

10GBASE-LR - single-mode fiber, 10 km maximum

**Coarse Wavelength Division Multiplexing:**

* Uses lower wavelength it can travel a little bit further
* Get only 18 channels

**Dense Wavelength Division Multiplexing:**

* Increases bandwidth over existing fiber networks
* Uses a higher wavelength which is more precise
* Get far more channels up to 88 channels

**Bidirectional Wavelength-division Multiplexing:**

* Used to multiplex numerous carrier signals into one optical fiber
* Performed using various wavelengths
* Bi-directional communications over a single optical cable

### Test

An ST connector would be found on which type of cabling?

* Fiber

The area of a patch panel where cable connections are hard-wired is referred to as what?

* Punchdown block

Category 5 cable could also be expressed using which cable specification?

* 100BaseTX

Which type of fiber cabling would be needed to connect two data centers that are 8 km apart?

* 10GBASE-LR

Which optical multimode fiber specification would be the minimum required to support at least 40 Gbps speeds over distances of 100 meters?

* OM3

Which transceiver would be required to support speeds of 10 Gbps over 4 channels?

* QSFP+

In which situations would a crossover cable be required?

* PC to PC
* Switch to Switch

Which categories of UTP cable are able to support speeds of at least 100 Mbps?

* 5
* 5e
