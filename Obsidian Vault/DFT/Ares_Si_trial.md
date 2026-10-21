[ares059@login02 relax]$ cat ares.log 
XC signature         : XcConfig { backend: GgaPbe, functionals: XcFunctionalKind { exchange: PbeX, correlation: PbeC } }
# ARES Job Execution Report
version     : 0.1.0
calculation : vc-relax
input       : ares.toml
topology    : p4 / b1 / g1 / threads1

## Job Initialization
### System
atoms       : 2
species     : 1
electrons   : 8
bands       : 12
flavor      : PAW

### Pseudopotentials
| Species | File | Type | Valence electrons | Functional |
|---|---|---|---|---|
| Si | /public/home/ares059/ares/dft/practice/relax/../Si.GGA_PBE-JTH.UPF | Paw | 4 | SLA PW PBX PBC |

### Basis and K-points
wavefunction cutoff : 5.00000000e1 Ry
density cutoff      : 2.00000000e2 Ry
wavefunction FFT    : 36 x 36 x 36
density FFT         : 36 x 36 x 36
k points            : 8

### Electronic Settings
XC backend          : GgaPbe
solver              : Davidson
mixing              : ModifiedBroyden
mixing beta         : 7.00000000e-1
maximum iterations  : 200
SCF threshold       : 2.00000000e-8 Ry

## Job Execution Information

VC Relax cell/ionic loop
  maximum evaluations : 40
  energy threshold    : 4.00000000e-5 Ry
  force threshold     : 6.00000000e-4 Ry/Bohr
  pressure threshold  : 1.00000000e-2 kbar
### Geometry Evaluation 1 (vc-relax)
#### Start SCF
context : vc-relax evaluation=1
Step time: root-local electronic iteration; report write/flush excluded; not MPI rank-max.
| Iteration |      Total energy (Ry) |     Energy change (Ry) |    SCF accuracy (Ry) |     Step time (s) |
|-----------|------------------------|------------------------|----------------------|-------------------|
|         1 |      -9.343754725553e1 |                     -- |        6.16839269e-2 |          0.330221 |
|         2 |      -9.344016199113e1 |     -2.614735598144e-3 |        2.31986631e-3 |          0.091243 |
|         3 |      -9.344022113816e1 |     -5.914703577048e-5 |        5.30395003e-5 |          0.095538 |
|         4 |      -9.344023693141e1 |     -1.579324822387e-5 |        1.29604758e-7 |          0.118108 |
|         5 |      -9.344023709934e1 |     -1.679263590404e-7 |        6.58535448e-9 |          0.110852 |
SCF electronic loop finished: converged after 5 iterations

VC Relax evaluation 1: initial (accepted steps=0)
  energy             : -9.344023709934e1 Ry
  enthalpy           : -9.344023709934e1 Ry
  enthalpy change    : --
  maximum force      : 0.00000000e0 Ry/Bohr
  pressure error     : 5.71789392e0 kbar
  volume             : 2.75848751e2 Bohr^3
  displacement norm  : 0.00000000e0 Bohr
  cell/ionic converged: no
### Geometry Evaluation 2 (vc-relax)
#### Start SCF
context : vc-relax evaluation=2
Step time: root-local electronic iteration; report write/flush excluded; not MPI rank-max.
| Iteration |      Total energy (Ry) |     Energy change (Ry) |    SCF accuracy (Ry) |     Step time (s) |
|-----------|------------------------|------------------------|----------------------|-------------------|
|         1 |      -9.344028236203e1 |                     -- |        1.78579847e-6 |          0.492117 |
|         2 |      -9.344027169442e1 |      1.066761403479e-5 |        1.47087151e-6 |          0.102051 |
|         3 |      -9.344026151869e1 |      1.017572759565e-5 |        6.44282702e-7 |          0.090806 |
|         4 |      -9.344026138839e1 |      1.303016290422e-7 |        4.40542455e-8 |          0.107016 |
|         5 |      -9.344026113632e1 |      2.520734199152e-7 |        1.56383239e-8 |          0.100938 |
SCF electronic loop finished: converged after 5 iterations

