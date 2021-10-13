# TSAL - Tractive System Active Light
The TSAL is an optical indicator mounted at the top of the main hoop while being protected by the rollover-envelope. The TSAL indicates the status of the TS.

The TSAL has the following pins:
- 24V power-input
- ground connection
- red and green signal inputs from the TSAC
- red signal input from the HV-Distribution
- green signal output to the Dashboard LED

SCS are adhered to. The TSAL inputs are considered SCS (T11.9) class a (signals transmitted by cable) and hence need to fail in safe mode if the following erros occur:
- Open circuit
- Short circuit to ground
The safe state of the TSAL is all lights being off. The two colors are mutually exclusive. If one color shorts to ground or fails in open circuit, it wont light up causing safe mode. Both devices needing measurement are directly connected to the TSAL. The TSAL performance additional plausibility-checks between DC-bus and TSAC voltages and states and outputs a buffered, plausibility-checked signal for the green LED in the dashboard.

The 2022 rules do *not* require measures against single points of failure causing a massive reduction of effort compared to 2019-2021.