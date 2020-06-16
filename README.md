My lab work from my Operating Systems Course
---

This repo consists of the final lab work from my Operating Systsmes course. It follows the "OSTEP" *Operating System: Three Easy Pieces* (Virtualization of the hardware, Peristence of important data, and Concurency) book. I really enjoyed this course; however, 10 weeks was not enough for me to feel satisfied with my understanding. Thus I am reading the OSTEP book on my own with hopes to replicate what was accomplished here. It uses QEMU for hardware emulation.

Things you should know:
- Some of this work was provided by the instructor (**blue9057**).
- In order to compile, you will need QEMU.

To setup...

Run the setup script `./setup.py`

After that, you should be able to make the project using Make in your shell of choice.

(The instructions below taken from the instructor's lab setup guide, viable here: https://bit.ly/37xqOAa).

`make qemu-nox`

    Like make qemu, but run with only the serial console. To exit, press Ctrl-a x. This is particularly useful over SSH connections to Athena dialups because the VGA window consumes a lot of bandwidth.

`make qemu-nox-gdb`

    A combination of the qemu-nox and qemu-gdb targets.

`make run-name`

    (Lab 3+) Run user program name. For example, make   run-hello runs user/hello.c.
`make run-name-nox, run-name-gdb, run-name-gdb-nox,`

    (Lab 3+) Variants of run-name that correspond to the variants of the qemu target.

The makefile also accepts a few useful variables:

`make QEMUEXTRA=’args’ …`

    Specify additional arguments to pass to QEMU. 