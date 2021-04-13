```python
# Dependencies and Setup
import pandas as pd

# File to Load (Remember to Change These)
file_to_load = "Resources/purchase_data.csv"

# Read Purchasing File and store into Pandas data frame
purchase_df = pd.read_csv(file_to_load)
purchase_df.head(20)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Purchase ID</th>
      <th>SN</th>
      <th>Age</th>
      <th>Gender</th>
      <th>Item ID</th>
      <th>Item Name</th>
      <th>Price</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>Lisim78</td>
      <td>20</td>
      <td>Male</td>
      <td>108</td>
      <td>Extraction, Quickblade Of Trembling Hands</td>
      <td>3.53</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>Lisovynya38</td>
      <td>40</td>
      <td>Male</td>
      <td>143</td>
      <td>Frenzied Scimitar</td>
      <td>1.56</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>Ithergue48</td>
      <td>24</td>
      <td>Male</td>
      <td>92</td>
      <td>Final Critic</td>
      <td>4.88</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>Chamassasya86</td>
      <td>24</td>
      <td>Male</td>
      <td>100</td>
      <td>Blindscythe</td>
      <td>3.27</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>Iskosia90</td>
      <td>23</td>
      <td>Male</td>
      <td>131</td>
      <td>Fury</td>
      <td>1.44</td>
    </tr>
    <tr>
      <th>5</th>
      <td>5</td>
      <td>Yalae81</td>
      <td>22</td>
      <td>Male</td>
      <td>81</td>
      <td>Dreamkiss</td>
      <td>3.61</td>
    </tr>
    <tr>
      <th>6</th>
      <td>6</td>
      <td>Itheria73</td>
      <td>36</td>
      <td>Male</td>
      <td>169</td>
      <td>Interrogator, Blood Blade of the Queen</td>
      <td>2.18</td>
    </tr>
    <tr>
      <th>7</th>
      <td>7</td>
      <td>Iskjaskst81</td>
      <td>20</td>
      <td>Male</td>
      <td>162</td>
      <td>Abyssal Shard</td>
      <td>2.67</td>
    </tr>
    <tr>
      <th>8</th>
      <td>8</td>
      <td>Undjask33</td>
      <td>22</td>
      <td>Male</td>
      <td>21</td>
      <td>Souleater</td>
      <td>1.10</td>
    </tr>
    <tr>
      <th>9</th>
      <td>9</td>
      <td>Chanosian48</td>
      <td>35</td>
      <td>Other / Non-Disclosed</td>
      <td>136</td>
      <td>Ghastly Adamantite Protector</td>
      <td>3.58</td>
    </tr>
    <tr>
      <th>10</th>
      <td>10</td>
      <td>Inguron55</td>
      <td>23</td>
      <td>Male</td>
      <td>95</td>
      <td>Singed Onyx Warscythe</td>
      <td>4.74</td>
    </tr>
    <tr>
      <th>11</th>
      <td>11</td>
      <td>Haisrisuir60</td>
      <td>23</td>
      <td>Male</td>
      <td>162</td>
      <td>Abyssal Shard</td>
      <td>2.67</td>
    </tr>
    <tr>
      <th>12</th>
      <td>12</td>
      <td>Saelaephos52</td>
      <td>21</td>
      <td>Male</td>
      <td>116</td>
      <td>Renewed Skeletal Katana</td>
      <td>4.18</td>
    </tr>
    <tr>
      <th>13</th>
      <td>13</td>
      <td>Assjaskan73</td>
      <td>22</td>
      <td>Male</td>
      <td>4</td>
      <td>Bloodlord's Fetish</td>
      <td>1.70</td>
    </tr>
    <tr>
      <th>14</th>
      <td>14</td>
      <td>Saesrideu94</td>
      <td>35</td>
      <td>Male</td>
      <td>165</td>
      <td>Bone Crushing Silver Skewer</td>
      <td>4.86</td>
    </tr>
    <tr>
      <th>15</th>
      <td>15</td>
      <td>Lisassa64</td>
      <td>21</td>
      <td>Female</td>
      <td>98</td>
      <td>Deadline, Voice Of Subtlety</td>
      <td>2.89</td>
    </tr>
    <tr>
      <th>16</th>
      <td>16</td>
      <td>Lisirra25</td>
      <td>20</td>
      <td>Male</td>
      <td>40</td>
      <td>Second Chance</td>
      <td>2.52</td>
    </tr>
    <tr>
      <th>17</th>
      <td>17</td>
      <td>Zontibe81</td>
      <td>21</td>
      <td>Male</td>
      <td>161</td>
      <td>Devine</td>
      <td>1.76</td>
    </tr>
    <tr>
      <th>18</th>
      <td>18</td>
      <td>Reunasu60</td>
      <td>22</td>
      <td>Female</td>
      <td>82</td>
      <td>Nirvana</td>
      <td>4.90</td>
    </tr>
    <tr>
      <th>19</th>
      <td>19</td>
      <td>Chamalo71</td>
      <td>30</td>
      <td>Male</td>
      <td>89</td>
      <td>Blazefury, Protector of Delusions</td>
      <td>4.64</td>
    </tr>
  </tbody>
</table>
</div>




```python
print(purchase_df.columns)
print()
purchase_df.dtypes

