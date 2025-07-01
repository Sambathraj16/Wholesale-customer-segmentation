# Wholesale-customer-segmentation
The dataset refers to clients of a wholesale distributor. It includes the annual spending in monetary units (m.u.) on diverse product categories  Source: UCI Wholesale customers Data Set



Observation from clustering I have added it for easier refference, below are observed analysis after performing clustering, feel free to add your coments.

Reason: I considered this dataset for interpretation since dataset size is very less and labeling this dataset doesnt made any sense to me.

Other regions - Retail section consuming less amount of frozen(Cluster 0) and more cosumption of Detergents_paper and Grocery(High consumption is justfiable since it is retail section)
Most of sales happening in Other regions(Horeca) and the sales are very well spread but in seling Detergents_paper and Delicassen we can still focus(Cluster 1)
Sales happening in Horeca in Lisbon region and we can improve sales of Delicassen which is less than average sales of Delicassen in overall country(Cluster 3)
We can imporove sales of Retail section in Lisbon city and consumption of grocery is very high than entire sales average
Retail section dominates our Grocery Detergents_paper Milk and Delicassen sales whereas Horeca section dominates
Though milk sales in Horeca Region is less, it is justifiable since Horeca wont cosumes much milk (NA to Cafe)
Process:

I tried with minmax scaling and both standard scaler.Many features contains outliers, so i tried with some transformations . But without transformation outputs are easily intrepretable.
For scaling, I used MinMaxscaling though it is sensitive to outliers. Since i considered for intrepretation, this gave good results and good silhouette score(greater than 0.6)
Feature plan: I tried only with DBSCAN, still we can try with Hierarchial clustering or other variants of DBSCAN such as HDBSCAN, OPTICS
