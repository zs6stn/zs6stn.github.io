---
title: Why SWR meters can be bad for your station by Chris Turner ZS6GM
author: chris
date: 2023-12-31
tags: [Tech Talks, SWR]
toc: false
---

Chris Turner, ZS6GM December 2023

When I listen across the ham bands, there seems to be an on-going obsession with achieving ‘low SWR’ on the feedline in the belief that low SWR is an indication of optimum radiation from the antenna. I'm reminded of Walter Maxwell W2DU1 who said *“we are in this state of mind because so much misleading information has been, and is still being published concerning the behaviour of antennas' performance in the presence of reflections when mismatched to the antenna and the meaning and interpretation of the SWR data”*.  

We've been conditioned to believe that  'one – to – one' SWR is the ultimate goal. This is a myth that has been propagated ‘as fact’ in so many articles and papers even though the correct teachings are contained in reference books such as the ARRL Antenna Book and the reference book Antennas by John D Krause.

### So, what is SWR?

SWR is the ratio of forward power to reflected power on a transmission line. Most so called SWR meters (more correctly called reflectometers) actually measure voltage standing wave ratio. VSWR is the ratio of (forward voltage + reflected voltage) to (forward voltage – reflected voltage) as measured on a transmission line.

### What is a Transmission Line?

It is to RF what a hose is to water. It may be  an open wire line (sometimes referred to as ladder line) or coaxial cable or even a wave guide. All transmission lines of whatever form have a characteristic impedance related to the mechanical dimensions. In amateur radio, open wire lines generally have an impedance of 300, 450 or 600 ohms. Common coaxial cables have an impedance of 50 or 72 ohms. There are some specialised cables used for matching which have other impedances.

When a transmission line is terminated at one end in its characteristic impedance by an antenna or other load, and power is applied at the opposite end, all the power will be absorbed in the antenna and there will be no power reflected back. The VSWR will be 1:1 at any point on the transmission line. So if you cut the transmission line and insert a reflectometer at any point, there will be no reflected power. However, when a transmission line is terminated in an impedance other than its characteristic impedance, Standing Waves will be present on the line. The question is whether this is important in the radiating of signals?

### Let us now consider the Conjugate Match

The transfer of power from a source (the transmitter) to a load (the antenna) follows Ohms law. When the source and load are pure resistances, maximum power transfer takes place when the load resistance is equal to the source resistance. But what happens when the load is a complex impedance and has resistance and reactance?  This is when we use a technique called Conjugate Matching.

Conjugate Match is achieved when the reactive portion of the load is matched by applying an equal but opposite reactance at the source.

An antenna that is not self resonant will always have a resistive component and a reactive component which may be inductive or capacitive. Matching cancels the reactive component in the antenna so that only the resistive portion is left and Ohm’s Law applies.

Optimum power is delivered by a transmitter using conjugate coupling into the transmission line. But, this match is in one direction only, that is forward. If one looks back into the transmitter, the line is completely mismatched when the transmitter is delivering power. An antenna matching unit or built in antenna tuner provides conjugate coupling into the transmission line Remember this because we will discuss it later.

It is important to note that matching need not be applied at the antenna, but may be applied at any position on the transmission line between the transmitter and the antenna.

You may ask “why doesn't the mismatch at the antenna cause high SWR resulting in losses?”

Try and picture this:  Conjugate Match means that if in one direction from a junction, the impedance has the dimensions R+jX (inductive impedance) then in the opposite direction the impedance will have the dimensions R-jX (capacitive impedance). What this means is that when a conjugate match is accomplished in a system, any reactance appearing at any junction is cancelled by an equal and opposite reactance. This includes any reactance appearing at a non-resonant antenna.

This reactance cancellation results in a net system reactance of zero establishing resonance in the entire system. In other words the entire system is resistive and has no reactive component.  In this condition, the transmitter delivers it maximum available power to the antenna.

### Let's Examine The Mechanism

The transmitter output stage has tuned circuits which provide a conjugate match between the output impedance of the tubes / transistors and the transmission line. In the case of a tube transmitter, the Pi output coupler provides the match between the tubes and the transmission line. In the case of a solid state transmitter, this can be means of a built-in or external antenna matching unit (ATU)

In the case where the antenna is purely resistive - self resonant, and it’s resistance is the same as the transmission line, maximum power will be absorbed by the antenna and radiated into space.  

