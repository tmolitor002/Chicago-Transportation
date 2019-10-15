# Chicago Transportation | Taxi

**Current files in folder:**

1. **10-14-2019 Taxi_Trips.csv:** Taxi trips reported to the City of Chicago in its role as a regulatory agency.
  * **Size:**                 Approximately 57.9 GB
  * **Source:**               [City of Chicago](https://data.cityofchicago.org/Transportation/Taxi-Trips/wrvz-psew "City of Chicago")
  * **Updated:**              October 10, 2019
  * **Retrieved:**            October 15, 2019
  * **Uploaded to Github:**   October 15, 2019
  * **Description:**  Taxi trips reported to the City of Chicago in its role as a regualtory agency. To protect privacy but allow for aggregate anlyses, the Taxi ID is consistent for any given taxi medallion number but does not show the number, Census Tracts are suppressed in some cases, and time are rounded to the nearest 15 minutes. Due to the data reporting process, not all trips are reported, but the City believes that most are.
    * See <http://ditigal.cityofchicago.org/index.php/chicago-taxi-data-relaesed> for more information about this dataset and how it was created.
    * See <http://dev.cityofchicago.org/open%20data/data%20portal/2019/04/12/tnp-taxi-privacy.html> for futher discussion of the approach to privacy in this dataset.
    * See <http://dev.cityofchicago.org/open%20data/data%20portal/2019/07/01taxi-dataset-relaunch.html> for discussion of significant changes in July 2019.

**Data Structure/Field Descriptions:**

1. `10-14-2019 Taxi_Trips.csv`:

| Field Name | Alternative Field Name | Description | Type | Format/Notes |
|---------------|---------------|------------------------|--------|---------------:|
| Trip ID | trip_id | A unique identifier for the trip. | Plain Text | n/a |
| Taxi ID | taxi_id | A unique identifier for the taxi. | Plain Text | n/a |
| Trip Start Timestamp | trip_start_timestamp | When the trip started, rounded to the nearest 15 minutes. | Date & Time | MM/dd/yyyy hh:mm:ss AM/PM |
| Trip End Timestamp | trip_end_timestamp | When the trip ended, rounded to the nearest 15 minutes. | Date & Time | MM/dd/yyyy hh:mm:ss AM/PM |
| Trip Seconds | trip_seconds | Time of the trip in seconds. | Number | n/a |
| Trip Miles | trip_miles | Distance of the trip in miles. | Number | 1.23 |
| Pickup Census Tract | pickup_census_tract | The Census Tracte where the trip began. For privacy, this Census Tract is not shown for some trips. This column often will be blank for locations outside of Chicago. | Plain Text | n/a |
| Dropoff Census Tract | dropoff_census_tract | The Census Tract where the trip ended. For privacy, this Census Tract is not shown for some trips. This column often will be blank for locations outside Chicago. | Plain Text | n/a |
| Pickup Community Area | pickup_community_area | The Community Area where the trip began. This column will be blank for locations outside Chicago | Number | n/a |
| Dropoff Community Area | dropoff_community_area | The Community Area where the trip ended. This column will be balnk for locations outside Chicago. | Number | n/a |
| Fare | fare | The fare for the trip. | Number | 123.45 |
| Tips | tips | The tip for the trip. Cash tips generally will not be recorded. | Number | 123.45 |
| Tolls | tolls | The tolls for the trip. | Number | 123.45 |
| Extras | extras | Extra charges for the trip. | Number | 123.45 |
| Trip Total | trip_total | Total cost of the trip, the total of the previous columns. | Number | 123.45 |
| Payment Type | payment_type | Type of payment for the trip. | Plain Text | n/a |
| Company | company | The taxi company. | Plain Text | n/a |
| Pickup Centroid Latitude | pickup_centroid_latitude | The latitude of the center of the pickup census tract or the community area if the census tract has been hidden for privacy. This column will be blank for locations outside Chicago. | Number | 12.345678901 |
| Pickup Centroid Longitude | pickup_centroid_longitude | The longitude of the center of the pickup census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago. | Number | 12.345678901 |
| Pickup Centroid Location | pickup_centroid_location | The latitude of the center of the pickup census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago. | Point | POINT (12.345678901 12.345678901) |
| Dropoff Centroid Latitude | dropoff_centroid_latitude | The latitude of the center of the dropoff census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago. | Number | 12.345678901 |
| Dropoff Centroid Longitude | dropoff_centroid_longitude | The longitude of the center of the dropoff census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago. | Number | 12.345678901 |
| Dropoff Centroid Location | dropoff_centroid_location | The location of the center of the dropoff census tract or the community area if the censu tract has been hidden for privacy. This column often will be blank for locations outside Chicago. | Point | POINT (12.345678901 12.345678901) |
| Community Areas | community_area | unkown | Number | n/a |
