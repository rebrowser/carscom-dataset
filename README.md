# Cars.com Vehicle Listings Dataset

![Updated](https://img.shields.io/badge/updated-2026--11--26-brightgreen?style=flat-square)&nbsp;![Records](https://img.shields.io/badge/records-11.0M-blue?style=flat-square)&nbsp;[![Rebrowser](https://img.shields.io/badge/full%20dataset-rebrowser.net-orange?style=flat-square)](https://rebrowser.net/products/datasets/carscom)

Daily sample of Cars.com vehicle listings with make, model, trim, mileage, body style, drivetrain, and dealer location across new and used inventory.


This repository contains a preview sample of the [Cars.com dataset](https://rebrowser.net/products/datasets/carscom) published by Rebrowser. If you're doing academic research, you may be eligible for free access to a much larger slice — see [Free Datasets for Research](https://rebrowser.net/free-datasets-for-research).


This dataset contains **1** entity, each in its own folder: Car Listings (`car-listings`). See below for a full field breakdown, sample counts, and data distributions for each.

*Found this useful? ⭐ Star this repo to help us keep publishing fresh data. Found an error? [Let us know](https://rebrowser.net/contact-us).*


---

### Car Listings
Sample of Cars.com vehicle listings with year, make, model, trim, mileage, body style, drivetrain, fuel type, and dealer location.




> **10,959,564** total records from 2025-11-16 to 2026-11-22, **up to 30,000** rows in this sample (0.27% of full dataset).
> Exported as one file per day, up to 1,000 rows each, last 30 days retained.

![Data Growth](car-listings/chart-growth.svg)

| Field | Type | Fill Rate | Description |
| --- | --- | --- | --- |
| `_primaryKey` | `string` | 100% | Unique identifier for this record |
| `_firstSeenAt` | `datetime` | 100% | First time this record was seen |
| `_lastSeenAt` | `datetime` | 100% | Last time this record was updated |
| `listingId` | `string` | 100% | Unique Cars.com listing UUID (e.g., 62a9e175-556a-49da-b18e-e2ac95ef83ba) |
| `vin` 🔒 | `string` | 100% | Vehicle Identification Number (17-character unique code) |
| `stockType` | `string` | 100% | Listing type (New, Used, Certified) |
| `year` | `float` | 100% | Vehicle model year |
| `make` | `string` | 100% | Vehicle manufacturer (e.g., Mazda, Audi, Toyota) |
| `model` | `string` | 100% | Vehicle model name (e.g., CX-5, Q5, Camry) |
| `trim` | `string` | 98% | Vehicle trim level (e.g., 2.5 S Preferred Package, Premium Plus 45 TFSI) |
| `price` 🔒 | `float` | 100% | Listed price in USD |
| `msrp` 🔒 | `float` | 41% | Manufacturer suggested retail price in USD |
| `mileage` | `float` | 99% | Odometer reading in miles |
| `bodyStyle` | `string` | 100% | Body style (Sedan, SUV, Coupe, Hatchback, Truck, etc.) |
| `exteriorColor` | `string` | 98% | Exterior color (e.g., Black, White, Silver) |
| `interiorColor` | `string` | 97% | Interior color (e.g., Black Leather, Beige) |
| `drivetrain` | `string` | 98% | Drivetrain type (e.g., All-wheel Drive, Front-wheel Drive, Four-wheel Drive, Rear-wheel Drive, FWD, AWD) |
| `transmission` | `string` | 1% | Transmission type (e.g., Automatic, Manual) |
| `engine` | `string` | 1% | Engine description (e.g., SKYACTIV-G 2.5L I-4) |
| `fuelType` | `string` | 98% | Fuel type (e.g., Gasoline, Hybrid, E85 Flex Fuel, Diesel) |
| `mpg` | `string` | 1% | EPA mileage rating range (e.g., 26-30) |
| `stockNumber` | `string` | 1% | Dealer stock number |
| `sellerType` | `string` | 100% | Seller type (e.g., dealership) |
| `sellerName` 🔒 | `string` | 99% | Seller/dealer name (e.g., Liberty Mazda, Audi Richmond) |
| `sellerCity` | `string` | 99% | Seller city location |
| `sellerState` | `string` | 99% | Seller state abbreviation (e.g., CT, VA) |
| `images` 🔒 | `array` | 46% | Array of all listing photo URLs |
| `imagesCount` | `float` | 46% | Number of listing images |
| `options` | `array` | 1% | Array of vehicle options (e.g., Adaptive Cruise Control, Heated Seats, Bluetooth) |
| `optionsCount` | `float` | 1% | Number of vehicle options |
| `description` | `string` | 1% | Seller description/notes about the vehicle |
| `listingUrl` 🔒 | `string` | 100% | Full URL to the Cars.com vehicle listing page |



> 🔒 **Premium fields** are included in the data files but their values are replaced with `[PREMIUM]`. To access real values, [use our website](https://rebrowser.net/products/datasets/carscom).



#### Field Distributions


<details>
<summary><strong>Stock Type (New/Used/Certified)</strong> (<code>stockType</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| Used | 6,787,500 | `████████████░░░░░░░░` 61.9% |
| New | 4,172,064 | `████████░░░░░░░░░░░░` 38.1% |

</details>


<details>
<summary><strong>Body Style Distribution</strong> (<code>bodyStyle</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| SUV | 6,020,268 | `███████████░░░░░░░░░` 55.1% |
| Truck | 2,090,877 | `████░░░░░░░░░░░░░░░░` 19.1% |
| Sedan | 1,759,871 | `███░░░░░░░░░░░░░░░░░` 16.1% |
| Hatchback | 302,913 | `█░░░░░░░░░░░░░░░░░░░` 2.8% |
| Coupe | 260,729 | `░░░░░░░░░░░░░░░░░░░░` 2.4% |
| Passenger Van | 173,151 | `░░░░░░░░░░░░░░░░░░░░` 1.6% |
| Convertible | 135,474 | `░░░░░░░░░░░░░░░░░░░░` 1.2% |
| Cargo Van | 104,159 | `░░░░░░░░░░░░░░░░░░░░` 1.0% |
| Wagon | 43,235 | `░░░░░░░░░░░░░░░░░░░░` 0.4% |
| Minivan | 42,877 | `░░░░░░░░░░░░░░░░░░░░` 0.4% |

</details>


<details>
<summary><strong>Top Vehicle Makes</strong> (<code>make</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| Ford | 1,365,592 | `████░░░░░░░░░░░░░░░░` 18.1% |
| Chevrolet | 1,162,138 | `███░░░░░░░░░░░░░░░░░` 15.4% |
| Toyota | 1,099,474 | `███░░░░░░░░░░░░░░░░░` 14.6% |
| Honda | 757,481 | `██░░░░░░░░░░░░░░░░░░` 10.0% |
| Nissan | 625,021 | `██░░░░░░░░░░░░░░░░░░` 8.3% |
| Jeep | 555,379 | `█░░░░░░░░░░░░░░░░░░░` 7.4% |
| Kia | 553,169 | `█░░░░░░░░░░░░░░░░░░░` 7.3% |
| Hyundai | 552,620 | `█░░░░░░░░░░░░░░░░░░░` 7.3% |
| GMC | 478,034 | `█░░░░░░░░░░░░░░░░░░░` 6.3% |
| BMW | 405,429 | `█░░░░░░░░░░░░░░░░░░░` 5.4% |

</details>


<details>
<summary><strong>Fuel Type Distribution</strong> (<code>fuelType</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| Gasoline | 9,106,409 | `█████████████████░░░` 85.2% |
| Hybrid | 616,463 | `█░░░░░░░░░░░░░░░░░░░` 5.8% |
| Diesel | 414,253 | `█░░░░░░░░░░░░░░░░░░░` 3.9% |
| Electric | 344,197 | `█░░░░░░░░░░░░░░░░░░░` 3.2% |
| E85 Flex Fuel | 114,074 | `░░░░░░░░░░░░░░░░░░░░` 1.1% |
| Gas | 36,597 | `░░░░░░░░░░░░░░░░░░░░` 0.3% |
| Regular gasoline | 21,674 | `░░░░░░░░░░░░░░░░░░░░` 0.2% |
| Plug-In Hybrid | 18,345 | `░░░░░░░░░░░░░░░░░░░░` 0.2% |
| Regular unleaded | 10,777 | `░░░░░░░░░░░░░░░░░░░░` 0.1% |
| Premium gasoline | 8,186 | `░░░░░░░░░░░░░░░░░░░░` 0.1% |

</details>


<details>
<summary><strong>Listings by State</strong> (<code>sellerState</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| TX | 1,109,156 | `████░░░░░░░░░░░░░░░░` 18.5% |
| FL | 1,073,748 | `████░░░░░░░░░░░░░░░░` 17.9% |
| CA | 1,027,329 | `███░░░░░░░░░░░░░░░░░` 17.2% |
| OH | 501,681 | `██░░░░░░░░░░░░░░░░░░` 8.4% |
| IL | 497,346 | `██░░░░░░░░░░░░░░░░░░` 8.3% |
| NY | 374,525 | `█░░░░░░░░░░░░░░░░░░░` 6.3% |
| GA | 363,651 | `█░░░░░░░░░░░░░░░░░░░` 6.1% |
| NC | 361,396 | `█░░░░░░░░░░░░░░░░░░░` 6.0% |
| VA | 341,348 | `█░░░░░░░░░░░░░░░░░░░` 5.7% |
| PA | 335,870 | `█░░░░░░░░░░░░░░░░░░░` 5.6% |

</details>






---

## Pre-built Views on Rebrowser

Rebrowser web viewer lets you filter, sort, and export any slice of this dataset interactively. These pre-built views are ready to open:


### Car Listings


[Vehicle Listings with Pricing](https://rebrowser.net/products/datasets/carscom/car-listings/views/listings-with-pricing) — 10,486,983 records

↳ `[{"field":"price","op":"gt","value":0},{"sort":"price ASC"}]`

[New Vehicle Listings](https://rebrowser.net/products/datasets/carscom/car-listings/views/new-vehicle-listings) — 4,011,183 records

↳ `[{"field":"stockType","op":"is","value":"New"},{"sort":"price ASC"}]`

[Used Vehicle Listings](https://rebrowser.net/products/datasets/carscom/car-listings/views/used-vehicle-listings) — 6,485,850 records

↳ `[{"field":"stockType","op":"is","value":"Used"},{"sort":"price ASC"}]`

[Listings with Multiple Photos](https://rebrowser.net/products/datasets/carscom/car-listings/views/listings-with-photos) — 4,076,138 records

↳ `[{"field":"imagesCount","op":"gt","value":5},{"sort":"imagesCount DESC"}]`

[SUV Listings](https://rebrowser.net/products/datasets/carscom/car-listings/views/suv-listings) — 5,758,747 records

↳ `[{"field":"bodyStyle","op":"is","value":"SUV"},{"sort":"price ASC"}]`


*[See all 34 views →](https://rebrowser.net/products/datasets/carscom/car-listings)*




---

## Code Examples

```python
import pandas as pd
from pathlib import Path

# ── Car Listings ─────────────────────────────────────────────────────────────
files = sorted(Path('rebrowser/carscom-dataset/car-listings/data').glob('*.parquet'))[-7:]
listings = pd.concat([pd.read_parquet(f) for f in files])

# Top 15 makes by listing count
print(listings['make'].value_counts().head(15).to_string())

# Body style breakdown for used vehicles
used = listings[listings['stockType'] == 'Used']
print(used['bodyStyle'].value_counts().to_string())

# Average mileage by body style for used cars
print(used.groupby('bodyStyle')['mileage'].mean().sort_values().to_string())

# States with the most listings
print(listings['sellerState'].value_counts().head(10).to_string())

# Fuel type distribution across all listings
print(listings['fuelType'].value_counts().to_string())

# Listings per model year (most recent years)
print(listings['year'].value_counts().sort_index(ascending=False).head(10).to_string())
```

---

## Use Cases


### Inventory Composition Analysis

Group listings by body style, drivetrain, and fuel type to understand how dealer inventory is distributed across vehicle segments and regions.


### Regional Market Comparison

Filter by seller state to compare which makes and models dominate specific geographic markets. Identify regional preferences like truck-heavy states vs sedan markets.


### Vehicle Specification Trends

Analyze how trim levels, drivetrain types, and fuel options shift across model years. Track the growth of hybrid and electric listings relative to gasoline.


### Listing Quality Benchmarking

Compare image counts and option detail completeness across listings to benchmark what constitutes a high-quality vehicle listing on Cars.com.



---

## Full Dataset on Rebrowser


This repo is a 1,000-row preview sample. The full dataset is at [rebrowser.net/products/datasets/carscom](https://rebrowser.net/products/datasets/carscom)

Doing academic research? You may qualify for free access to a larger slice. See [Free Datasets for Research](https://rebrowser.net/free-datasets-for-research).

On Rebrowser you can:
- **Filter before you buy** — use the web UI to apply documented filters and sortable columns. Preview results before purchasing; paid exports freeze their exact selected identities before billing.
- **Export in your format** — CSV, JSON, JSONL, or Parquet depending on your plan.
- **Access via API** — integrate dataset queries into your pipelines and workflows.
- **Choose your freshness** — plans range from a 14-day lag to real-time data with no delay.
- **Select only the fields you need** — keep exports lean. Premium fields with richer data are available on higher plans.

[Pricing](https://rebrowser.net/pricing) starts at **$2 per 1,000 rows** with volume discounts.

---

## License & Terms

**Free for research and non-commercial use** with attribution. See [license terms](https://rebrowser.net/free-datasets-for-research#license) and [how to cite](https://rebrowser.net/free-datasets-for-research#citation).

```bibtex
@misc{rebrowser_carscom,
  author       = {Rebrowser},
  title        = {Cars.com Vehicle Listings Dataset},
  year         = {2026},
  howpublished = {\url{https://rebrowser.net/products/datasets/carscom}},
  note         = {Accessed: YYYY-MM-DD}
}
```

Commercial use requires a paid license — see [pricing](https://rebrowser.net/pricing). Use of this data is governed by the [Rebrowser Terms of Use](https://rebrowser.net/terms-of-use), which may be updated at any time independently of this repository.

---

## Disclaimer

Rebrowser is an independent data provider and is not affiliated with, endorsed by, or sponsored by Cars.com. Any trademarks are the property of their respective owners. This dataset is compiled from publicly available information; we do not request or collect Cars.com user credentials. By using this dataset, you agree to comply with Cars.com's Terms of Service and all applicable laws and regulations. Images, logos, descriptions, and other materials included in this dataset remain the intellectual property of their respective owners and are provided solely for informational purposes. Rebrowser makes no warranties regarding the accuracy, completeness, or legality of the data and assumes no liability for how the data is used. You are solely responsible for ensuring that your use of this dataset does not infringe on the rights of any third party.


You can also find this data on [Kaggle](https://www.kaggle.com/datasets/rebrowser/carscom-dataset), [HuggingFace](https://huggingface.co/datasets/rebrowser/carscom-dataset), [Zenodo](https://doi.org/10.5281/zenodo.18716326).

