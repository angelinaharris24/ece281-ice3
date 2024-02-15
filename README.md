# ECE 281 ICE 3: FullAdder with Top Level Design

**Fork** this repo.

[ICE 3 instructions](https://usafa-ece.github.io/ece281-book/ICE/ICE3.html)

Targeted toward Digilent Basys3. Make sure to install the [board files](https://github.com/Xilinx/XilinxBoardStore/tree/2018.2/boards/Digilent/basys3).

Tested on Vivado 2018.2.

---

## GitHub Actions Testbench

You can *optionally* enable Actions on your fork.

The workflow uses the [setup-ghdl-ci](https://github.com/ghdl/setup-ghdl-ci) GitHub action
to run a *nightly* build of [GHDL](https://ghdl.github.io/ghdl/).

First, the workflow uses GHDL to **analyze** all `.vhd` files in `src/hdl/`.

Then it **elaborates** the *any* entity with the name `*_tb`.

Finally, the workflow **runs** the simulation. If successful then it will quietly exit with a `0` code.
If any of the `assert` statements fail **with** `severity failure` then GHDL will cease the simulation and exit with non-zero code; this will also cause the workflow to fail.
Assert statements of other severity levels will be reported, but not fail the workflow.

<<<<<<< HEAD








=======
![Waveform](https://github.com/angelinaharris24/ece281-ice3/assets/156052376/cabd97e6-4816-4b5c-b997-c104a5ac51dc)


DEMO VIDEO LINK: https://youtube.com/shorts/xDj9s7ErVlk?feature=share 

## Documentation
C3C Alex Sick and C3C John Costello helped me see how to set various files as "top" so that the proper test bench will execute when appropriate. C3C Alex Sick also used the graphic on the ICE 3 instructions page to explain which signals I should declare in my test bench file.
>>>>>>> e0ebb0ad06e7c63cf67fb97050e7c6d5f8e6df0b
