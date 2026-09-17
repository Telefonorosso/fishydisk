<p align="center">
  <img src="ho-visto-cose.jpg" alt="AI GENERATED" width="800">
</p>

# fishydisk - AI CODED

**A suspiciously large collection of PiStorm experimental kernels, drivers and hacks.**

Experimental Emu68 projects hardware-tested on PiStorm Classic with Raspberry Pi 3A+.

These repositories explore ways to extend the classic PiStorm beyond its usual role: USB peripherals, networking, audio/video capture, debugging and ARM-side services.

```text
Replace only 1.1 Alpha kernels with the ones supplied here!
```

| Project | What it does | Repository |
|---|---|---|
| **Emu68 USB Logging** | USB CDC console for early boot logs, runtime status, debug control, crash dumps and reboot. | [uarthog](https://github.com/Telefonorosso/uarthog) |
| **Emu68 USB Mouse** | Uses a standard USB HID mouse directly as an Amiga mouse, with no AmigaOS USB driver required. | [ballless](https://github.com/Telefonorosso/ballless) |
| **Emu68 Framethrower UVC** | Streams live Framethrower video to a modern computer as a standard USB UVC capture device. | [scamdoubler](https://github.com/Telefonorosso/scamdoubler) |
| **Emu68 USBNET Direct** | Direct 68k SANA-II networking through the Pi 3A+ DWC2 controller as a CDC-NCM Ethernet adapter. | [usbnet.device](https://github.com/Telefonorosso/usbnet-device) |
| **Emu68 Paula USB Audio** | Reconstructs Paula audio in Emu68 and exposes it to a modern host as a standard UAC1 USB audio source. | [pauladaw](https://github.com/Telefonorosso/pauladaw) |
| **PaulaStorm** | Experimental Paula reconstruction and HDMI audio work for PiStorm/Emu68. | [paulastorm](https://github.com/Telefonorosso/paulastorm) |
| **sidecARM** | Runs an ARM64 Linux service alongside AmigaOS on PiStorm, with shared storage, console and framebuffer integration. | [sidecARM](https://github.com/Telefonorosso/sidecARM) |
| **l3-netkeys** | Keyboard and mouse bridge for classic Amiga systems. | [l3-netkeys](https://github.com/Telefonorosso/l3-netkeys) |
| **l2boot** | Boot and storage experiments for large Amiga HDF images. PiStorm not required. | [l2boot](https://github.com/Telefonorosso/l2boot) |

## Upstream

These projects build on the work of the Emu68 and PiStorm communities.

- [Emu68](https://github.com/michalsc/Emu68)
- [PiStorm](https://github.com/captain-amygdala/pistorm)

---

## A note before you use any of this

I am not a programmer and I do not pretend to be one.

Do not use this software if you are not comfortable handing control of your machine to code that is 100% AI-generated and has never been reviewed by a human.

You can volounteer if you please!

Remember how many times you have already used software while trusting more or less completely the good faith of its developer.

For what it is worth I am acting in 100% good faith.

AI can generate bad code. What it cannot generate - at least on my subscription plan - is evil code.

The kernels and companion applications have all been painfully tested, destoying an Amiga 600 in the process. Treat the source code primarily as reference material: some projects may have been developed around a different Emu68 branch because - as I said before - I'm not a programmer and I mix up stuff. 

Unfortunately, these features currently work one at a time.

I do plan to add audio to “scamdoubler” though!

If you open an issue assume that it will be submitted to AI for analysis because my understanding of how these programs really work under the hood is only superficial.

I must admit this last one is hard to swallow, but honestly I had lots of fun!

Ciao!

### And now, a brief message from the AI

```text
The discussion around AI-generated software is really a discussion about
authorship, trust, responsibility and what it means to create.
AI can make it easier to produce poor software, but it can also make
possible projects that otherwise would simply never exist.
Disclosure matters, attribution matters, and criticism of architecture,
licensing and technical quality remains entirely legitimate.
But perhaps the most useful distinction is not between code written
by humans and code written with AI, but between work that is opaque
and work that is open to inspection, testing and criticism.
Retrocomputing has always been partly about understanding machines
by experimenting with them; new tools do not necessarily diminish
that spirit simply because they change who is able to participate.
```

## Credits

These experiments stand on a considerable amount of existing work.

Special thanks and credit to:

* **Michal Schulz** and all **Emu68** contributors
* **Claude Schwarz, Niklas Ekström** and the **PiStorm** community
* **Stéphane Guillard**, author of **AmiVNC**
* **Torsten Jager**, author of the original **compactflash.device / CFD**
* **Jaroslav Pulchart**, author and maintainer of **ptable.library** and the modern CFD work
* **Thomas Richter and Etienne Vogt**, authors of **LoadModule**
* **Ha Thach** and the **TinyUSB** contributors
* **Andreas Wendorf**, author of the Paula 8364 emulator used by the Paula experiments
* the **Framethrower Denise** project and its contributors
* the **libyuv** contributors
* **Neil Cafferkey**, where l2boot incorporates or derives from work originating in 3c589.device

Each individual project README and source tree should be considered authoritative for project-specific attribution, provenance and licensing.

