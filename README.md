# python-api-challenge: What’s the weather like

This analysis randomly selects 500+ unique cities based on latitude and longitude, performs a weather check on each of the cities using API calls, and checks the relationship between temperature, Humidity, Cloudiness and Wind speed with the Latitudes.
It then filters out the cities with ideal weather condition, and uses Google Places API to find the first hotel for each city located within 5000 meters.

Observable trends based on the data:


1. Overall humidity in all selected cities is more intensely distributed within 50%-100% range, cloudiness is evenly distributed between 0-100%, while wind speed focuses in the range of 0-15%.

2. The temperature gets higher as approaching the equator. This is proven by the linear regression analysis between Max Temp vs. Latitude. In Northern Hemisphere, temperature is negatively related to latitude while in Southern Hemisphere temperature is positively related to latitude.

3. All other factors- humidity, cloudiness and wind speeds have very low/no relationship with latitude, as there are more local factors that contribute to them. For these factors there are no obvious difference between Northern Hemisphere and Southern Hemisphere.

4. Cloudiness is somewhat positively related to Humidity because clouds are formed from water and ice. The higher the humidity, the more water is available to make clouds.