# see if we have to clean any data with missing information
#purchase_df.count()
```

    Index(['Purchase ID', 'SN', 'Age', 'Gender', 'Item ID', 'Item Name', 'Price'], dtype='object')
    
    




    Purchase ID      int64
    SN              object
    Age              int64
    Gender          object
    Item ID          int64
    Item Name       object
    Price          float64
    dtype: object



## Player Count

* Display the total number of players



```python
players = len(purchase_df["SN"].unique())
total_players_df = pd.DataFrame([{"Total Players": players}])
total_players_df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Total Players</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>576</td>
    </tr>
  </tbody>
</table>
</div>



## Purchasing Analysis (Total)

* Run basic calculations to obtain number of unique items, average price, etc.


* Create a summary data frame to hold the results


* Optional: give the displayed data cleaner formatting


* Display the summary data frame



```python
#Finding total_unique_items
total_unique_items = purchase_df["Item ID"].nunique()
#total_unique_items

# Finding Average Price
ave_price = purchase_df["Price"].mean()
#ave_price

# Finding Total Purchases
total_purchases = purchase_df["Purchase ID"].count()
#total_purchases

#Finding Total Revenue
total_revenue = purchase_df["Price"].sum()
#total_revenue

#Creating the summary dataframe and fromatting
summary_df = pd.DataFrame({"Number of Unique Items": [total_unique_items],
                           "Average Price": [ave_price],
                           "Number of Purchases": [total_purchases],
                           "Total Revenue": [total_revenue]})
# mapping/formatting colums
summary_df["Average Price"] = summary_df["Average Price"].map("${:.2f}".format)
summary_df["Total Revenue"] = summary_df["Total Revenue"].map("${:.2f}".format)
summary_df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Number of Unique Items</th>
      <th>Average Price</th>
      <th>Number of Purchases</th>
      <th>Total Revenue</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>179</td>
      <td>$3.05</td>
      <td>780</td>
      <td>$2379.77</td>
    </tr>
  </tbody>
</table>
</div>



## Gender Demographics

* Percentage and Count of Male Players


* Percentage and Count of Female Players


* Percentage and Count of Other / Non-Disclosed





```python
# Reference webpage - https://stackoverflow.com/questions/64613127/pandas-count-rows-in-table-based-on-two-columns-using-one-columns-value
unique_genders_df = purchase_df.groupby(["Gender"])["SN"].nunique()
#print(unique_genders_df)

#total = unique_genders_df.sum()
#print(total)

percentage = (unique_genders_df / unique_genders_df.sum()) * 100
#print(percentage)

genders_df = pd.concat([unique_genders_df, percentage], axis=1)
genders_df.columns = ["Total Count", "Percentage of Players"]
#print(genders_df)
genders_df["Percentage of Players"] = genders_df["Percentage of Players"].map("{:.2f}%".format)
sort_genders_df = genders_df.sort_values("Total Count", ascending=False)
sort_genders_df

#final_s = pd.concat([unique_genders, percentage_df], axis=1)
#print(final_s)
#sort_final_s = final.sort_values("SN", ascending=False)
#sort_final_s.rename(columns = {"SN": "Total Count", "Gender": "Percentage of Players"}, inplace=True)
#sort_final_s["Percentage of Players"] = sort_final_s["Percentage of Players"].map("{:.2f}%".format)
#sort_final_s
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Total Count</th>
      <th>Percentage of Players</th>
    </tr>
    <tr>
      <th>Gender</th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Male</th>
      <td>484</td>
      <td>84.03%</td>
    </tr>
    <tr>
      <th>Female</th>
      <td>81</td>
      <td>14.06%</td>
    </tr>
    <tr>
      <th>Other / Non-Disclosed</th>
      <td>11</td>
      <td>1.91%</td>
    </tr>
  </tbody>
</table>
</div>




## Purchasing Analysis (Gender)

* Run basic calculations to obtain purchase count, avg. purchase price, avg. purchase total per person etc. by gender




