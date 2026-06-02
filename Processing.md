#polymers


## Batch Processing Techniques
- [[Compression Molding]] - Used in [[Thermoset]] plastics and a few [[Thermoplastics]]
- [[Injection molding]] - at low volume, its batch
- [[Reaction Injection Molding]] - injection molding but there's a reaction
- [[Resin Transfer Molding]] - Resin injected into a mold containing reinforcement fibers, handlayup is the manual, open mold way of doing this
- [[Rotational Molding]] - rotational figures
- [[Casting]] - first thing that comes to mind
## Continuous Processing Techniques
- [[Processing#Extrusion]] - extrusion, I've written a good deal on this below
- [[Blow Molding]] - used to make hollow parts
- [[Calendaring]] - extrusion but for films
- [[Thermoforming]] - heated sheets stretched over a mold
- [[Pultrusion]] - Fibers pulled through a resin bath to form composites
# Stuff I wrote before
* You process a polymer at it's processing temperature. In case of polymers the processing temperature is above it's melting temperature
* To reduce the resistance of the material, you need to increase the temperature above the melt temperature to reduce viscosity. Generally about 10C higher than melting point
* Polymer processing is done for application, study of properties and to reduce the cost of a compound by adding a filler or use a cheaper material along with the polymer
* First part of processing is called dry blending then melt blending. Not strictly a requirement
## Blending them
* Dry blending -  You don't allow the polymer to melt when processing. Example - you have one powder phase and one pellet/granular phase and they're just mixed up. Can't be regularly agitated since the powder will separate from the granules due to difference in density. ==Oily phase to be added to the mixture so the powder is tied to the granules. The oily phase is called a wetting agent and that causes adsorption/ soaking of the powder on the granule.==
* The granules are added then wetting agent then powder at the end. The wetting agent isn't added in the end because this would cause the powder to be clumped up together
* When you're mixing in a tumbler, the rpm you choose is important. The optimized speed is a problem. The RPM where you're getting a constant bulk density is the optimum speed
* ![[Pasted image 20240802100231.png]]
* To know when something is properly mixed you sample and check the bulk density. The bulk density is measured using a British cylinder
* Melt blending - Melt 'n Mix after making a uniform dry blend as written above. It's not mandatory all the time to have dry then melt processing, you can go directly to melt by using feeders. 
## Extrusion
* Extrusion is a continuous output with positive displacement.
* A cycle air pump is not an extruder since it retracts and this it is not continuous
* A screw is used to extrude polymer to have a continuous positive displacement
* ![[Pasted image 20240802100254.png]]
* To increase the mixing, you must reduce the distance between the screw and the barrel. This has the consequence of reducing the mass flow
* Should the shear profile be constant or profile(non constant) through the extrusion? It shouldn't because it wouldnt be mixed properly if it was
* You mostly use thermoplastic in an extruder
* Screw has 3 zones - feed zone, compression/transition zone and the metering zone(?)
* Screw will be tapered (thicker toward the end)
* feed zone you're feeding the material from the hopper. It's only there to convey the material
* Compression zone is for intensive shear mixing of the polymer to be extruded
* metering zone is to push the mixed polymer through a die (the stuff that extrudes it)
* L/D ratio of the screw is the ratio of the screw groove diameter to the length of the screw
* the clearance of the screw is different at different zones. Feed zone the clearance is high. end of the compression zone the clearance is low and the metering zone it's constant at low. Clearance is the distance between the end of the grove of the screw and the wall of the extruder
>[!todo]
>understand how the clearance changes between different parts and why. Actually just study all of extrusion from somewhere

* compression ratio:
* $$compression \space ratio = \frac{clearance_{feed}}{clearance_{metering}}$$
* RPM of the screw cant vary
* Temperature will not be constant throughout, the temperature at the feed zone is less and the temperature as you go ahead increases to slowly melt and mix and extrude it
* If the temperature at the feed zone is high, the extruder will get clogged as the stuff will stick to the screw when it melts
> Extrusion is a positive displacement technique. Considered to be an adiabatic technique and every zone is isothermal (the temperature doesn't variably change, it is fixed at the melt temperature at non feed zones). Metering zone has screen plate (mesh) and breaker plate(supports the screen plate) right before the die. The screen plate is to restrict unmelted polymer. Breaker plate converts turbulent to laminar flow. 
* There are three types of flows in an extruder - the drag flow (dragged by the screw), pressure flow (pressure from the screen and breaker plate, causing backflow, better mixing) and leakage flow (clearance leakage)
 >[!danger]
>compression ratio has nothing to do with actual pressure - it's just a metric for mixing
## Twin screw
* Single motor, two screws, parallel, no tapered design. Screws both move clockwise, there will be pressure buildup since the screws are different directionally threaded (co-rotating). Co rotating has a bad shear profile but good mixing
* It also be non - corotating - counter rotating. The screws both move in different directions and the mixture flows in an infinite symbol shape. counter rotating has a better shear profile but bad mixing and bad distribution of filler in extruded material

>[!Danger]
>Shear profile and rate are NOT THE SAME. Counter rotating has a better shear profile but not shear rate apparently


* ![[Pasted image 20240823094343.png]]
* It can be non intermeshing(?) also 
* It provides better mixing compared to single screw extruder
* Segmented screw has different types of screws in the shaft so you can add different types of screws at different zones as required
>[!important]
>Distributing mixing: distributes small particles
>Dispersive mixing: dispereses big particles

-  A complex product is something where the material flow is complex
- Injection molding is the most accurate way to deal with complex geometry
- Injection molding has the same type of machine as extrusion , except the screw length is less than the barrel length so it can move forward and backward
- Theromoforming - make the plastic soft then make imprints, you heat it above the T_g. HIPS,PE,PP used
- Rotomolding - 