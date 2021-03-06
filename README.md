This repo provides Latex source for materials related to nuclear
physics.

Content
=======
Materials in this repo are related to three courses offered at MIT's
nuclear science and engineering department:

- 22.101 Applied nuclear physics: basic quantum mechanics and modern
physics material, extending into nuclear structure, nucleon-nucleon
scattering, radioactive decay, and neutron interactions.

- 22.106 Neutron interactions: neutron transport theory, starting from
  cross-sections and R-matrix theory, and covering the
  differential-integral and integral form of the transport equation,
  Monte Carlo, CPM, MOC, SN, PN methods.

- 22.211 Nuclear reactor physics I: slowing down equation with
  emphasis on resonance treatment and self-shielding treatment,
  spectral calculation, diffusion theory, point kinetics, nodal
  diffusion theory (CMFD, NEM, ANM, SANM), homogenization and
  de-homogenization.

**If you just want the pdfs**, visit www.mit.edu/~lululi

Build
=======

To build the Latex sources in this repo, you would need to git clone
and build tek (https://github.com/palmer-dabbelt/tek), which is the
Latex Makefile generator I use. Then run

```
TEXINPUTS="$(readlink -f latex)/:" tek
```

which generates a Makefile that points to the latex style files
(latex/) used in these Latex sources.

Then run

```
make
```

Note: Latex package dependencies can be found in
latex/school-style-packages.sty. The very first time you build this
repo you are most likely going to get error messages of missing some
packages (depending on your Latex distributions they come with a
different set of random stuffs). You can fix so by installing linux
distribution packages, or installing Latex distribution packages, or
by going to CTAN to get the file.


Contact
=======

Please feel free to create a pull request/collaborate etc. My email
address is lululi@mit.edu for now.