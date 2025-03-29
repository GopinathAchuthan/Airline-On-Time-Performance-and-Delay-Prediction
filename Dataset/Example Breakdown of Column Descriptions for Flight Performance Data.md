**Column Descriptions for Flight Performance Data**

1. **year**: The year the data corresponds to (e.g., `2024`).

2. **month**: The month the data corresponds to, in MM format (e.g., `12` for December). Each data row represents a specific month.

3. **carrier**: The airline’s code assigned by the U.S. Department of Transportation (DOT) (e.g., `MQ` for Envoy Air).

4. **carrier_name**: The full name of the airline corresponding to the carrier code (e.g., `Envoy Air`).

5. **airport**: The airport's three-character code as assigned by the DOT (e.g., `EVV` for Evansville Regional Airport).

6. **airport_name**: The full name and location of the airport (e.g., `Evansville, IN: Evansville Regional`).

7. **arr_flights**: The total number of arrival flights to the airport during the specified month (e.g., `61.0`).

8. **arr_del15**: The number of flights delayed by 15 minutes or more during the month (e.g., `9.0`).

9. **carrier_ct**: The average delay in minutes caused by the airline carrier across all flights in the month (e.g., `1.52` minutes).

10. **weather_ct**: The average delay in minutes caused by weather conditions across all flights in the month (e.g., `1.08` minutes).

11. **nas_ct**: The average delay in minutes caused by National Air System (NAS) factors like air traffic control and airport congestion during the month (e.g., `0.56` minutes).

12. **security_ct**: The average delay in minutes caused by security-related issues (e.g., `0.0` indicating no security-related delays during the month).

13. **late_aircraft_ct**: The average delay in minutes caused by late-arriving aircraft (e.g., `5.84` minutes).

14. **arr_cancelled**: The total number of canceled flights during the month (e.g., `0.0` indicating no cancellations).

15. **arr_diverted**: The total number of diverted flights during the month (e.g., `0.0` indicating no diversions).

16. **arr_delay**: The total accumulated arrival delay in minutes for all flights during the month (e.g., `732.0` minutes).

17. **carrier_delay**: The total accumulated delay in minutes caused by the airline carrier during the month (e.g., `47.0` minutes).

18. **weather_delay**: The total accumulated delay in minutes caused by weather conditions during the month (e.g., `90.0` minutes).

19. **nas_delay**: The total accumulated delay in minutes caused by National Air System (NAS) factors during the month (e.g., `19.0` minutes).

20. **security_delay**: The total accumulated delay in minutes caused by security issues during the month (e.g., `0.0` minutes).

21. **late_aircraft_delay**: The total accumulated delay in minutes caused by late-arriving aircraft during the month (e.g., `576.0` minutes, the largest contributor to delays).

### Notes on Data:
- **Monthly Data**: Each row in the dataset represents a specific month, providing flight performance data for that period.
- **Averages for Delay Causes**: Columns like `carrier_ct`, `weather_ct`, `nas_ct`, etc., reflect average delays caused by specific factors, calculated for the entire month.
- **Cumulative Totals**: Columns like `arr_delay`, `carrier_delay`, `weather_delay`, etc., represent cumulative delay totals across all flights during the month.
- **No Cancellations or Diversions**: If columns like `arr_cancelled` and `arr_diverted` show `0.0`, it indicates no cancellations or diversions occurred during the month.
- **Total vs. Average**: The dataset tracks both total delays (e.g., `arr_delay`) and average delays (e.g., `carrier_ct`) to provide a comprehensive view of monthly flight performance.