# Cytoskeleton and Cell Morphology

**Name:** Pasculado, Mark Ryan T. 

**Date Completed:** October 22, 2026

**Phenotype:** Phospho-histone H3 dots 09339-actin; 09339-DNA

**Goal:** Download and choose your own fluorescence images of HT29 human colon-cancer cells, select one phenotype, measure five cells in Fiji, make two plots in R, and document your work on GitHub.

## Process
<img width="1901" height="857" alt="01_Fiji Downloads page with Windows x86-64 selected" src="https://github.com/user-attachments/assets/1ab5ac20-8ee9-4e57-a180-e180a8669ca5" />

**Figure 1.** Fiji ImageJ download page showing the selection of the Windows x86-64 version for installation on a Windows computer.

<img width="1500" height="492" alt="Screenshot 2026-10-21 132600" src="https://github.com/user-attachments/assets/01a5c51f-f68a-4db6-9706-886eb2a2a8f2" />

**Figure 2.** Fiji software installed and ready (fiji-latest-win64-jdk)

<img width="1918" height="1020" alt="Screenshot 2026-10-21 132754" src="https://github.com/user-attachments/assets/e34fce8e-17f3-4c11-9091-1db9ffdd07c2" />

**Figure 3.** Opening the .DIB images in Fiji with File > Import > Bio-Formats

<img width="1366" height="768" alt="Screenshot 2026-10-22 09339" src="https://github.com/user-attachments/assets/c882dd6a-4790-4dfb-a64f-81a6579482f8" />

**Figure 4.** Opening the field 09339 actin, DNA and pH3 images in Fiji (File > Open)

<img width="1002" height="1025" alt="Screenshot 2026-10-21 133456" src="https://github.com/user-attachments/assets/0366c8b0-710a-4ff8-a8c1-32b8ad9464db" />
**Figure 5.** Measuring each traced cell with Analyze > Measure

<img width="1206" height="761" alt="Screenshot 2026-10-21 133749" src="https://github.com/user-attachments/assets/b958a729-c20c-45fc-b4ac-62b3c9a59fca" />

**Figure 6.** Fiji Set Measurements: Area, Mean gray value, Shape descriptors, Display label

### Download, choose and register your OWN image

| Item | Answer |
|---|---|
| Phenotype chosen (visual classification) | Long projections |
| Image-field ID | 09339 |
| Actin filename | 09339-actin.DIB |
| DNA filename | 09339-DNA.DIB |
| Dataset page | <https://bbbc.broadinstitute.org/BBBC018> |
| Download link | <https://data.broadinstitute.org/bbbc/BBBC018/BBBC018_v1_images.zip> |
| Visible features supporting the phenotype | Several cells appear rounded, with bright actin staining around their edges and varying staining intensities. |
<img width="200" height="371" alt="PH3" src="https://github.com/user-attachments/assets/7d4c1617-ae89-44d6-884f-78e490856e18" />


**Figure 7.** BBBC018 reference example: Phospho-histone H3 dots (field 099339)
### Open your chosen fluorescence images in Fiji

<img width="522" height="562" alt="actin" src="https://github.com/user-attachments/assets/d1fff649-c636-4680-8d84-c936f7f1fa15" />

**Figure 8.** Field 09339, F-actin channel (phalloidin), before measurement

<img width="523" height="562" alt="DNA" src="https://github.com/user-attachments/assets/405c7c41-c64f-4e9a-ad9d-fa180251ba22" />


**Figure 9.** Field 09339, DNA channel (Hoechst 33342), used as a guide for locating nuclei

<img width="519" height="563" alt="PH3" src="https://github.com/user-attachments/assets/30173bc0-e8c1-486f-9d68-0ce6111d36d4" />

**Figure 10.** Field 09339, pH3 channel (phospho-histone H3), optional reference

### Measure five cells in Fiji

<img width="517" height="564" alt="5cells" src="https://github.com/user-attachments/assets/0cbdab29-4f68-4944-b625-1aedfb2da230" />


**Figure 11.** Five traced cells measured on 09339-actin.DIB (yellow outlines)

<img width="527" height="287" alt="ROI" src="https://github.com/user-attachments/assets/25ab2cc7-17ec-4cdb-b555-bfe55a88fc7d" />

**Figure 12.** ROI Manager with the five traced cells of field 09339

**Table 2.** Fiji measurements of five cells in field 09339 (09339-actin.DIB)
|   | Label                     | Area | Mean    | Min | Max  | Circ. | AR    | Round | Solidity |
|---|---------------------------|-----:|--------:|----:|-----:|------:|------:|------:|---------:|
| 1 | 09339-actin.DIB:0173-0221 | 249  | 974.442 | 411 | 1415 | 0.915 | 1.134 | 0.882 | 0.988 |
| 2 | 09339-actin.DIB:0146-0393 | 1013 | 472     | 249 | 666  | 0.919 | 1.225 | 0.816 | 0.997 |
| 3 | 09339-actin.DIB:0151-0182 | 1266 | 405.034 | 291 | 527  | 0.909 | 1.291 | 0.775 | 0.990 |
| 4 | 09339-actin.DIB:0282-0188 | 1020 | 482.995 | 306 | 732  | 0.907 | 1.082 | 0.924 | 0.986 |
| 5 | 09339-actin.DIB:0128-0205 | 1225 | 480.391 | 262 | 731  | 0.850 | 1.640 | 0.610 | 0.983 |


<img width="900" height="650" alt="actin_intensity" src="https://github.com/user-attachments/assets/361b4a30-ab15-4015-b56f-19ee32c3a29d" />

**Figure 13.** Mean actin fluorescence of the five measured cells in field 09339

<img width="900" height="650" alt="area_vs_circularity" src="https://github.com/user-attachments/assets/07c21575-fccd-417f-9645-48783b4cc613" />

**Figure 14.** Cell area versus circularity for the five measured cells in field 09339

## Explain your results

1. Which specific phenotype did you choose, and what visible features support that choice?
- I chose the phospho-histone H3 dots phenotype. The classification is based on the visual features observed in the fluorescence images and comparison with the dataset references. One major visible features is the cells orientation and arrangement of the cells, along with their shape and staining patterns.
2. Were your five cells mostly round or elongated? Refer to your circularity and aspect-ratio results.
- My five measured cells were mostly round, based on their circularity values, which ranged from 0.850 to 0.919. Their aspect ratios ranged from 1.082 to 1.640, indicating that most cells were close to a rounded shape, although the fifth cell was more elongated than the others.
3. What role does actin play in maintaining cell shape and in cell movement (Karp Chapter 9)?
- Actin filaments form a supportive network beneath the plasma membrane that maintains cell shape and enables the formation of extensions, such as protrusions and tails. During movement, actin filaments grow at the front of the cell, pushing the membrane forward. Working with myosin and cell attachments, actin helps the cell move across a surface.
4. Why can a single fixed fluorescence image NOT show how fast a cell moves?
- A single fixed fluorescence image captures cells at only one point in time. Although it reveals cell shape, orientation, and actin staining patterns, it cannot show changes in cell position over time. Live-cell imaging is needed to track cell movement and calculate speed.
## References

**Fiji (free):** <https://imagej.net/software/fiji/downloads>

**R (free):** <https://cran.r-project.org/>

**BBBC018 dataset page and phenotype examples:** <https://bbbc.broadinstitute.org/BBBC018>

**Direct download: BBBC018_v1_images.zip (46 MB):** <https://data.broadinstitute.org/bbbc/BBBC018/BBBC018_v1_images.zip>
