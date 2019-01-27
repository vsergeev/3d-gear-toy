# Parametric Bearing Gear Toy (12/2018)

<table>
<tr>
<td><a href="images/rendering1.png"><img src="images/rendering1.thumb.png" alt="Rendering 1"/></a></td>
<td><a href="images/rendering2.png"><img src="images/rendering2.thumb.png" alt="Rendering 2"/></a></td>
</tr>
</table>

A parametric gear toy based on the [parametric spur gear](https://github.com/vsergeev/3d-gears/tree/master/parametric-spur-gear), using small bearings. The four gear teeth counts and bearing dimensions are adjustable parameters. The default settings yields a gear ratio of approximately 3 from the outside to inside gear, and uses MR104-2RS (4mm ID x 10mm OD x 4mm W) bearings. The bearings are press fit into the gear assemblies and onto the frame shafts.

See the [parametric gear toy](/parametric-gear-toy) for a bearing-less version.

This design exposes the following gear related top-level parameters:

* `TOP_GEAR1_TEETH` - tooth count of right gear (default 35)
* `TOP_GEAR2_TEETH` - tooth count of top middle gear (default 16)
* `TOP_GEAR3_TEETH` - tooth count of bottom middle gear (default 33)
* `TOP_GEAR4_TEETH` - tooth count of left gear (default 24)
* `TOP_GEAR_HEIGHT` - height of all gears (default 5mm)
* `TOP_GEAR_SCALE` - tooth scaling for process margin (default 0.925)

This design addresses material shrinkage and printing accuracy discrepancies in the gear teeth by scaling the gear teeth with the parameter `TOP_GEAR_SCALE`, which ranges from 0.0-1.0 and defaults to 0.925. This parameter scales the width of the gear teeth along their reference diameter, where 1.0 is the nominal width. If you do encounter binding or slop, you can adjust `TOP_GEAR_SCALE` to compensate.

In addition, this design exposes the following top-level parameters for bearing dimensions and bearing press fit:

* `TOP_BEARING_BORE` - inner diameter of bearings (default 4mm)
* `TOP_BEARING_DIAMETER` - outer diameter of bearings (default 10mm)
* `TOP_BEARING_HEIGHT` - width of bearings (default 4mm)
* `PRESS_FIT_SOCKET_CLEARANCE` - socket margin for press fitting the outer diameter of the bearings into the gear sockets (default 0.01mm)
    * The socket diameters are increased by this amount
* `PRESS_FIT_SHAFT_CLEARANCE` - shaft margin for press fitting the shafts into the inner diameter of the bearings (default 0.05mm)
    * The shaft diameters are increased by this amount

The press fit clearance parameters may require some adjustment for an effective press fit of the bearings.

**Design**: [Parametric Bearing Gear Toy v12.f3d](Parametric%20Bearing%20Gear%20Toy%20v12.f3d) (Fusion 360 Archive)

**Design**: https://a360.co/2EI4bxf (A360)

**STLs**:

  * [Frame.stl](stls/Frame.stl)
  * [Gear Assembly 1.stl](stls/Gear%20Assembly%201.stl)
  * [Gear Assembly 2.stl](stls/Gear%20Assembly%202.stl)
  * [Gear Assembly 3.stl](stls/Gear%20Assembly%203.stl)

**Recommended Print Settings:** 0.20mm layer height, 20% infill

**Thingiverse:** https://www.thingiverse.com/thing:3336671

**License**: [![CC-BY](https://i.creativecommons.org/l/by/4.0/80x15.png)](http://creativecommons.org/licenses/by/4.0/)
