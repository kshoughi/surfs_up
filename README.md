# surfs_up
## Overview of the Analysis
The purpose of this project is to gather temperature data for the months of June and December in Oahu, in order to determine if the surf and ice cream shop business is sustainable year-round.  

## Results
1- The average temperature for the month of June is 74.94.  
2- The average temperature for the month of December is 71.04.  
3- The minimum temperature for June is 64 while the minimum temperature for December is 56.  

## Summary
Since the average temperatures for June and December are very close, it can be concluded that the surf and ice cream shop business is sustainable year-round. Additionally, the min temperatures for June and December are both close which confirms that the business is sustainable year-round.
Two other queries that can be used to further investigate the viability of the surf and ice cream shop is to check the precipitation data for the months of June and December. From the results, it can be seen that the average precipitation for these months are 0.136 and 0.217, respectively. Which shows that there is not a lot of rain and surf and ice cream shop business is sustainable year-round. The following query was used to extract precipitation data for month of June.  

``results = session.query(Measurement.prcp).\
    filter(extract('month', Measurement.date)==6).all()``  
``prc = list(np.ravel(results))  ``  
``prc_df = pd.DataFrame(prc) ``  
``prc_df.describe()``



