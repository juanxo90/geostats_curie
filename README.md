# Geostatistical mapping of the depth to the bottom of magnetic sources from Mexico

This repo will take the results of the depth to the bottom of magnetic source from the paper "*Geostatistical mapping of the depth to the bottom of magnetic sources and heat flow estimations in Mexico*" and replicate the geostatistics using python insted of GSLIB. The notebooks used will shows basics statistics, normal score tranformation, variogram calculation, variogram modelling and sequential gaussian simulations. I pretend to used google colab but if is not possible to used it, the branch will run in a MSI laptop model GL-8SC under windows subsystem for linux (WSL) with 11 gb of ram, windows 11 and 6 physcal cores (I not totally sure if I can running it using the GPU).

The aeromagnetic data used and the Depth to the bottom of magnetic source calculations are available at: **J.L. Carrillo-de la Cruz, R.M. Prol-Ledesma, G. Gabriel. Geostatistical mapping of the depth to the bottom of magnetic sources and heat flow estimations in Mexico. Geothermics, 97 (2021), [Article 102225, 10.1016/j.geothermics.2021.102225](https://doi.org/10.1016/j.geothermics.2021.102225)**

The structure of the data is a .dat file that is allowed to be used in GSLIB. Coordinates are WGS84. The cols names in the file data are exlained below:
* data: File name
* 10: # of solumns
* x: position in X
* y: position in y
* FP: Fractal parameter used to calculated the top, centroid and bottom of magnetic sources.
* Zt: Top to the magnetic sources
* Zo: Centroid of the magnetic sources
* Zb: Depth to the bottom of magnetic sources
* Zt_err: Error in the top calculation
* Zo_err: Error in the centroid calculation
* Zb_err: Error in the deoth to the bottom calculation
* misfit: Misfit between the theorical and calculated spectra from magnetic data.

After this headrer the data is structured following the columns names.
