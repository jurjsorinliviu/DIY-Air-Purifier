# DIY-Air-Purifier
A small DIY air purifier using off-the-shelf components for &lt;$100aud.

## Background
![](images/1576814734-MelbourneSmokeHaze.jpg)
In the summer of 2019/2020 Australia is experiencing unprecedented dangerous fire conditions driven by climate change. Much of the east coast of the country south of Brisbane is engulfed in deadly bushfires and air pollution ratings in cities such as Sydney, Canberra, Melbourne and many other regional cities and towns is many times the recommended safe levels of PM2.5 particles. The long term affects of the inhalation of bushfire smoke is mostly unknown at this time, but already people have died from respiratory distress bought about by the smoke-filled air.

There has been a great deal of discussion online and in the media about the use of P2 respirators and home air purifiers to reduce the effects of the bushfire smoke. However, information about the efficiacy of P2 respirators for bushfire smoke is not readily available and what information can be found suggests they may be of limited use. Health officials are continuing to recommend eliminating exposure to PM2.5 particles and bushfire smoke-related chemicals by remaining indoors if possible. Unfortunately for many people the summer heat makes indoors extremely uncomfortable and the evaporative air conditioners installed in many homes in my state of Victoria do not filter the damaging PM2.5 particles from the air. Health officials recommend using HEPA H13 air purifiers, however these are extremely expensive with even a basic unit suitable for a single room costing around $500aud.

With all this in mind I set about finding a way to build a low-cost, effective air purifier that would meet the minimum requirement to filter PM2.5 particles in a bedroom, so that children and at-risk people could at least sleep without  inhaling these dangerous airborne contaminants.

This github sets out the process I followed to construct and test the device, as well as the BOM and 3D print STL files for recreating the device.

## Purpose
The purpose of this project is to create a small air purifier suitable for a bedroom or caravan (or similar sized space) that meets the following critiera:
  - Costs under $100aud to build (in parts);
  - Can be constructed with relatively low levels of technical skill (there is soldering of two wires required);
  - Uses off-the-shelf components available in most Australian cities, or by order over the internet from Australian suppliers; and
  - Uses a HEPA H13 rated filter; and
  - Is powered from a commonly available USB powerbank.

## Method
I selected a readily available HEPA H13 rated filter normally used in cheap vacuum cleaners and available from Bunnings Warehouse. The rest of the air purifier is based around that filter. I then selected a range of 120mm computer fans with relatively high static pressure ratings (>2.0 mmAq) that could operate on 12vDC. As the fans are 12vDC I used a USB 'booster cable' which steps-up the voltage of any USB-A port from 5v to 12v; these cables are available online or from a range of electronics shops such as Jaycar.
After selecting the components I then designed a fan housing using Fusion 360 that provides the interface between the 120mm and the HEPA filter. The filter comes with a removable seal/cover at one end, so I use that end as the base of the unit and fit the fan to the top.
After basic testing with a small smoke generator to ensure the selected fans could draw air through the filter to a reasonable standard I have determined the project suitable for release so others can create their own version of this device both for use in their homes and for further testing.

![](images/Air_Purifier_V2_2020-Jan-13_09-48-57PM-000_CustomizedView1437179471.png)

The image above shows the rendered view of the device from Fusion 360 with an iPhone X for scale. The first version of the housing used a separate fan grill but I was able to eliminate this by incorporating the hex pattern into the housing, which also saved about $7 off the cost.

## Materials
The BOM for the air purifier is:
  - 1x 120mm computer fan. I recommend you use this one: https://www.pccasegear.com/products/36033 which draws around 600ma, or if you have a larger power bank this one: https://www.pccasegear.com/products/27866 which draws around 1000ma but pushes a lot more air. The second fan is also a bit more expensive so if the budget is tight the first one will work perfectly.
  - 1x 2.5mm DC bulkhead socket: https://www.jaycar.com.au/2-5mm-bulkhead-male-dc-power-connector/p/PS0524. This allows you to plug the device in with the USB booster cable to supply 12vDC to the fan.
  - 1x 12v USB booster cable: https://www.jaycar.com.au/universal-usb-12v-step-up-power-cable/p/PP1978./ Ensure you get the 12v version as these do come in 9v also and that wont work.
  - 1x HEPA H13 filter: https://www.bunnings.com.au/powerfit-h13-hepa-cartridge-filter_p6210793. Ensure you get this exact filter as the housing is dimensioned to fit over the end. Other filters with the same diameter may work, but are untested. This filter comes with an end-piece that will be the base of your device, so ensure this is in the box.
  - 1x USB power bank. Any power bank that can supply 5v >1amp will work but for best results choose one at least 10,000maH that supports pass-through charging. This allows you to use the battery as a UPS for the air purifier and run it continuously from a mains power, with  the battery being used for power outages.
  - 1x 3D printed fan housing. The STL file can be found in: 
  - 4pin fan cable: https://www.pccasegear.com/products/35666/cablemod-4-pin-fan-to-3x-4-pin-fan-y-cable-black-30cm. This cable is cheap and gives you three female plugs so you can make multiple devices with the one cable.
  - Heatshrink tubing 8mm (30mm long).

## Tools
You will need the following tools to assemble the device:
  - Soldering iron and solder
  - Pliers (with wire cutters)
  - Scissors
  - Multimeter (to determine correct polarity for the wiring of the socket)
  
## Assembly
### Step 1
Assemble the wiring harness for the 2.5mm socket.
- Take the 4pin fan cable and cut one of the female plugs off leaving about 10cm of cable on the plug.
- Trim back the cable protective sleeve with the scissors leaving about 2cm of exposed wires.
- If you use the cable I linked above to make this harness you need the orange (+) and black (-) wires, other cables may differ so check before you go further you have the correct wires.
- Keeping the orange and black wires the length you cut previously, cut the other two wires off shorter so they will be inside the cable sheath and out of the way.
- Strip and tin the orange and black wires with new 60/40 solder and place on the heatshrink tubing over the top of the cable protective sheath.
- Determine the correct terminal lugs on the 2.5mm socket using the multimeter. Then solder the + and - wires to the correct terminals.
- Pull the heatshrink over the socket lugs and shrink it with a heat gun or flame.
- The completed wiring harness should look similar to this
![](xxx)