VC Relax evaluation 2: accepted (accepted steps=1)
  energy             : -9.344026113632e1 Ry
  enthalpy           : -9.344026113632e1 Ry
  enthalpy change    : 2.40369805e-5 Ry
  maximum force      : 0.00000000e0 Ry/Bohr
  pressure error     : 3.18285489e0 kbar
  volume             : 2.76653690e2 Bohr^3
  displacement norm  : 3.22785327e-3 Bohr
  cell/ionic converged: no
### Geometry Evaluation 3 (vc-relax)
#### Start SCF
context : vc-relax evaluation=3
Step time: root-local electronic iteration; report write/flush excluded; not MPI rank-max.
| Iteration |      Total energy (Ry) |     Energy change (Ry) |    SCF accuracy (Ry) |     Step time (s) |
|-----------|------------------------|------------------------|----------------------|-------------------|
|         1 |      -9.344028864694e1 |                     -- |        2.02862924e-6 |          0.407142 |
|         2 |      -9.344027800163e1 |      1.064530749773e-5 |        1.36217581e-6 |          0.097637 |
|         3 |      -9.344026920668e1 |      8.794944491797e-6 |        5.80836048e-7 |          0.092522 |
|         4 |      -9.344026883867e1 |      3.680149234242e-7 |        7.87884224e-8 |          0.103042 |
|         5 |      -9.344026821180e1 |      6.268671910448e-7 |        3.90726029e-8 |          0.094277 |
|         6 |      -9.344026820523e1 |      6.566736487912e-9 |       4.36122660e-10 |          0.098705 |
SCF electronic loop finished: converged after 6 iterations

VC Relax evaluation 3: accepted (accepted steps=2)
  energy             : -9.344026820523e1 Ry
  enthalpy           : -9.344026820523e1 Ry
  enthalpy change    : 7.06891791e-6 Ry
  maximum force      : 0.00000000e0 Ry/Bohr
  pressure error     : 1.59156351e0 kbar
  volume             : 2.77103308e2 Bohr^3
  displacement norm  : 1.80114661e-3 Bohr
  cell/ionic converged: no
### Geometry Evaluation 4 (vc-relax)
#### Start SCF
context : vc-relax evaluation=4
Step time: root-local electronic iteration; report write/flush excluded; not MPI rank-max.
| Iteration |      Total energy (Ry) |     Energy change (Ry) |    SCF accuracy (Ry) |     Step time (s) |
|-----------|------------------------|------------------------|----------------------|-------------------|
|         1 |      -9.344029002926e1 |                     -- |        2.50452946e-6 |          0.389542 |
|         2 |      -9.344027904794e1 |      1.098131876631e-5 |        1.30641195e-6 |          0.096386 |
|         3 |      -9.344027185469e1 |      7.193242780090e-6 |        5.26268791e-7 |          0.088251 |
|         4 |      -9.344027144482e1 |      4.098764350147e-7 |        1.25971697e-7 |          0.102572 |
|         5 |      -9.344027017835e1 |      1.266463243610e-6 |        8.16447716e-8 |          0.091649 |
|         6 |      -9.344027007592e1 |      1.024368998515e-7 |        5.64009456e-9 |          0.092263 |
SCF electronic loop finished: converged after 6 iterations

VC Relax evaluation 4: accepted (accepted steps=3)
  energy             : -9.344027007592e1 Ry
  enthalpy           : -9.344027007592e1 Ry
  enthalpy change    : 1.87068350e-6 Ry
  maximum force      : 0.00000000e0 Ry/Bohr
  pressure error     : 9.06198603e-1 kbar
  volume             : 2.77328562e2 Bohr^3
  displacement norm  : 9.01869922e-4 Bohr
  cell/ionic converged: no
