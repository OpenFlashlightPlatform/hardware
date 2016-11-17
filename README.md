# Blue Sun OFP

The Blue Sun Open Flashlight Platform is an open source (both hardware and software)
attempt at creating a software-defined ultra-reliable high-performance flashlight.

This project was inspired by the AvE Midnight Sun project, and is intended to match
with the mechanicals developed there, both physically and in spirit. To that end,
a core set of specifications were identified:

 0. The project must be fun. This rule can be applied to override any subsequent
    rule.
 1. The design must be skookum. If in doubt as to the actual definition of "skookum"
    just go balls to the wall and hope the result is sufficiently epic.
 2. The platform should be capable of driving a diverse range of COBs at up to
    160W (40V / 4A). Ensure that in every aspect of the circuit, rule 1 is
    strongly enforced, so that excursions beyond 160W are tolerated and the
    circuit can dynamically detect and react to overload.
 3. The driver should have fine-grained current-mode control of the COB.
 4. The platform should operate from a 3s LiPo battery, and be capable of charging it
    from a 12V source. Naturally, transients, noise and polarity inversions on this
    source must be tolerated. Furthermore, all best practices for LiPo operation
    must be followed including UVLO, cell balancing and temperature monitoring.
 5. The platform should be accessible and open source at every possible level.
    To that end, it should be compatible out-of-the box with an Arduino IDE
    and programmable without any non-free tools, software or licenses.
 6. The circuit must be implemented in the spirit of Rule 1. Everything must be
    resistant to temperature, humidity, vibration, ESD, overvoltage, cell imbalance,
    and short circuit. The circuit must continue to function after being shaken
    in a container of salty boiling water mixed with conductive metal powder.
 7. Every net in the circuit, including internal nets and power supply rails,
    must pass IEC 61000-4-2 (25kV) and IEC 61004-4 (40A) ESD resistance tests.
 8. The firmware itself, both in source form and compiled form, must adhere to
    rule 1. In particular, wherever possible (in that it does not contradict rule
    5), the firmware should be MISRA C:2012 compliant.
 9. Every aspect of the project must be well documented. If the primary maintainer
    were to become unavailable, the community ought to be able to pick up and
    continue.
