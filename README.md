# Solar Bike

Notes for building an open hardware solar transportation vehicle.

Licence: CERN Open Hardware Licence Version 1.2

# Constraints

* Can run at the speed of traffic on secondary roads (40-60 km/h);
* Can carry cargo;
* Require limited manufacturing skills:
  * Ideally no soldering or custom frame building;
* Use as many standard bike and solar energy components as possible;
* Can be easily assembled and disassembled in 10-15 min;
* Fits in an average apartment storage space after disassembly;
* Can carry multiple times disassembled copies of itself (which allows bootstrapping a delivery network with itself);
* Fits 2-4 people actively pedalling: when less than 4 people, the extra space can be replaced by carrying capacity for luggage;
* Minimize the use of short-lived components, such as batteries;
* The solar panels should be easily and quickly available for other things when the vehicle is not in use (which amortizes the cost of panels on multiple usages and enables all sorts of nomad capabilities, such as manufacturing, repair, etc.);
* Allow a sub-set of the parts to be used when a single person wants to travel shorter distances and the others do not need/want to travel with that person.

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

Solar Panel Surface: ````VW*VL - 4*(CW*CL)````

# Preliminary Design

## Typical Cyclist

### Dimensions

* Stationary width: 0.6m 
* Essential maneuvering space width: 0.9m
* Length: 1.5-1.8m

Taken from: http://www.dot.state.mn.us/bike/pdfs/manual/Chapter3.pdf

### Power

* Average Non-trained: 100W Sustained
* Average Active: 100-200W Sustained
* Elite: 400W Sustained

## Vehicle constraints

* Maximum vehicle width: 2.6m (taken from truck size regulation)

Taken from: https://ops.fhwa.dot.gov/FREIGHT/publications/size_regs_final_rpt/index.htm#width

## Solar Power

* Typical Insolation: 1000W/m2
* PV solar panel efficiency: 10-20% (100-200W/m2)
* Cost: <1$US/W

## Electric Motor

* Efficiency: >= 80 % (for [Bafang motors](http://www.bafang-e.com/en/components/component/motor/mm-g520250.html))


## Observations

* The surface area occupied by a cyclist can be used to produce 1-2x the mechanical power of an average cyclist using solar panels and an electric motor


# Possibly Useful Components

* S-S Bicycle Torque Coupling For Quickly Assembling-Disassembling Bike Frames: http://sandsmachine.com/
* Mid-drive kits from solarbike.com: [250-350W](http://solarbike.com.au/electrickits/250-350-watt-8fun-mid-drive-kits/) and [750W](http://solarbike.com.au/electrickits/750-watt-8fun-mid-drive-kit/)
* Flexible Solar Panel 18V 2.7A (48.6W), 56cmx54cmx0.2cm 1.5kg [Amazon](https://www.amazon.fr/MOHOO-Photovolta%C3%AFque-Semi-Flexible-Transformation-l%C3%A9lectricit%C3%A9-Construction/dp/B06XWCD5K6/ref=sr_1_cc_1?s=aps&ie=UTF8&qid=1516489784&sr=1-1-catcorr&keywords=sunpower+18V)
* Folding Bikes: http://enbeecycling.co.uk/bicycles/folding-bicycles/

# Related Works

* Maxun solar bike: http://maxun.cc/solar-cycling
* e-lectrike vehicles: http://e-lectrike.lu/vehicles/
* Dominic Tarr's DIY Folding Recumbent: https://www.flickr.com/photos/dominictarr/sets/72157641235154114