### Geometry Evaluation 5 (vc-relax)
#### Start SCF
context : vc-relax evaluation=5
Step time: root-local electronic iteration; report write/flush excluded; not MPI rank-max.
| Iteration |      Total energy (Ry) |     Energy change (Ry) |    SCF accuracy (Ry) |     Step time (s) |
|-----------|------------------------|------------------------|----------------------|-------------------|
|         1 |      -9.344029036069e1 |                     -- |        2.71816767e-6 |          0.381475 |
|         2 |      -9.344027928768e1 |      1.107301869752e-5 |        1.28012272e-6 |          0.096271 |
|         3 |      -9.344027302203e1 |      6.265644884706e-6 |        5.07987077e-7 |          0.195079 |
|         4 |      -9.344027261414e1 |      4.078913491412e-7 |        1.60024279e-7 |          0.100336 |
|         5 |      -9.344027092808e1 |      1.686063725970e-6 |        1.16898794e-7 |          0.086464 |
|         6 |      -9.344027062367e1 |      3.044041534395e-7 |        1.70068672e-8 |          0.091822 |
SCF electronic loop finished: converged after 6 iterations

VC Relax evaluation 5: accepted (accepted steps=4)
  energy             : -9.344027062367e1 Ry
  enthalpy           : -9.344027062367e1 Ry
  enthalpy change    : 5.47753785e-7 Ry
  maximum force      : 0.00000000e0 Ry/Bohr
  pressure error     : 5.38115737e-1 kbar
  volume             : 2.77456941e2 Bohr^3
  displacement norm  : 5.13851222e-4 Bohr
  cell/ionic converged: no
### Geometry Evaluation 6 (vc-relax)
#### Start SCF
context : vc-relax evaluation=6
Step time: root-local electronic iteration; report write/flush excluded; not MPI rank-max.
| Iteration |      Total energy (Ry) |     Energy change (Ry) |    SCF accuracy (Ry) |     Step time (s) |
|-----------|------------------------|------------------------|----------------------|-------------------|
|         1 |      -9.344029039727e1 |                     -- |        2.83631284e-6 |          0.386151 |
|         2 |      -9.344027928230e1 |      1.111496507633e-5 |        1.26761551e-6 |          0.096021 |
|         3 |      -9.344027366692e1 |      5.615386115210e-6 |        4.98481115e-7 |          0.093931 |
|         4 |      -9.344027325728e1 |      4.096395258557e-7 |        1.87154116e-7 |          0.101415 |
|         5 |      -9.344027144574e1 |      1.811536989749e-6 |        1.44749435e-7 |          0.086184 |
|         6 |      -9.344027095667e1 |      4.890676024161e-7 |        3.76817298e-8 |          0.092439 |
|         7 |      -9.344027077879e1 |      1.778789311402e-7 |        9.11891782e-9 |          0.085208 |
SCF electronic loop finished: converged after 7 iterations

VC Relax evaluation 6: accepted (accepted steps=5)
  energy             : -9.344027077879e1 Ry
  enthalpy           : -9.344027077879e1 Ry
  enthalpy change    : 1.55122521e-7 Ry
  maximum force      : 0.00000000e0 Ry/Bohr
  pressure error     : 2.53586182e-1 kbar
  volume             : 2.77533217e2 Bohr^3
  displacement norm  : 3.05251068e-4 Bohr
  cell/ionic converged: no
### Geometry Evaluation 7 (vc-relax)
#### Start SCF
context : vc-relax evaluation=7
Step time: root-local electronic iteration; report write/flush excluded; not MPI rank-max.
| Iteration |      Total energy (Ry) |     Energy change (Ry) |    SCF accuracy (Ry) |     Step time (s) |
|-----------|------------------------|------------------------|----------------------|-------------------|
|         1 |      -9.344029033269e1 |                     -- |        2.97198579e-6 |          0.386294 |
|         2 |      -9.344027915409e1 |      1.117860290378e-5 |        1.25806803e-6 |          0.097701 |
|         3 |      -9.344027400360e1 |      5.150492683015e-6 |        4.89055026e-7 |          0.086970 |
|         4 |      -9.344027360877e1 |      3.948261735331e-7 |        2.04266462e-7 |          0.098067 |
|         5 |      -9.344027200267e1 |      1.606103580798e-6 |        1.62998431e-7 |          0.086574 |
|         6 |      -9.344027129738e1 |      7.052846484612e-7 |        6.83528327e-8 |          0.090547 |
|         7 |      -9.344027143256e1 |     -1.351706941932e-7 |        2.66998746e-8 |          0.086004 |
|         8 |      -9.344027090276e1 |      5.297989957853e-7 |        3.45908709e-8 |          0.088551 |
|         9 |      -9.344027080682e1 |      9.593601646429e-8 |        4.14373636e-9 |          0.084665 |
SCF electronic loop finished: converged after 9 iterations

