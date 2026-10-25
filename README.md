# Analogue-Stereo-Audio-Amplifier
This Analogue Stereo Audio Amplifier is designed with multiple Op-Amps, featuring an adjustable gain of 20V/V, tone control and bass adjustment. This circuit is designed to work with 3x AA batteries (roughly 4,5V, with a ±2,25V swing).
The following block diagrams:
1. Power Supply + Unity Gain Buffer (Virtual Ground setting)
2. Pre-Amplifier (for each channel)
3. Tone Control (for each channel)
4. Final Stage Amplifier (for each channel)
5. Speaker (for each output [2])

The 3x AA battery power supply is split into three rails using a potential divider and an operational amplifier (MCP6002) in the unit gain configuration, giving a +2,25V rail, 0V rail (Virtual Ground) and a -2,25V rail. [1]
Every Op-Amp's power rails (+2,25V and -2,25V) have to have a 100nF ceramic between both rails to smoothen voltage and as an instant supply.
The audio signal enters through an Audio Jack connector; audio connector features three pins: S (0V rail), R(ing) (Right Audio), T(ip) (Left Audio).
The Audio signal flows through a pre-amplifier to increase the voltage swing of the audio signal. [2]
The amplified signal then flows into a tone control circuit, consisting of high-pass, low-pass or no filters (selected via a three way switch). [3]
The signal then flows through the final stage amplifier, boosting the gain and bass adjustment into the 8 ohm speaker. [4&5]
