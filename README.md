# 8-Bit-Successive-Approximation-Register-ADC-Chip-CMOS-Design

__SAR ADC__

The Successive approximation register ADC converts a continuous analog waveform into a discrete digital representation via a binary search through all possible levels before finally converging upon a digital output for each conversion. The ADC takes a continuous analog waveform as input. A Sample and Hold circuit perform a sample to the input base on its clock frequency and past it output to the comparator, which checks if the value is less or greater than the DAC output. The comparator outputs a one if the DAC voltage is less than Sample and Hold value (S/H), and a 0 if the DAC voltage is greater than the S/H output. The output of the comparator is fed into the SAR register, which produces a discrete digital representation via a binary search through all possible quantization levels. The SAR must run N (number of bits) faster than the S/H in other to produce all bits level. The DAC register converts the binary output of the SAR via an R-2R Ladder register, see figure below. 

![SAR - DAC](https://images.app.goo.gl/d7VuwVg7xA5Jmtdi6)

  
  __Please check out file__ _EECE 416 Project Report.docx_ __for complete understand of the project__
