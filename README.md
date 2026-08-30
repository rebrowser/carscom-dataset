# Cars.com Vehicle Listings Dataset

![Updated](https://img.shields.io/badge/updated-2026--08--30-brightgreen?style=flat-square)&nbsp;![Records](https://img.shields.io/badge/records-8.6M-blue?style=flat-square)&nbsp;[![Rebrowser](https://img.shields.io/badge/full%20dataset-rebrowser.net-orange?style=flat-square)](https://rebrowser.net/products/datasets/carscom)

Daily sample of Cars.com vehicle listings with make, model, trim, mileage, body style, drivetrain, and dealer location across new and used inventory.


This repository contains a preview sample of the [Cars.com dataset](https://rebrowser.net/products/datasets/carscom) published by Rebrowser. If you're doing academic research, you may be eligible for free access to a much larger slice — see [Free Datasets for Research](https://rebrowser.net/free-datasets-for-research).


This dataset contains **1** entity, each in its own folder: Car Listings (`car-listings`). See below for a full field breakdown, sample counts, and data distributions for each.

*Found this useful? ⭐ Star this repo to help us keep publishing fresh data. Found an error? [Let us know](https://rebrowser.net/contact-us).*


---

### Car Listings
Sample of Cars.com vehicle listings with year, make, model, trim, mileage, body style, drivetrain, fuel type, and dealer location.




> **8,579,870** total records from 2025-11-16 to 2026-08-23, **up to 30,000** rows in this sample (0.35% of full dataset).
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
| `msrp` 🔒 | `float` | 42% | Manufacturer suggested retail price in USD |
| `mileage` | `float` | 99% | Odometer reading in miles |
| `bodyStyle` | `string` | 100% | Body style (Sedan, SUV, Coupe, Hatchback, Truck, etc.) |
| `exteriorColor` | `string` | 99% | Exterior color (e.g., Black, White, Silver) |
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
| `images` 🔒 | `array` | 31% | Array of all listing photo URLs |
| `imagesCount` | `float` | 31% | Number of listing images |
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
| Used | 5,195,589 | `████████████░░░░░░░░` 60.6% |
| New | 3,384,281 | `████████░░░░░░░░░░░░` 39.4% |

</details>


<details>
<summary><strong>Body Style Distribution</strong> (<code>bodyStyle</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| SUV | 4,721,933 | `███████████░░░░░░░░░` 55.2% |
| Truck | 1,637,615 | `████░░░░░░░░░░░░░░░░` 19.1% |
| Sedan | 1,371,778 | `███░░░░░░░░░░░░░░░░░` 16.0% |
| Hatchback | 237,498 | `█░░░░░░░░░░░░░░░░░░░` 2.8% |
| Coupe | 201,854 | `░░░░░░░░░░░░░░░░░░░░` 2.4% |
| Passenger Van | 130,215 | `░░░░░░░░░░░░░░░░░░░░` 1.5% |
| Convertible | 104,134 | `░░░░░░░░░░░░░░░░░░░░` 1.2% |
| Cargo Van | 86,547 | `░░░░░░░░░░░░░░░░░░░░` 1.0% |
| Minivan | 33,813 | `░░░░░░░░░░░░░░░░░░░░` 0.4% |
| Wagon | 32,936 | `░░░░░░░░░░░░░░░░░░░░` 0.4% |

</details>


<details>
<summary><strong>Top Vehicle Makes</strong> (<code>make</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| Ford | 1,078,173 | `████░░░░░░░░░░░░░░░░` 18.2% |
| Chevrolet | 901,457 | `███░░░░░░░░░░░░░░░░░` 15.2% |
| Toyota | 843,708 | `███░░░░░░░░░░░░░░░░░` 14.3% |
| Honda | 588,481 | `██░░░░░░░░░░░░░░░░░░` 9.9% |
| Nissan | 487,367 | `██░░░░░░░░░░░░░░░░░░` 8.2% |
| Jeep | 448,571 | `██░░░░░░░░░░░░░░░░░░` 7.6% |
| Hyundai | 440,600 | `█░░░░░░░░░░░░░░░░░░░` 7.4% |
| Kia | 437,797 | `█░░░░░░░░░░░░░░░░░░░` 7.4% |
| GMC | 374,840 | `█░░░░░░░░░░░░░░░░░░░` 6.3% |
| BMW | 319,745 | `█░░░░░░░░░░░░░░░░░░░` 5.4% |

</details>


<details>
<summary><strong>Fuel Type Distribution</strong> (<code>fuelType</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| Gasoline | 7,171,992 | `█████████████████░░░` 85.4% |
| Hybrid | 480,453 | `█░░░░░░░░░░░░░░░░░░░` 5.7% |
| Diesel | 321,019 | `█░░░░░░░░░░░░░░░░░░░` 3.8% |
| Electric | 263,972 | `█░░░░░░░░░░░░░░░░░░░` 3.1% |
| E85 Flex Fuel | 92,548 | `░░░░░░░░░░░░░░░░░░░░` 1.1% |
| Gas | 31,075 | `░░░░░░░░░░░░░░░░░░░░` 0.4% |
| Plug-In Hybrid | 12,096 | `░░░░░░░░░░░░░░░░░░░░` 0.1% |
| Regular unleaded | 10,301 | `░░░░░░░░░░░░░░░░░░░░` 0.1% |
| Flexible Fuel | 6,181 | `░░░░░░░░░░░░░░░░░░░░` 0.1% |
| Premium unleaded | 3,690 | `░░░░░░░░░░░░░░░░░░░░` 0.0% |

</details>


<details>
<summary><strong>Listings by State</strong> (<code>sellerState</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| TX | 868,266 | `████░░░░░░░░░░░░░░░░` 18.4% |
| FL | 855,478 | `████░░░░░░░░░░░░░░░░` 18.2% |
| CA | 811,131 | `███░░░░░░░░░░░░░░░░░` 17.2% |
| OH | 397,283 | `██░░░░░░░░░░░░░░░░░░` 8.4% |
| IL | 388,374 | `██░░░░░░░░░░░░░░░░░░` 8.2% |
| NY | 295,908 | `█░░░░░░░░░░░░░░░░░░░` 6.3% |
| GA | 288,095 | `█░░░░░░░░░░░░░░░░░░░` 6.1% |
| NC | 280,073 | `█░░░░░░░░░░░░░░░░░░░` 5.9% |
| VA | 263,532 | `█░░░░░░░░░░░░░░░░░░░` 5.6% |
| NJ | 260,445 | `█░░░░░░░░░░░░░░░░░░░` 5.5% |

</details>






---

## Pre-built Views on Rebrowser

Rebrowser web viewer lets you filter, sort, and export any slice of this dataset interactively. These pre-built views are ready to open:


### Car Listings


[Vehicle Listings with Pricing](https://rebrowser.net/products/datasets/carscom/car-listings/views/listings-with-pricing) — 8,082,343 records

↳ `[{"field":"price","op":"gt","value":0},{"sort":"price ASC"}]`

[New Vehicle Listings](https://rebrowser.net/products/datasets/carscom/car-listings/views/new-vehicle-listings) — 3,242,502 records

↳ `[{"field":"stockType","op":"is","value":"New"},{"sort":"price ASC"}]`

[Used Vehicle Listings](https://rebrowser.net/products/datasets/carscom/car-listings/views/used-vehicle-listings) — 4,848,747 records

↳ `[{"field":"stockType","op":"is","value":"Used"},{"sort":"price ASC"}]`

[Listings with Multiple Photos](https://rebrowser.net/products/datasets/carscom/car-listings/views/listings-with-photos) — 1,923,217 records

↳ `[{"field":"imagesCount","op":"gt","value":5},{"sort":"imagesCount DESC"}]`

[SUV Listings](https://rebrowser.net/products/datasets/carscom/car-listings/views/suv-listings) — 4,463,983 records

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

