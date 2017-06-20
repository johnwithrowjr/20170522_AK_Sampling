
# Alaska IDS Inference Preprocessing

## Executive Summary

This discussion investigates what inferences can be made regarding total acreage of various host tree species and similar total acreage of various pest-host disturbance events throughout a set of spatial zones in Alaska, based upon data collected from a set of twenty grid squares placed as a result of a spatially distributed random sample.  Each grid square is 20 miles by 20 miles, and so represents the result of an intensive and time-consuming effort, but a level of effort which of course cannot be applied to the full area for which inference is desired.  In addition, there appears to be some uncertainty as to the central objective of the sampling process, to which it is hoped that the current investigation will elucidate areas of focus by revealing what objectives may be most achievable given the constraints of the data.

## Data Provided

GRTS_Unequalsites_n20_over20_334_PanelOne.shp - ESRI Point shape file showing 20 sample points with attribute information apparently showing total acreage for Sitka spruce (FIA spp 98), western hemlock (spp 263), Alaska cedar (42), lodgepole pine (108), quaking aspen (746), white spruce (94), and paper birch (375).  Similar totals are given for what appears to be a tree mask.

ReducedArea3b_wbm_INT_mask_20mi_gtet25percent_CoreArea_Sample_n20.shp - ESRI polygon shape file showing showing 20 squares of size 20 miles by 20 miles, each one encompassing one of the sample points in the previous file.  Difficult to discern fields in the attribute table, but one appears to show percentage forest cover.  

zones.shp - ESRI polygon shape file showing apparent zones of desired inference.

SampleListUpdated20170316.xls - Excel spreadsheet showing apparent pest-host combinations of interest to the study.

## Statistical Approach

The goal here will be to create a single flat file that shows a single record for each square zone, where percentage forest cover will be unioned with the variables in the opposite shape file.  Zonal statistics will be run on relevant host layers from Ellenwood as well as pest acreage totals from the IDS database.  Correlations will be investigated between Ellenwood host layer total acreage and acreage values reported from the sample areas.
