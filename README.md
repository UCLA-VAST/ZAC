# ZAC Compiler
Compilation for zoned architectures based on neutral atom arrays.
Open source under the BSD 3-Clause license.

## Logistics
- We recommend to run the compiler in a Python3 virtual environment.
- `qiskit` is used to parse QASM files and transpile circuits to the hardware-supported gates, i.e., CZ, U3.
- Install [ffmpeg](https://www.ffmpeg.org) for animation generation

## Repo structure
- `run.py` is an example of using the compiler on a circuit. Refer to `python run.py -h` for options.
- `zac/` contains the source files implementing ZAC.
- `exp_setting/` is the directory containing example of experimental setting. See `exp_setting/README.md` for more inforamtion.
- `hardware_spec/` is the directory containing the example for zoned architecture specficiation. See `hardware_spec/README.md` for more inforamtion.
- `benchmark/` is the directory containing the circuit examples from QASMBench.
- `results/zac/` is the default directory for the results.
  - `results/zac/code/` contains the ZAIR files generated from compilation results.
  - `results/zac/animations/` contains animation generated from ZAIR.
  - `results/zac/fidelity/` contains fidelity estimation based on code files.

## How to use
- Run `python run.py <S>` where `<S>` is the json file for experimental setting.

## Publication
```
@inproceedings{lin2025reuse,
  title={Reuse-aware compilation for zoned quantum architectures based on neutral atoms},
  author={Lin, Wan-Hsuan and Tan, Daniel Bochen and Cong, Jason},
  booktitle={2025 IEEE International Symposium on High Performance Computer Architecture (HPCA)},
  pages={127--142},
  year={2025},
  organization={IEEE}
}
```
