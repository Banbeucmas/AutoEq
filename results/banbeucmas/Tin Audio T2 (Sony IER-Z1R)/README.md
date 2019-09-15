# Tin Audio T2
See [usage instructions](https://github.com/jaakkopasanen/AutoEq#usage) for more options and info.

### Parametric EQs
In case of using parametric equalizer, apply preamp of **-6.9dB** and build filters manually
with these parameters. 


| Type    | Fc       |    Q | Gain    |
|:--------|:---------|:-----|:--------|
| Peaking | 58 Hz    | 0.21 | 7.0 dB  |
| Peaking | 288 Hz   | 0.51 | -6.0 dB |
| Peaking | 1658 Hz  | 1.78 | 3.0 dB  |
| Peaking | 2775 Hz  | 3.58 | -6.0 dB |
| Peaking | 5069 Hz  | 4.34 | -7.0 dB |
| Peaking | 5366 Hz  | 0.65 | 4.2 dB  |
| Peaking | 7778 Hz  | 3.91 | -1.7 dB |
| Peaking | 7819 Hz  | 3.37 | -1.3 dB |
| Peaking | 10868 Hz | 2.95 | 3.3 dB  |
| Peaking | 12160 Hz | 1.59 | -6.8 dB |

### Fixed Band EQs
In case of using fixed band (also called graphic) equalizer, apply preamp of **-7.7dB**
(if available) and set gains manually with these parameters.

| Type    | Fc       |   Q | Gain    |
|:--------|:---------|:----|:--------|
| Peaking | 31 Hz    | 1.5 | 6.1 dB  |
| Peaking | 62 Hz    | 1.5 | 5.5 dB  |
| Peaking | 125 Hz   | 1.5 | 2.9 dB  |
| Peaking | 250 Hz   | 1.5 | -2.6 dB |
| Peaking | 500 Hz   | 1.5 | -2.8 dB |
| Peaking | 1000 Hz  | 1.5 | 0.3 dB  |
| Peaking | 2000 Hz  | 1.5 | 1.6 dB  |
| Peaking | 4000 Hz  | 1.5 | -0.7 dB |
| Peaking | 8000 Hz  | 1.5 | -0.2 dB |
| Peaking | 16000 Hz | 1.5 | -2.8 dB |

### Graphs
![](https://raw.githubusercontent.com/banbeucmas/AutoEq/master/results/banbeucmas/Tin%20Audio%20T2%20(Sony%20IER-Z1R)/Tin%20Audio%20T2.png)

### Commands
```bash
python ./frequency_response.py --input_dir="oratory1990/data/inear/Tin Audio T2" --output_dir="results/banbeucmas/Tin Audio T2 (Sony IER-Z1R)" --compensation="compensation/harman_in-ear_2017-1.csv" --sound_signature="results/oratory1990/harman_in-ear_2017-1/Sony IER-Z1R/Sony IER-Z1R.csv" --parametric_eq --fixed_band_eq  --max_filters=10 --q=1.5 --fc=31,62,125,250,500,1000,2000,4000,8000,16000 --equalize
```
