# fishydisk

**A suspiciously large collection of PiStorm experimental kernels, drivers and hacks.**

A collection of experimental Emu68 projects developed and hardware-tested on **PiStorm Classic with Raspberry Pi 3A+**.

These repositories explore ways to extend the classic PiStorm beyond its usual role: USB peripherals, networking, audio/video capture, debugging and ARM-side services.

> **Target platform:** PiStorm Classic + Raspberry Pi 3A+  
> These projects are experimental and are not official Emu68 releases.

| Project | What it does | Repository |
|---|---|---|
| **Emu68 USB Logging** | USB CDC console for early boot logs, runtime status, debug control, crash dumps and reboot. | [Emu68-USB-Logging](https://github.com/Telefonorosso/Emu68-USB-Logging) |
| **Emu68 USB Mouse** | Uses a standard USB HID mouse directly as an Amiga mouse, with no AmigaOS USB driver required. | [Emu68-USB-Mouse](https://github.com/Telefonorosso/Emu68-USB-Mouse) |
| **Emu68 Framethrower UVC** | Streams live Framethrower/Amiga video to a modern computer as a standard USB UVC capture device. | [Emu68-Framethrower-UVC](https://github.com/Telefonorosso/Emu68-Framethrower-UVC) |
| **Emu68 USBNET Direct** | Direct 68k SANA-II networking through the Pi 3A+ DWC2 controller as a CDC-NCM Ethernet adapter. | [Emu68-USBNET-Direct](https://github.com/Telefonorosso/Emu68-USBNET-Direct) |
| **Emu68 Paula USB Audio** | Reconstructs Paula audio in Emu68 and exposes it to a modern host as a standard UAC1 USB audio source. | [Emu68-Paula-USB-Audio](https://github.com/Telefonorosso/Emu68-Paula-USB-Audio) |
| **PaulaStorm** | Experimental Paula reconstruction and HDMI audio work for PiStorm/Emu68. | [paulastorm](https://github.com/Telefonorosso/paulastorm) |
| **sidecARM** | Runs an ARM64 Linux service alongside AmigaOS on PiStorm, with shared storage, console and framebuffer integration. | [sidecARM](https://github.com/Telefonorosso/sidecARM) |
| **Framethrower Audio Experiments** | Experiments around digital Paula/audio capture using the Framethrower bus-snooping path. | [Framethrower-Audio](https://github.com/Telefonorosso/Framethrower-Audio) |
| **l2boot** | Boot and storage experiments for large Amiga HDF images on the PiStorm/Emu68 platform. | [l2boot](https://github.com/Telefonorosso/l2boot) |

## Upstream

These projects build on the work of the Emu68 and PiStorm communities.

- [Emu68](https://github.com/michalsc/Emu68)
- [PiStorm](https://github.com/captain-amygdala/pistorm)

---

## A note before you use any of this

I am not a programmer, and I do not pretend to be one.

Do not use this software if you are not comfortable handing control of your machine to code that is 100% AI-generated and has never been reviewed by a human — except perhaps by you.

Remember how many times you have already used software while trusting, more or less completely, the good faith of its developer.

For what it is worth: I am acting in 100% good faith.

AI can generate bad code. What it cannot generate — at least on my subscription plan — is *evil* code.

The kernels and companion applications have been tested. Treat the source code primarily as reference material: some projects may have been developed around a different Emu68 branch or milestone.

Unfortunately, these features currently work one at a time. I do plan to add audio to “scamdoubler”, though.

If you open an issue, assume that it will be submitted to AI for analysis, because my understanding of how these programs really work under the hood is only superficial.

### And now, a brief message from the AI

The discussion around AI-generated software is really a discussion about authorship, trust, responsibility and what it means to create.

AI can make it easier to produce poor software, but it can also make possible projects that otherwise would simply never exist.

Disclosure matters, attribution matters, and criticism of architecture, licensing and technical quality remains entirely legitimate.

But perhaps the most useful distinction is not between code written by humans and code written with AI, but between work that is opaque and work that is open to inspection, testing and criticism.

Retrocomputing has always been partly about understanding machines by experimenting with them; new tools do not necessarily diminish that spirit simply because they change who is able to participate.

In the end, the interesting question may be less “who wrote this?” than “what did this allow someone to explore, learn, test or build that would otherwise not have existed?”