VC Relax evaluation 7: accepted (accepted steps=6)
  energy             : -9.344027080682e1 Ry
  enthalpy           : -9.344027080682e1 Ry
  enthalpy change    : 2.80259798e-8 Ry
  maximum force      : 0.00000000e0 Ry/Bohr
  pressure error     : 1.22557507e-1 kbar
  volume             : 2.77569173e2 Bohr^3
  displacement norm  : 1.43882032e-4 Bohr
  cell/ionic converged: no
### Geometry Evaluation 8 (vc-relax)
#### Start SCF
context : vc-relax evaluation=8
Step time: root-local electronic iteration; report write/flush excluded; not MPI rank-max.
| Iteration |      Total energy (Ry) |     Energy change (Ry) |    SCF accuracy (Ry) |     Step time (s) |
|-----------|------------------------|------------------------|----------------------|-------------------|
|         1 |      -9.344029030007e1 |                     -- |        3.02188826e-6 |          0.490254 |
|         2 |      -9.344027910009e1 |      1.119998282206e-5 |        1.25376560e-6 |          0.099131 |
|         3 |      -9.344027415952e1 |      4.940569610312e-6 |        4.85822073e-7 |          0.089543 |
|         4 |      -9.344027377796e1 |      3.815624722847e-7 |        2.12639427e-7 |          0.101991 |
|         5 |      -9.344027240963e1 |      1.368329037632e-6 |        1.72296617e-7 |          0.088828 |
|         6 |      -9.344027163876e1 |      7.708717220112e-7 |        9.18782015e-8 |          0.087676 |
|         7 |      -9.344027186157e1 |     -2.228096604995e-7 |        4.60720866e-8 |          0.094562 |
|         8 |      -9.344027102271e1 |      8.388612968702e-7 |        5.93485140e-8 |          0.091155 |
|         9 |      -9.344027080901e1 |      2.136951025022e-7 |        1.03342551e-8 |          0.086436 |
SCF electronic loop finished: converged after 9 iterations

VC Relax evaluation 8: accepted (accepted steps=7)
  energy             : -9.344027080901e1 Ry
  enthalpy           : -9.344027080901e1 Ry
  enthalpy change    : 2.18990692e-9 Ry
  maximum force      : 0.00000000e0 Ry/Bohr
  pressure error     : 9.98035762e-2 kbar
  volume             : 2.77586553e2 Bohr^3
  displacement norm  : 6.95452993e-5 Bohr
  cell/ionic converged: no
### Geometry Evaluation 9 (vc-relax)
#### Start SCF
context : vc-relax evaluation=9
Step time: root-local electronic iteration; report write/flush excluded; not MPI rank-max.
| Iteration |      Total energy (Ry) |     Energy change (Ry) |    SCF accuracy (Ry) |     Step time (s) |
|-----------|------------------------|------------------------|----------------------|-------------------|
|         1 |      -9.344029029030e1 |                     -- |        3.01667427e-6 |          0.398552 |
|         2 |      -9.344027909851e1 |      1.119179040643e-5 |        1.25316404e-6 |          0.096657 |
|         3 |      -9.344027426719e1 |      4.831311841258e-6 |        4.85798497e-7 |          0.086766 |
|         4 |      -9.344027388302e1 |      3.841717841624e-7 |        2.18836637e-7 |          0.099382 |
|         5 |      -9.344027258754e1 |      1.295484040043e-6 |        1.78425427e-7 |          0.090413 |
|         6 |      -9.344027181012e1 |      7.774161474572e-7 |        1.02328527e-7 |          0.088442 |
|         7 |      -9.344027209214e1 |     -2.820146818294e-7 |        5.60119157e-8 |          0.090543 |
|         8 |      -9.344027109511e1 |      9.970233918466e-7 |        7.28779399e-8 |          0.094348 |
|         9 |      -9.344027080601e1 |      2.891002139904e-7 |        1.44223579e-8 |          0.085516 |
SCF electronic loop finished: converged after 9 iterations

