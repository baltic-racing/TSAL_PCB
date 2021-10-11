# TSAL - Tractive System Active Light
The TSAL is an optical indicator mounted at the top of the main hoop while being protected by the rollover-envelope. The TSAL indicates the status of the TS.

The TSAL has a 24V power-input, a signal-input for each color (red, green) and a ground connection.

SCS are adhered to. The TSAL inputs are considered SCS (T11.9) class a (signals transmitted by cable) and hence need to fail in safe mode if the following erros occur:
- Open circuit
- Short circuit to ground
The safe state of the TSAL is all lights being off. The two colors are mutually exclusive. If one color shorts to ground or fails in open circuit, it wont light up causing safe mode.

The 2022 rules do *not* require measures against single points of failure causing a massive reduction of effort compared to 2019-2021.