Let us consider a lossless transmission line. If the transmission line is either open circuit or short circuit at the far end,  all the power conducted along the transmission line will be reflected back to the transmitter. If the antenna is reactive, that is it comprises resistance and reactance, a portion of the power will be reflected back towards the transmitter and a portion will be absorbed by the antenna.

Here is the myth. Many people believe that power reflected back to the transmitter will be absorbed in the transmitter causing over heating or damage.  This is a myth.

So what is the truth?

Reflected power does not make its way back to the active output amplifier and it cannot be absorbed into the transmitter. Remember as we said earlier; matching is in one direction only, that is from source to load. When the reflected power arrives back at the transmitter, it sees a total mismatch so it is again reflected back towards the antenna. A bit like ping pong.

If we had a lossless transmission line, because there is no resistive loss of power at the antenna, and there is no absorption of power at the transmitter, there is no loss of power.  All the power will be radiated by the antenna.  In the real world, transmission lines do have some loss. So, any power reflected back to the transmitter will incur loss in both the reflected and forward directions.

### Now Let's Prove the point

This experiment will prove that no power is lost at the transmitter resulting from a mismatch or high SWR. A directional wattmeter will show that forward power always = source power + reflected power.

For this experiment it important that the transmitter output is fixed and does not automatically compensate for changes in load. In other words output power levelling or ALC must be disabled. Ideally, a tube transmitter should be used.

Connect a directional wattmeter between the transmitter and the transmission line, after any tuner. It's no good putting the wattmeter between the transmitter and the tuner as this will defeat the measurement. Arrange for a mismatch at the antenna end of the line by moving the transmit frequency away from perfect antenna match so that reflected power may be observed.

You now establish a reference point. Connect a dummy load to the output of the wattmeter and measure forward power. This we call source power.  There should be zero reflected power. Now remove the dummy load and connect the transmission line. Again measure the forward power and reflected power. You will notice that the forward power will equal the source power + reflected power. So, if the source power is 20 Watts and the reflected power is 5 Watts, the forward power will measure 25 Watts on the wattmeter.

Modern solid state transmitters use an output power levelling circuit. This means that if there is reflected power, the transmitter will reduce its output so that the forward power is also reduced. This disguises the additive effect of forward and reflected power. This is why it is important that a fixed source power is used for this experiment.

### The question you may ask, is where to Match

I said earlier that it is not necessary to match the antenna at its feed point but that matching can take place anywhere between the source (transmitter) and the load. Coaxial stubs and tuned transmission lines are examples of distributed matching. An antenna matching unit at the transmitter output is just as effective. Remember to place your SWR meter between the transmitter and the ATU so that you match the system to the transmitter output. Not between the ATU and transmission line.

The only reason to aim for a reasonable antenna SWR (typically less than 3:1) is to mitigate transmission line losses.  If transmission line losses are not a factor, you can quite happily use non-resonant antennas like the G5RV/ZS6BKW with an antenna matching unit at the transmitter output. You can also use a fairly narrow band self resonant antenna over a much wider range of frequencies and suffer no measurable loss in radiated power and cause no damage to your transmitter.

So in closing, I want you to throw away the misbeliefs and myths and remember this:

The truth is that all the power that enters the line from the transmitter is absorbed by the antenna except that which is dissipated in the line itself due to transmission line loss.. because the power reflected by the mismatch is conserved and returned to the antenna by re-reflection from the transmitter matching circuits.  This is true even when the antenna is not matched to the line impedance

Remember that because the forward power in a transmission line is the sum of the source and reflected powers, the forward power will always be greater than the transmitter power when the SWR is greater than 1. Therefore, our concern of SWR involves only the loss due to transmission line attenuation. This means that we can tolerate a higher SWR when line attenuation is low.  This is why open wire feeders are very effective for non-self-resonant antennas.

The main reason to aim for low SWR is to permit the easy matching of a transmitter with a fixed output impedance into a 50 ohm feedline. The use of an antenna matching device between the transmitter output and feedline will mitigate any SWR effects on the feedline. Note that the SWR meter must be placed between the transmitter and tuner and NOT between the tuner and the feedline.

*References:*

1. Walt Maxwell is a Technical Adviser in the field of antennas and transmission lines and is the author of the book Reflections, Transmission Lines and Antennas, ARRL 1990.  From 1960 to retirement in 1980 he was in charge of Astro's Space Centre Antenna Laboratory and was responsible for the design of a multitude of antennas for spacecraft. Prior to this he was a senior engineer a RCA.
