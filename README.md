# README
The codes are combining the ploughmeter, seismology, runoff and velocity data together with the framework to analyse them.
Too cite the code, please go to: https://zenodo.org/badge/latestdoi/519147675

# Reference
The codes are supporting the manuscript 'The MAMMAMIA project: A multi-scale multi-method approach to
understand runoff-induced changes in the subglacial environment
and consequences for surge dynamic in Kongsvegen glacier,
Svalbard', Coline bouchayer, Ugo Nanni, Pierre-Marie Lefeuvre, John Hulth, Louise Schmidt, Jack Kohler, Francois Renard and Thomas V. Schuler. The mansucript is in prepartaion to be submitted to The Crysophere (@ Add DOI when submitted).

# The mammamia project
The data and this study have been supported by the Research Council of Norway through the project MAMMAMIA (grant no. 301837). It stands for Multi-scAle-Multi-Method Analysis of Mechanisms causing Ice Acceleration. Sliding of ice is a major player in controlling the glacier contribution to sea-level rise, yet it is poorly understood. In the research project MAMMAMIA we will conduct a Multi-method-multi-scale analysis of mechanisms causing ice acceleration.
For more information, please visit the page of the project (https://www.mn.uio.no/geo/english/research/projects/mammamia/).

# Data availability
The full data set including all the data used in the study at a 3H resolution can be found on Zenodo (DOI: 10.5281/zenodo.7648444).

# Library required:
import numpy as np,
import pandas as pd,
import matplotlib.pyplot as plt,
import scipy.optimize,
from scipy.optimize import minimize,
from numpy.random import rand,
from scipy import interpolate,
import itertools,
import time,
from scipy import signal,
import datetime,
from datetime import timedelta, date,
import xarray as xr,

# Description of the files
KGS01_spectrogram.ipynb: code to reproduce the spectrogram in the Figure E1 (Appendix E). The spectrogram is the frequency content of KSG01 (geophone at the surface of borehole)

frequency_data.ipynb: code to reproduce the figure I1 (Appendix I). It displays the frequency content of all the time series explored in this study. 

plough2Theta.ipynb: code to convert the data of the ploughmeter to force and azimuth (Figure 4d).

produce_df2122_clean.ipynb: code to combine all the data used in this study at a 3h time resoulution between the 6th June 2021 and 9th August 2022. The code is made to reproduce the Figure 4 + Figure D1

velocity_long_term.ipynb: code to produce Figure 1b showing the velocity at KNG6 from 2005 to 2022 (Credits: NPI/Jack Kohler).

work_flow_diurnal_3.ipynb: workflow to filter the data at a diurnal time scale, comparing P, R and S to Q with predictions and discriminate the events into class (Figure 8, 9, G1)

work_season_3D.ipynb: workflow to filter the data at a seasonal and 3D time scale, comparing P, R and S to Q with predictions and discriminate the events into class (Figure 5, 6, 7)
