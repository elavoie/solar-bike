# Solar Bike

Notes for building an open hardware solar transportation vehicle.

# Constraints

* Can run at the speed of traffic on secondary roads (40-60 km/h);
* Can carry cargo;
* Require limited manufacturing skills:
  * Ideally no soldering or custom frame building;
* Use as many standard bike and solar energy components as possible;
* Can be easily assembled and disassembled in 10-15 min;
* Fits in an average appartment storage space after disassembly;
* Fits 2-4 people actively pedalling: when less than 4 people, the extra space can be replaced by carrying capacity for luggage;
* Minimize the use of short-lived components, such as batteries.

# Design Concept

## Observations

* Aerodynamism is much better in a pack of cyclists than for an individual cyclist, even if a given cyclist is not really aerodynamic: only the front of the pack need to "break the air", the rest benefit from the inertia;
* Solar power depends on the total surface of the solar panels;
* The key factor is the power/weight ratio.

Therefore the ideal solar bike would have no weight, an infinite surface of solar panels, and an infinite number of super fit people pedaling under the panels in a tight pack to minimize the frontal area.

## Principles

* Replace material with control sofware;
* Use a single bike as a basic element and combine multiple bikes/cargo cycles/etc. to create the vehicle;
* Make the design a flexible modular 'connective-tissue' between the individual bikes;
* Aim for a better power/weight ratio per cyclist than existing alternatives;
* Worry about aerodynamism and single-bike weight optimization later: if the 'connective-tissue' is flexible and modular enough, it should allow significant room for improvement without changing the basic principles (ex: accomodate replacing a cyclist with cargo and a powered wheel, use lower recumbent bikes and make the solar panels cover the cyclists also, etc.);
* Focus on designing solid and flexible interconnections for modularity.

## Practical Concept

Acronyms:
* VW: Vehicle Width
* VL: Vehicle Length
* CW: Cyclist Width
* CL: Cyclist Length

Top-Down View:

````
                    VW
           +--------------------+
              CW
           +------+

   +    +  +------+------+------+
   |    |  |      |      |      |
   |    |  |      |      |      |
   |  CL|  |  C1  |      |  C2  |
   |    |  |      |      |      |
   |    |  |      |      |      |
   |    |  |      |      |      |
   |    +  +------+      +------+
   |       |                    |
   |       |                    |
   |       |        Solar       |
   |       |        Panels      |
VL |       |                    |
   |       |                    |
   |       +------+      +------+
   |       |      |      |      |
   |       |      |      |      |
   |       |  C3  |      |  C4  |
   |       |      |      |      |
   |       |      |      |      |
   |       |      |      |      |
   +       +------+------+------+
````



# Preliminary Design

## Typical Cyclist Dimensions

* Stationary width: 0.6m 
* Essential maneuvering space width: 0.9m
* Length: 1.5-1.8m

Taken from: http://www.dot.state.mn.us/bike/pdfs/manual/Chapter3.pdf

## Vehicle constraints

* Maximum vehicle width: 2.6m (taken from truck size regulation)

Taken from: https://ops.fhwa.dot.gov/FREIGHT/publications/size_regs_final_rpt/index.htm#width

## Solar Power

* Typical Insolation: 1000W/m2
* PV solar panel efficiency: 10-20% (100-200W/m2)
* Cost: <1$US/W

## Electric Motor

* Efficiency: ?? %


## Observations

* The surface area occupied by a cyclist can be used to produce 1-2x the mechanical power of an average cyclist using solar panels and an electric motor


# Possibly Useful Components

* S-S Bicycle Torque Coupling For Quickly Assembling-Disassembling Bike Frames: http://sandsmachine.com/
* 

# Related Works

* Maxun solar bike: http://maxun.cc/solar-cycling


License: CERN OHL version 1.2
