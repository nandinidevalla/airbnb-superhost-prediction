# 📊 Airbnb Dataset Description

This folder contains Airbnb listing data used to predict Superhost status. Each Excel file corresponds to a specific city and includes features across multiple Superhost evaluation periods.

---

## 🧠 Dataset Context

The dataset is structured around Airbnb’s Superhost certification program, which evaluates hosts quarterly based on:

1. At least 10 trips hosted
2. 90%+ response rate
3. No cancellations
4. 80%+ 5-star reviews

Each row represents a property during one of 8 Superhost evaluation periods:  
April (2017, 2018), July (2016, 2017), October (2016, 2017), January (2017, 2018)

---

## 🏷️ Key Fields

| Feature | Description |
|--------|-------------|
| `host_is_superhost_in_period` | Binary label: whether the host is a Superhost in that evaluation period |
| `rating_ave_pastYear` | Avg. host rating over the past year |
| `numReviews_pastYear` | Total reviews in past year |
| `numCancel_pastYear` | Cancellations in past year |
| `numReserv_pastYear` | Total number of reservations |
| `available_days`, `booked_days` | Future availability and bookings |
| `available_days_aveListedPrice` | Avg. listed price for available days |
| `booked_days_avePrice` | Avg. booking price for booked days |
| `revenue`, `occupancy_rate` | Revenue and occupancy KPIs |
| `Zipcode`, `Neighborhood`, `Bedrooms`, `Latitude`, `Longitude` | Property attributes and geolocation |
| `tract_*`, `zip_*` | Demographic and census-level data (race %, population, housing units, etc.) |
| `superhost_change`, `superhost_change_gain_superhost`, `superhost_change_lose_superhost` | Status transition indicators |

---

## 📁 Files Included

- `chicago_airbnb.xlsx`
- `austin_airbnb.xlsx`
- `seattle_airbnb.xlsx`
- `dallas_airbnb.xlsx`

Each file shares a common schema and is suitable for model training and cross-city comparison.

---

## 📝 Notes

- Features with prefix `prev_` indicate values from the previous evaluation period
- The `superhost_period_all` field indicates which quarter this record belongs to
- Dataset includes over 80 engineered features combining performance, listing, and neighborhood-level metrics
