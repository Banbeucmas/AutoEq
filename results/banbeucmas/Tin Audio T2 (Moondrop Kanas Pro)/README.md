# Tin Audio T2
See [usage instructions](https://github.com/jaakkopasanen/AutoEq#usage) for more options and info.

### Parametric EQs
In case of using parametric equalizer, apply preamp of **-6.8dB** and build filters manually
with these parameters. 


| Type    | Fc       |    Q | Gain     |
|:--------|:---------|:-----|:---------|
| Peaking | 57 Hz    | 0.19 | 6.7 dB   |
| Peaking | 236 Hz   | 0.75 | -3.9 dB  |
| Peaking | 658 Hz   | 0.42 | -2.7 dB  |
| Peaking | 1947 Hz  | 1.19 | 6.2 dB   |
| Peaking | 4167 Hz  | 2.06 | 2.2 dB   |
| Peaking | 5263 Hz  | 2.67 | -5.2 dB  |
| Peaking | 11257 Hz | 1.46 | -11.5 dB |
| Peaking | 13616 Hz | 2.68 | 3.6 dB   |
| Peaking | 20141 Hz | 2.43 | -1.0 dB  |

### Fixed Band EQs
In case of using fixed band (also called graphic) equalizer, apply preamp of **-7.7dB**
(if available) and set gains manually with these parameters.

| Type    | Fc       |   Q | Gain    |
|:--------|:---------|:----|:--------|
| Peaking | 31 Hz    | 1.5 | 6.1 dB  |
| Peaking | 62 Hz    | 1.5 | 5.5 dB  |
| Peaking | 125 Hz   | 1.5 | 3.3 dB  |
| Peaking | 250 Hz   | 1.5 | -1.7 dB |
| Peaking | 500 Hz   | 1.5 | -2.1 dB |
| Peaking | 1000 Hz  | 1.5 | -1.4 dB |
| Peaking | 2000 Hz  | 1.5 | 5.9 dB  |
| Peaking | 4000 Hz  | 1.5 | 0.3 dB  |
| Peaking | 8000 Hz  | 1.5 | -7.7 dB |
| Peaking | 16000 Hz | 1.5 | -2.9 dB |

### Graphs
![](https://raw.githubusercontent.com/jaakkopasanen/AutoEq/master/results/banbeucmas/Tin%20Audio%20T2%20(Moondrop%20Kanas%20Pro)/Tin%20Audio%20T2.png)

### Commands
```bash
python ./frequency_response.py --input_dir="oratory1990/data/inear/Tin Audio T2" --output_dir="results/banbeucmas/Tin Audio T2 (Moondrop Kanas Pro)" --compensation="compensation/harman_in-ear_2017-1.csv" --sound_signature="results/oratory1990/harman_in-ear_2017-1/Moondrop Kanas Pro/Moondrop Kanas Pro.csv" --parametric_eq --fixed_band_eq --max_filters=10 --q=1.5 --fc=31,62,125,250,500,1000,2000,4000,8000,16000 --equalize
```bash