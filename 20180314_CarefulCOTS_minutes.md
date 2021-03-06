Phase 4 Space organized and hosted an ASCENT conference call on 14 March 2018 with Nate Temple and Neel Pandeya from Ettus Research. The purpose of the meeting was to identify next steps for a careful COTS layout of a current Universal Software Radio Peripheral (USRP) device, primarily for AMSAT payloads.

Attending were Howie D., Michelle T., Nate T., Neel P., Ray R., and Jordan T.

With the Tritium unavailable due to business and technical reasons, the discussion moved on to which design would be the best starting point. 

The X300/310 has a National Instruments chip that is proprietary. The chip provides PCI Express interface, but also performs other functions. Even if one does not use the PCI Express interface, the chip is required. It is highly unlikely that National Instruments will release anything about this chip. This puts the X310 further down the list for consideration. The other USRPs do not have this chip. 

The E310 has a Zynq 7020 (Artix 7) and is currently available. 

The E320 will be available late summer or early fall 2018 and will have a Zynq 7045 (Kintex 7). 

The E320 will be code-compatible with established USRPs and will use the Analog Devices 9361 RFIC. 

Nate and Neel will pursue what level of intellectual property support from and agreements with Ettus Research are necessary to commence work on a re-layout. The Gerber, the full Bill of Materials, and the parts models are all being requested. We may get some, none, or all of this level of information. If an NDA is required, then it will be presented to AMSAT for consideration and signing. AMSAT has signed similar NDAs in the past and no specific issues with signing an NDA were anticipated. 

Work can commence with the E310. Assuming success, we can consider moving to the E320 when it's available. With this basic roadmap, a progression that keeps pace with current USRPs can be established.

Nate emphasized that a re-layout offers multiple opportunities to address a variety of challenges. For example, a co-processor could be added to handle things like LDPC forward error correcting codes. Or, instead of a co-processor, add an additional 7020. For RF, the second output can drive an LO for 10GHz. RF components can be incorporated. 

Everyone agreed that heat dissipation and size restrictions are substantial primary challenges for this design. 

Ray explained that while GOLF doesn't have the same bandwidth requirements as Phase 4, it is believed to be possible that one can use a larger part (like a 7045) and turn off gates in order to save power. This was in the context of having two hardware variants, one for higher bandwidth deployments and one for lower bandwidth deployments. Avoiding the management of multiple hardware variants would be beneficial for several reasons. 

Determining the FPGA requirements for the Phase 4 payload is necessary to determine the exact part size required. The FPGA requirements for GOLF may not necessarily be as large, but a goal for GOLF is to allow experiments and to get as much longevity as possible. Therefore, as large a part size that the power bus can support would be ideal. 

We discussed several technical challenges including memory. Jordan mentioned triple modular redundancy (TMR) which is used in some types of Error-correcting code memory (ECC) memory.


Other action items included:

 * Set up a Slack channel for careful COTS (private channel #careful_cots set up in order to better support work that might be under NDA) 
 * Ensure contact information is shared (done)