* Create a summary data frame to hold the results


* Optional: give the displayed data cleaner formatting


* Display the summary data frame


```python
# Count number of purchase by gender
purchase_count_gender = purchase_df.groupby(["Gender"])["Item ID"].count()
#print(purchase_count_gender)

# Average purchase price by gender
avg_price_gender = purchase_df.groupby(["Gender"])["Price"].mean()
#print(avg_price_gender)

# Total price by gender
total_price_gender = purchase_df.groupby(["Gender"])["Price"].sum()
#print(total_price_gender)

# Average purchase price per person, I am using the dataframe unique_genders_df from above
avg_price_person = total_price_gender / unique_genders_df
#print(avg_price_person)

# create summary
purchase_gender_df = pd.DataFrame({"Purchase Count": purchase_count_gender,
                                   "Average Purchase Price": avg_price_gender,
                                   "Total Purchase Value": total_price_gender,
                                   "Avg Total Purchase per Person": avg_price_person})
# format
purchase_gender_df["Average Purchase Price"] = purchase_gender_df["Average Purchase Price"].map("${:,.2f}".format)
purchase_gender_df["Total Purchase Value"] = purchase_gender_df["Total Purchase Value"].map("${:,.2f}".format)
purchase_gender_df["Avg Total Purchase per Person"] = purchase_gender_df["Avg Total Purchase per Person"].map("${:,.2f}".format)
purchase_gender_df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Purchase Count</th>
      <th>Average Purchase Price</th>
      <th>Total Purchase Value</th>
      <th>Avg Total Purchase per Person</th>
    </tr>
    <tr>
      <th>Gender</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Female</th>
      <td>113</td>
      <td>$3.20</td>
      <td>$361.94</td>
      <td>$4.47</td>
    </tr>
    <tr>
      <th>Male</th>
      <td>652</td>
      <td>$3.02</td>
      <td>$1,967.64</td>
      <td>$4.07</td>
    </tr>
    <tr>
      <th>Other / Non-Disclosed</th>
      <td>15</td>
      <td>$3.35</td>
      <td>$50.19</td>
      <td>$4.56</td>
    </tr>
  </tbody>
</table>
</div>



## Age Demographics

* Establish bins for ages


* Categorize the existing players using the age bins. Hint: use pd.cut()


* Calculate the numbers and percentages by age group


* Create a summary data frame to hold the results


* Optional: round the percentage column to two decimal points


* Display Age Demographics Table



```python

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Total Count</th>
      <th>Percentage of Players</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>&lt;10</th>
      <td>17</td>
      <td>2.95%</td>
    </tr>
    <tr>
      <th>10-14</th>
      <td>22</td>
      <td>3.82%</td>
    </tr>
    <tr>
      <th>15-19</th>
      <td>107</td>
      <td>18.58%</td>
    </tr>
    <tr>
      <th>20-24</th>
      <td>258</td>
      <td>44.79%</td>
    </tr>
    <tr>
      <th>25-29</th>
      <td>77</td>
      <td>13.37%</td>
    </tr>
    <tr>
      <th>30-34</th>
      <td>52</td>
      <td>9.03%</td>
    </tr>
    <tr>
      <th>35-39</th>
      <td>31</td>
      <td>5.38%</td>
    </tr>
    <tr>
      <th>40+</th>
      <td>12</td>
      <td>2.08%</td>
    </tr>
  </tbody>
</table>
</div>



## Purchasing Analysis (Age)

* Bin the purchase_data data frame by age


* Run basic calculations to obtain purchase count, avg. purchase price, avg. purchase total per person etc. in the table below


* Create a summary data frame to hold the results


* Optional: give the displayed data cleaner formatting


* Display the summary data frame


