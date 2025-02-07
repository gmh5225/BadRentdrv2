# BadRentdrv2

A vulnerable driver exploited by me (BYOVD) that is capable of terminating several EDRs and antivirus software in the market, rendering them ineffective, working for both x32 and x64.

## How does it work?

Compile targeting the legacy x32 architecture for a wider attack range.

In an elevated command prompt(Admin), use the following command line:
```
BadRentdrv2.exe <PID>
```
This will terminate the protected process without any difficulty.

Note: In this proof of concept, I have only programmed it to terminate the process using the PID. It supports other methods such as terminating by the process name and terminating the process and its child processes by the parent process name. To do this, simply make a small modification, and it will work. Please read the proof of concept code to understand.

## Tests on the most well-known security systems in the market:

#### 360 Antivirus

![360 Antivirus teste](imgs/teste_poc_360_antivirus.gif)

#### Kaspersky Antivirus

![Kaspersky Antivirus teste](imgs/teste_poc_kaspersky_antivirus.gif)

#### Avast Antivirus

![Avast Antivirus teste](imgs/teste_poc_avast_antivirus.gif)

#### AVG Antivirus

![AVG Antivirus teste](imgs/teste_poc_avg_antivirus.gif)

#### Panda Antivirus

![Panda Antivirus teste](imgs/teste_poc_panda_antivirus.gif)

#### Windows Defender

![Windows Defender teste](imgs/teste_poc_windows_defender_antivirus.gif)