VC Relax evaluation 9: accepted (accepted steps=8)
  energy             : -9.344027080601e1 Ry
  enthalpy           : -9.344027080601e1 Ry
  enthalpy change    : 2.99648661e-9 Ry
  maximum force      : 0.00000000e0 Ry/Bohr
  pressure error     : 7.04668310e-2 kbar
  volume             : 2.77600707e2 Bohr^3
  displacement norm  : 5.66365288e-5 Bohr
  cell/ionic converged: no
### Geometry Evaluation 10 (vc-relax)
#### Start SCF
context : vc-relax evaluation=10
Step time: root-local electronic iteration; report write/flush excluded; not MPI rank-max.
| Iteration |      Total energy (Ry) |     Energy change (Ry) |    SCF accuracy (Ry) |     Step time (s) |
|-----------|------------------------|------------------------|----------------------|-------------------|
|         1 |      -9.344029027649e1 |                     -- |        3.02194719e-6 |          0.378643 |
|         2 |      -9.344027908544e1 |      1.119105343150e-5 |        1.25219266e-6 |          0.092084 |
|         3 |      -9.344027434815e1 |      4.737287000012e-6 |        4.85371143e-7 |          0.083666 |
|         4 |      -9.344027396315e1 |      3.849957153079e-7 |        2.23568369e-7 |          0.097513 |
|         5 |      -9.344027273901e1 |      1.224147212042e-6 |        1.83193923e-7 |          0.084098 |
|         6 |      -9.344027199767e1 |      7.413356115649e-7 |        1.11356656e-7 |          0.084715 |
|         7 |      -9.344027235143e1 |     -3.537609245541e-7 |        6.71057122e-8 |          0.082398 |
|         8 |      -9.344027121903e1 |      1.132398026016e-6 |        8.84035655e-8 |          0.085811 |
|         9 |      -9.344027098143e1 |      2.376049792474e-7 |        2.15313673e-8 |          0.086236 |
|        10 |      -9.344027080306e1 |      1.783642744613e-7 |        8.90736179e-9 |          0.077817 |
SCF electronic loop finished: converged after 10 iterations

VC Relax evaluation 10: accepted (accepted steps=9)
  energy             : -9.344027080306e1 Ry
  enthalpy           : -9.344027080306e1 Ry
  enthalpy change    : 2.95038660e-9 Ry
  maximum force      : 0.00000000e0 Ry/Bohr
  pressure error     : 8.41320247e-3 kbar
  volume             : 2.77610702e2 Bohr^3
  displacement norm  : 3.99902132e-5 Bohr
  cell/ionic converged: yes
