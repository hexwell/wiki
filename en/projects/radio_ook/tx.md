LF radio OOK transmitter
========================

This is a receiver I plan to use with my [receiver](rx.md). The result
should be an OOK tx/rx pair

Considerations:

-   I need a good design for the transmitter. It should feature a simple
    fixed frequency oscillator and optionally if the signal is too week
    an amplifier made with the lowest count of parts possible and
    possibly based around a simple NPN transistor (2N2222)

-   I need components in order to make this projects. I might consider
    buying them when I have a nice design.

-   I need a scope to debug the circuit. The oscillator resonant
    frequency need to be checked with it.

-   When the frequency is determined precisely the title of this and the
    receiver posts should be updated to match it.

Frequency
---------

After having spent a long time thinking about this I came to the
conclusion that I want a **30 Mhz** frequence if possible. This is so it
will be possible to see this transmitter with an RTL-SDR. The
feasibility of this option should be checked with the crystal
considerations below.

Ten Minute Transmitter
----------------------

This is a nice design currently under evaluation.

[ten minute
transmitter](https://makerf.com/posts/ten-minute-transmitter)

This is what I understand about it.

-   It\'s an oscillator, so it\'s a CW transmitter de facto
-   Oscillators are made made of an amplifier a filtered feedback (a
    filter that provides feedback to the amplifier)
-   The amplifier in this case is a single transistor amplifier
-   The transistor needs to be biased in order to properly amplify the
    signal
-   A transistor bias provides some middle voltage that can be altered
    positively or negatively by a signal (the feedback in this case)
-   The filter in this case is just the crystal
-   Crystals should behave like an LC tuned circuit with a series
    capacitor (as they do not conduct DC)
-   C1 is for power supply stability
-   L1 is an RF Choke, although I\'m not fully convinced it\'s it\'s
    only purpose
-   R1 is for transistor bias and to make it start conducting at power
    up
-   C3 should be for impedance matching with the antenna (?)
-   C2 is to not fry the transistor when the key is released, as it
    charges up to the supply voltage and stops the oscillator by making
    the voltage across the transistor (V collector-emitter) = 0

So the doubts that I have yet to dispel are:

-   How does the crystal work and can I get one for 30 MHz?
-   Can the crystal be replaced with an LC tuned circuit (optionally
    with a DC blocking capacitor)?
-   Is C3 just impedance matching if it\'s impedance matching at all
-   Some loading resistor between transistor emitter and keyer might be
    useful. This would probably make the transistor heat up less and
    probably would make the use a non metal-can/heatsinked transistor
    feasible.
-   The biasing resistor may as well be a voltage divider probably. This
    needs to be investigated

Possible nice explanation:
<https://www.electrical4u.com/crystal-oscillator/>
