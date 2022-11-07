# MinPlot_V1.0

Information: MinPlot is a MATLAB®-based mineral formula recalculation and compositional plotting program for electron microprobe analyses (EPMA). The program offers recalculation and structural formula assignment for 15 different mineral groups: Garnet, pyroxene, olivine, amphibole, feldspar, mica, staurolite, cordierite, chlorite, chloritoid, talc, epidote, titanite, spinel, and sulfides. MinPlot is a fast and easy to use command line program and requires no prior computer programming knowledge. Percent mass fractions of oxides are loaded from datafiles and the user answers simple prompts to select mineral type, normalization scheme, and plotting options. Recalculated mineral formulas are automatically saved as output files and plots may be further manually customized by the user prior to saving. 

Loading and Saving Data: MinPlot reads data stored as text (.txt) files. The first line must contain oxide-based headers that are specific to the mineral formula to be recalculated (see Table 1 below). The headers must have capital and lowercase characters as shown in Table 1. For some phases, certain oxides are optional and will be calculated assuming a mass fraction of zero (W_j=0) if they are not included in the file read by MinPlot. MinPlot searches the header row for the column containing the appropriate header for each oxide, as a result the oxide data can be listed in any order in the input file. To start MinPlot, change the MATLAB® directory to the folder containing MinPlot and type the name of the program into the command window and hit ‘return’. When loading the data, the user is prompted to select the file in a pop-up window and, importantly, the file can be located in any folder on the user’s computer or in their network. Following calculation, the user is prompted to save their calculation. If yes, the data is automatically saved as tab delimited text files in the same directory as the source file, allowing for simplified data organization. 

<img width="758" alt="Screen Shot 2022-11-07 at 10 42 01 PM" src="https://user-images.githubusercontent.com/87534196/200421489-c8585cc9-adf4-4ea5-b261-60513d7ac4c3.png">

# Mineral Plotting Options

Garnet supergroup: Garnet (X3Y2Z3O12) calculates with the following site assignments: X = Na, Ca, Ca, Mg, Mn, Fe2+, and Y at the dodecahedral site, Y = Fe3+, Cr, Ti, and VIAl at the octahedral site, Z = Fe3+, IVAl, and Si at the tetrahedral site, and O2 at the anion site. Garnet structural formula are calculated using normalization to 8 cations and 12 oxygens (for Fe3+-estimation), or 12 oxygen basis alone (for totalFe=Fe2+). Endmember fractions are calculated using the matrix inversion method for solving systems of linear equations. The garnet endmembers considered are almandine (Xalm), spessartine (Xsps), grossular (Xgrs), pyrope (Xprp), andradite (Xadr), and uvarovite (Xuv). Plotting options for garnet include the Xalm + Xsps, Xgrs, and Xprp ternary.