VC Relax cell/ionic loop finished: converged after 10 evaluations / 9 accepted steps
## Job Execution Results
ARES VC Relax
calculation : vc-relax
input      : ares.toml
topology   : p4 / b1 / g1 / threads1
status     : converged
evaluations: 10
accepted   : 9
cell trajectory (Ry, Ry/Bohr, kbar, Bohr, Bohr^3):
  eval accepted state        energy       enthalpy        delta_H       max_force   pressure_err      step_norm          volume
     1        0 initial     -9.344024e1    -9.344024e1             --     0.000000e0     5.717894e0     0.000000e0     2.7584875e2
          0.0000000000e0     5.1667051190e0     5.1667051190e0
          5.1667051190e0     0.0000000000e0     5.1667051190e0
          5.1667051190e0     5.1667051190e0     0.0000000000e0
     2        1 accepted    -9.344026e1    -9.344026e1  2.40369805e-5     0.000000e0     3.182855e0    3.227853e-3     2.7665369e2
          0.0000000000e0     5.1717257921e0     5.1717257921e0
          5.1717257921e0     0.0000000000e0     5.1717257921e0
          5.1717257921e0     5.1717257921e0     0.0000000000e0
     3        2 accepted    -9.344027e1    -9.344027e1  7.06891791e-6     0.000000e0     1.591564e0    1.801147e-3     2.7710331e2
          0.0000000000e0     5.1745259746e0     5.1745259746e0
          5.1745259746e0     0.0000000000e0     5.1745259746e0
          5.1745259746e0     5.1745259746e0     0.0000000000e0
     4        3 accepted    -9.344027e1    -9.344027e1  1.87068350e-6     0.000000e0    9.061986e-1    9.018699e-4     2.7732856e2
          0.0000000000e0     5.1759277022e0     5.1759277022e0
          5.1759277022e0     0.0000000000e0     5.1759277022e0
          5.1759277022e0     5.1759277022e0     0.0000000000e0
     5        4 accepted    -9.344027e1    -9.344027e1  5.47753785e-7     0.000000e0    5.381157e-1    5.138512e-4     2.7745694e2
          0.0000000000e0     5.1767262452e0     5.1767262452e0
          5.1767262452e0     0.0000000000e0     5.1767262452e0
          5.1767262452e0     5.1767262452e0     0.0000000000e0
     6        5 accepted    -9.344027e1    -9.344027e1  1.55122521e-7     0.000000e0    2.535862e-1    3.052511e-4     2.7753322e2
          0.0000000000e0     5.1772005795e0     5.1772005795e0
          5.1772005795e0     0.0000000000e0     5.1772005795e0
          5.1772005795e0     5.1772005795e0     0.0000000000e0
     7        6 accepted    -9.344027e1    -9.344027e1  2.80259798e-8     0.000000e0    1.225575e-1    1.438820e-4     2.7756917e2
          0.0000000000e0     5.1774241498e0     5.1774241498e0
          5.1774241498e0     0.0000000000e0     5.1774241498e0
          5.1774241498e0     5.1774241498e0     0.0000000000e0
     8        7 accepted    -9.344027e1    -9.344027e1  2.18990692e-9     0.000000e0    9.980358e-2    6.954530e-5     2.7758655e2
          0.0000000000e0     5.1775322101e0     5.1775322101e0
          5.1775322101e0     0.0000000000e0     5.1775322101e0
          5.1775322101e0     5.1775322101e0     0.0000000000e0
     9        8 accepted    -9.344027e1    -9.344027e1  2.99648661e-9     0.000000e0    7.046683e-2    5.663653e-5     2.7760071e2
          0.0000000000e0     5.1776202116e0     5.1776202116e0
          5.1776202116e0     0.0000000000e0     5.1776202116e0
          5.1776202116e0     5.1776202116e0     0.0000000000e0
    10        9 accepted    -9.344027e1    -9.344027e1  2.95038660e-9     0.000000e0    8.413202e-3    3.999021e-5     2.7761070e2
          0.0000000000e0     5.1776823476e0     5.1776823476e0
          5.1776823476e0     0.0000000000e0     5.1776823476e0
          5.1776823476e0     5.1776823476e0     0.0000000000e0
final energy        : -9.344027080306e1 Ry
final enthalpy      : -9.344027080306e1 Ry
final max force: 0.000000000000e0 Ry/Bohr
final volume        : 2.776107018710e2 Bohr^3
final pressure error: 8.413202468952e-3 kbar
final stress (Cartesian kbar):
| Component | x | y | z |
|---|---|---|---|
| x |    8.4132024690e-3 |     0.0000000000e0 |     0.0000000000e0 |
| y |     0.0000000000e0 |    8.4132024689e-3 |     0.0000000000e0 |
| z |     0.0000000000e0 |     0.0000000000e0 |    8.4132024689e-3 |
final cell (Bohr):
      0.0000000000e0     5.1776823476e0     5.1776823476e0
      5.1776823476e0     0.0000000000e0     5.1776823476e0
      5.1776823476e0     5.1776823476e0     0.0000000000e0
final positions (crystal):
  Si       0.0000000000e0     0.0000000000e0     0.0000000000e0
  Si      2.5000000000e-1    2.5000000000e-1    2.5000000000e-1
Fermi energy: 4.531282157318e-1 Ry
electronic state: /public/home/ares059/ares/dft/practice/relax/../out/si.save
final structure : /public/home/ares059/ares/dft/practice/relax/../out/si.final.cell

## Job Statistics