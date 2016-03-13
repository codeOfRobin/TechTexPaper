# Smart Bandages

In smart bandages, sensors are integrated to provide a measure for the pressure applied to a human. Examples of these include :-
- **The Salzmann Medico Sub-bandage Pressure Monitor** : This device consists of a monitor and thin plastic sleeve with four paired electrical contact probes, which is laid on the leg surface and bandaged over.  The sleeve is inflated with air until the contacts are broken when the pressure exerted by the air is greater than the pressure exerted by the outer compression layer.
- **The Oxford Pressure Monitor Mark 2** : measures pressure by observation of the pressure flow characteristics of small pulses of air. The probes can be taped together or are available as a sheet.

For the measurement in compression bandages, 2 types of sensors can be considered - Force sensors and air sensors. The pressure sensors would have to be accurate, reliable, robust and small.

Air Sensors are small air filled devices. The sensor has a sponge filling used to maintain the shape of the device and reduce discomfort to the patient. However, they come with their fair share of problems :-
- The reading vs pressure changes are not linear. They drop at around 1000 Pa.
- There should be a suitable volume of air in the air sensors before they are used. The quantity of air in the sensors affects the measurement results, as the sensor needs air to transfer the pressure. For example, if there is no air in it, data cannot be obtained. Otherwise, if it accepts too much air, the existing air pressure will result in large change.
- Air leaks may render the sensor completely useless. They also make testing very difficult
- The soft plastic usually used in these sensors may break under repeated use.

![Image Alt](http://i.imgur.com/dAoDUVu.png)

Force Sensors are typically tested by application of metric weights. The relationship between weight applied and readings is typically linear.

![Image Alt](http://i.imgur.com/eFrZWtV.png)

It is because of the above reasons that force sensors are usually preferred because the readings are linear with pressure (Laplace's law), simple electronic interface and robustness.

In order to test these sensors, a hollow dummy leg is used to model the 'average' leg. The leg is kept hollow to improve ease of construction and wiring.

Another new innovation in bandages is to etch rhombi on the surface of the bandage. The aspect ratio of the rhombi is kept such that when a constant amount of the required pressure is applied, the rhombi are stretched to be approximately square. This provides an easy visual clue to the doctor/nurse that the right pressure has been applied.

## Final Product

The circuit diagram and the screenshots of the software(built in Visual Basic) are seen below.

![Image Alt](http://i.imgur.com/RBlgb2U.png)
![Image Alt](http://i.imgur.com/ErraizQ.png)

## Testing and review results

First, a test was conducted to see if the surface area of the instrument affected the pressure readings. The test was carried out with the compression bandage applied to the bare sensor (diameter 6.5mm) and then to the sensor with a disk attached (diameter 18mm). To achieve the same bandage tension, a compression bandage with regular squares was used. The principle was that if the tension of the bandage could be kept same when it was applied, the widths of the squares would be same.

Following are the results for different circumferences of wrapping(corresponding to decreased height of wrapping). As can be seen, the pressure increases with the tension applied. But, the pressure for increasing radius remains same, which is a desirable outcome.

![Image Alt](http://i.imgur.com/NjnXw4m.png)

However, if we increase the number of layers of a bandage, the pressure increases linearly, following Laplace's law

![Image Alt](http://i.imgur.com/l371tAy.png)

## Conclusion

It was observed in the study that the results do not exactly match up with Laplace's law. This may be due to several reasons. Firstly, the materials are different (a real human leg is much more compressible than the wood model used in the lab). So, the shape of the leg may change due to this pressure. Secondly, in the real leg, the pressure applied by the bandage has to reach the veins of the leg. These veins lie at deeper depth under a layer of skin and fat. In the wooden model, this force is only on the surface. Lastly, differing levels of training  in the volunteers may cause issues.

## References

- Sockalingham S., Barbenel J.C., Queen D., Ambulatory monitoring of the pressures beneath compression bandages. Care Science and Practice, 1990, 8(2), 75-79.
- Callam A.B., Haiart D., Farouk M., et al., Effect of time and posture on pressure profiles obtained by three different types of compression. Phlebology, 1991, 6, 79-84.
