# MSc Thesis
# A Voronoi-base Algorithm for Medial Axis Extraction (Case Study: Watershed Delineation from River Networks)

<i>A thesis submitted to the Graduate Studies Office in partial fulfillment of the requirement for the degree of Master of Science in Surveying Engineering – Geospatial Information System (GIS) <br>

The Medial Axis (MA) that is unique for a given shape and is topologically equivalent to its shape is considered as the locus of the centers of circles that are tangent to shape boundary in two or more points, where all such circles are contained in shape. The MA is used in a variety of applications especially in image analysis and also it can be used in Geospatial Information System (GIS) for applications such as watershed delineation.<br>

The methods proposed for the MA extraction are classified into discrete, semi-continuous and continuous (exact); the focus of this research is on the semi-continuous methods that the shape is approximated by a set of sample points on the shape boundary and, then, the MA is extracted using these points based on different structures, say, Voronoi diagram of the sample points. The quality of the approximated MA depends, among other parameters, on the density of sample points. If sampling is sufficiently dense, the sample points carry the shape information of the curve, i.e., they can be used to reconstruct the original curve and approximate its MA.<br>

A major issue of the MA is its inherent instability under small perturbations. The MA is very sensitive to small changes of the boundary, which produce many irrelevant branches in the MA corresponding to non-significant parts of the boundary, so as two very similar shapes can have significantly different MAs. Filtering extraneous branches is a common solution to handle this issue. Some of the filtering methods work as a pre-processing step through simplifying (smoothing) the boundary before computation of the MA; The others prune the irrelevant branches of the extracted MA in a post-processing step. In general, however, the filtering methods may alter the topological or geometrical structure of the MA.<br>

This research reviews the semi-continuous methods that use Voronoi diagram to approximate the MA from sample points. Furthermore, we introduce the most commonly used methods for filtering irrelevant branches of the MA, and discuss their main issues. This investigation has led us to proposing a new MA approximation algorithm that automatically avoids irrelevant branches through labeling the sample points. The results illustrate that our method is stable, easy to implement, robust and able to handle sharp corners, even in the presence of significant noise and perturbations.<br>

For evaluating the practical usability of the proposed algorithm in GIS, this algorithm is used to delineate the watershed of the river network. The watersheds are commonly delineated from Digital Elevation Models (DEM). This approach is not efficient when an accurate DEM is not available. Furthermore, since raster-based algorithms are employed, the computations for large areas are very time consuming and even may be impractical. This research investigates delineation of the watersheds from the MA of river networks: If the river network is sampled by a set of points, the MA of the sample points provides an approximation of the catchments, whose aggregation results in the watersheds. The results indicate that the watersheds delineated using the proposed and the DEM-based methods are reasonably comparable; The proposed approach is used in a case study and the results are compared with a DEM-based method. The results of applying the proposed method indicate the overall accuracy of 96.43% and kappa coefficient of 95.67% as compared with the result of DEM-based method with the overall accuracy of 99.20% and kappa coefficient of 98.76%. <br>
