# Sony WH-1000XM4 ANC Repair

This repository documents how I diagnosed and repaired a Sony WH-1000XM4 headset with unstable Active Noise Cancelling (ANC).

## The problem

My headphones started making a high-pitched squealing noise, but only when ANC was enabled. The problem became more noticeable over time, especially after longer use. Normal audio playback still worked.

## Initial suspicion

At first, I was not sure whether the issue came from software, sealing, moisture, or one of the ANC microphones. After comparing the symptoms with similar reported failures and looking at how the problem behaved, the external feedforward microphone became the main suspect.

## What I found

After opening the earcup, I found visible discoloration and residue near the microphone housing. Cleaning the area improved the behavior temporarily, which made the microphone even more likely as the source of the problem.

I did not use laboratory measurements or oscilloscope testing here. The diagnosis was based on symptom behavior, visual inspection, comparison with similar known failures, and the final repair result.

## Repair

I replaced the original microphone with a compatible electret microphone that matched the required sensitivity more closely than common lower-sensitivity alternatives.

During soldering, I kept the temperature controlled and the contact time short to avoid damaging the replacement microphone.

## Result

After the replacement, the ANC squealing disappeared and the headphones worked normally again. I did not notice any obvious loss in audio quality or ANC performance during normal use.

## What this project shows

- practical fault diagnosis
- electronics disassembly and repair
- component selection using datasheets
- precision soldering
- technical documentation

## Repository contents

- `XM4_Repair.pdf` - full report
- `images/` - repair photos
- `media/` - supplementary video
- `README.md` - project summary

## Selected Images

### Original microphone and visible oxidation

<p align="center">
  <img src="./images/original-microphone-with-visible-oxidation.jpg" width="320">
  <img src="./images/oxidation-on-microphone-cover.jpg" width="320">
</p>

### Replacement microphone and repaired result

<p align="center">
  <img src="./images/replacement-microphone-closeup.jpg" width="320">
  <img src="./images/soldered-replacement-microphone-closeup.jpg" width="320">
</p>

### Opened earcups

<p align="center">
  <img src="./images/both-earcups-opened.jpg" width="320">
  <img src="./images/both-earcups-opened-with-replacement-microphone.jpg" width="320">
</p>

Additional repair photos are available in the `images/` folder.

## Supplementary video

- `media/anc-squealing-before-repair.mp4`

## Full report

[Open the report](./XM4_Repair.pdf)

## Note

This repair was done carefully and at my own risk. Opening consumer electronics may void warranty.