```python

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Purchase Count</th>
      <th>Average Purchase Price</th>
      <th>Total Purchase Value</th>
      <th>Avg Total Purchase per Person</th>
    </tr>
    <tr>
      <th>Age Ranges</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>&lt;10</th>
      <td>23</td>
      <td>$3.35</td>
      <td>$77.13</td>
      <td>$4.54</td>
    </tr>
    <tr>
      <th>10-14</th>
      <td>28</td>
      <td>$2.96</td>
      <td>$82.78</td>
      <td>$3.76</td>
    </tr>
    <tr>
      <th>15-19</th>
      <td>136</td>
      <td>$3.04</td>
      <td>$412.89</td>
      <td>$3.86</td>
    </tr>
    <tr>
      <th>20-24</th>
      <td>365</td>
      <td>$3.05</td>
      <td>$1,114.06</td>
      <td>$4.32</td>
    </tr>
    <tr>
      <th>25-29</th>
      <td>101</td>
      <td>$2.90</td>
      <td>$293.00</td>
      <td>$3.81</td>
    </tr>
    <tr>
      <th>30-34</th>
      <td>73</td>
      <td>$2.93</td>
      <td>$214.00</td>
      <td>$4.12</td>
    </tr>
    <tr>
      <th>35-39</th>
      <td>41</td>
      <td>$3.60</td>
      <td>$147.67</td>
      <td>$4.76</td>
    </tr>
    <tr>
      <th>40+</th>
      <td>13</td>
      <td>$2.94</td>
      <td>$38.24</td>
      <td>$3.19</td>
    </tr>
  </tbody>
</table>
</div>



## Top Spenders

* Run basic calculations to obtain the results in the table below


* Create a summary data frame to hold the results


* Sort the total purchase value column in descending order


* Optional: give the displayed data cleaner formatting


* Display a preview of the summary data frame




```python

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Purchase Count</th>
      <th>Average Purchase Price</th>
      <th>Total Purchase Value</th>
    </tr>
    <tr>
      <th>SN</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Lisosia93</th>
      <td>5</td>
      <td>$3.79</td>
      <td>$18.96</td>
    </tr>
    <tr>
      <th>Idastidru52</th>
      <td>4</td>
      <td>$3.86</td>
      <td>$15.45</td>
    </tr>
    <tr>
      <th>Chamjask73</th>
      <td>3</td>
      <td>$4.61</td>
      <td>$13.83</td>
    </tr>
    <tr>
      <th>Iral74</th>
      <td>4</td>
      <td>$3.40</td>
      <td>$13.62</td>
    </tr>
    <tr>
      <th>Iskadarya95</th>
      <td>3</td>
      <td>$4.37</td>
      <td>$13.10</td>
    </tr>
  </tbody>
</table>
</div>



## Most Popular Items

* Retrieve the Item ID, Item Name, and Item Price columns


* Group by Item ID and Item Name. Perform calculations to obtain purchase count, average item price, and total purchase value


* Create a summary data frame to hold the results


* Sort the purchase count column in descending order


* Optional: give the displayed data cleaner formatting


* Display a preview of the summary data frame




```python

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th></th>
      <th>Purchase Count</th>
      <th>Item Price</th>
      <th>Total Purchase Value</th>
    </tr>
    <tr>
      <th>Item ID</th>
      <th>Item Name</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>92</th>
      <th>Final Critic</th>
      <td>13</td>
      <td>$4.61</td>
      <td>$59.99</td>
    </tr>
    <tr>
      <th>178</th>
      <th>Oathbreaker, Last Hope of the Breaking Storm</th>
      <td>12</td>
      <td>$4.23</td>
      <td>$50.76</td>
    </tr>
    <tr>
      <th>145</th>
      <th>Fiery Glass Crusader</th>
      <td>9</td>
      <td>$4.58</td>
      <td>$41.22</td>
    </tr>
    <tr>
      <th>132</th>
      <th>Persuasion</th>
      <td>9</td>
      <td>$3.22</td>
      <td>$28.99</td>
    </tr>
    <tr>
      <th>108</th>
      <th>Extraction, Quickblade Of Trembling Hands</th>
      <td>9</td>
      <td>$3.53</td>
      <td>$31.77</td>
    </tr>
  </tbody>
</table>
</div>



## Most Profitable Items

* Sort the above table by total purchase value in descending order


* Optional: give the displayed data cleaner formatting


* Display a preview of the data frame




```python

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th></th>
      <th>Purchase Count</th>
      <th>Item Price</th>
      <th>Total Purchase Value</th>
    </tr>
    <tr>
      <th>Item ID</th>
      <th>Item Name</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>92</th>
      <th>Final Critic</th>
      <td>13</td>
      <td>$4.61</td>
      <td>$59.99</td>
    </tr>
    <tr>
      <th>178</th>
      <th>Oathbreaker, Last Hope of the Breaking Storm</th>
      <td>12</td>
      <td>$4.23</td>
      <td>$50.76</td>
    </tr>
    <tr>
      <th>82</th>
      <th>Nirvana</th>
      <td>9</td>
      <td>$4.90</td>
      <td>$44.10</td>
    </tr>
    <tr>
      <th>145</th>
      <th>Fiery Glass Crusader</th>
      <td>9</td>
      <td>$4.58</td>
      <td>$41.22</td>
    </tr>
    <tr>
      <th>103</th>
      <th>Singed Scalpel</th>
      <td>8</td>
      <td>$4.35</td>
      <td>$34.80</td>
    </tr>
  </tbody>
</table>
</div>


