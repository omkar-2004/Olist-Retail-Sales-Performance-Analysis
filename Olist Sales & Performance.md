
# 📊 Olist Retail Sales Performance Analysis

### Optimizing E-Commerce Sales Performance \& Revenue Drivers

\---



## 📂 Dataset Overview

**Dataset Name:** Brazilian E-Commerce Public Dataset by Olist  
**Source:** [Kaggle Dataset Link](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
---


## 🗄️ Database Schema \& Tables



###### Below is the structured relational schema of the Olist e-commerce dataset, comprising 9 interconnected tables:

### 

### 1\. `Customer`



|Column Name|Description|
|-|-|
|`customer\\\_id`|Key to each order (each order gets a unique customer\_id)|
|`customer\\\_unique\\\_id`|Unique identifier for the actual customer|
|`customer\\\_zip\\\_code\\\_prefix`|First 5 digits of customer zip code|
|`customer\\\_city`|Customer city name|
|`customer\\\_state`|Customer state (state abbreviation)|

### 

### 2\. `Geolocation`



|Column Name|Description|
|-|-|
|`geolocation\\\_zip\\\_code\\\_prefix`|First 5 digits of zip code|
|`geolocation\\\_lat`|Latitude coordinate|
|`geolocation\\\_lng`|Longitude coordinate|
|`geolocation\\\_city`|City name|
|`geolocation\\\_state`|State name|

### 

### 3\. `Order\\\_item`



|Column Name|Description|
|-|-|
|`order\\\_id`|Unique order identifier|
|`order\\\_item\\\_id`|Sequential number identifying items within the same order|
|`product\\\_id`|Unique product identifier|
|`seller\\\_id`|Unique seller identifier|
|`shipping\\\_limit\\\_data`|Seller shipping limit date for handling|
|`price`|Item price|
|`freight\\\_value`|Item freight value (shipping cost)|

### 

### 4\. `order\\\_payments`



|Column Name|Description|
|-|-|
|`order\\\_id`|Unique order identifier|
|`payment\\\_sequential`|Sequence of payment methods used|
|`payment\\\_type`|Method of payment (credit\_card, boleto, voucher, etc.)|
|`payment\\\_installments`|Number of installments chosen|
|`payment\\\_value`|Total amount paid|

### 

### 5\. `order\\\_reviews`



|Column Name|Description|
|-|-|
|`review\\\_id`|Unique review identifier|
|`order\\\_id`|Unique order identifier|
|`review\\\_score`|Satisfaction score from 1 to 5|
|`review\\\_comment\\\_title`|Comment title|
|`review\\\_comment\\\_message`|Review message text|
|`review\\\_creation\\\_date`|Date the review survey was sent|
|`review\\\_answer\\\_timestamp`|Date/time of survey response|

### 

### 6\. `orders`



|Column Name|Description|
|-|-|
|`order\\\_id`|Unique order identifier|
|`customer\\\_id`|Key to customer table|
|`order\\\_status`|Current status of the order|
|`order\\\_purchase\\\_timestamp`|Timestamp of the purchase|
|`order\\\_approved\\\_at`|Timestamp of payment approval|
|`order\\\_delivered\\\_carrier\\\_date`|Timestamp of handover to carrier|
|`order\\\_delivered\\\_customer\\\_date`|Actual delivery date to customer|
|`order\\\_estimated\\\_delivery\\\_date`|Estimated delivery date shown at checkout|

### 

### 7\. `products`



|Column Name|Description|
|-|-|
|`product\\\_id`|Unique product identifier|
|`product\\\_category\\\_name`|Category name in Portuguese|
|`product\\\_name\\\_lenght`|Number of characters in product name|
|`product\\\_description\\\_lenght`|Number of characters in description|
|`product\\\_photos\\\_qty`|Number of published photos|
|`product\\\_weight\\\_g`|Product weight in grams|
|`product\\\_length\\\_cm`|Product length in cm|
|`product\\\_height\\\_cm`|Product height in cm|
|`product\\\_width\\\_cm`|Product width in cm|

### 

### 8\. `sellers`



|Column Name|Description|
|-|-|
|`seller\\\_id`|Unique seller identifier|
|`seller\\\_zip\\\_code\\\_prefix`|First 5 digits of seller zip code|
|`seller\\\_city`|Seller city name|
|`seller\\\_state`|Seller state|

### 

### 9\. `product\\\_category\\\_name\\\_translation`



|Column Name|Description|
|-|-|
|`product\\\_category\\\_name`|Category name in Portuguese|
|`product\\\_category\\\_name\\\_english`|Category name translated to English|

\---
