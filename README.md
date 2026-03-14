# Hotel Booking Cancellation Prediction

## Context
A significant number of hotel bookings are called off due to cancellations or no-shows. The typical reasons for cancellations include change of plans, scheduling conflicts, etc. This is often made easier by the option to cancel free of charge or at a low cost. While this flexibility benefits hotel guests, it can negatively impact hotel revenue, especially in cases of last-minute cancellations.

With the rise of online booking channels, customers now have more flexibility and options when making reservations. This has significantly changed booking behavior and increased the complexity of managing cancellations.

Booking cancellations impact hotels in several ways:

1. **Loss of revenue** when the hotel cannot resell the canceled room.
2. **Additional distribution costs**, such as higher commissions or marketing expenses to resell rooms.
3. **Last-minute price reductions** to resell rooms, which reduces profit margins.
4. **Operational overhead**, as staff must manage cancellations and rebookings.

---

## Objective
The increasing number of cancellations calls for a **Machine Learning–based solution** that can predict which bookings are likely to be canceled.

**INN Hotels Group**, a chain of hotels in Portugal, is experiencing a high rate of booking cancellations and has approached our firm for a **data-driven solution**.

As a **Data Scientist**, the objectives are:

- Analyze the booking data to identify factors influencing cancellations.
- Build a **predictive machine learning model** that can forecast whether a booking will be canceled.
- Help the hotel develop **profitable cancellation and refund policies** based on the insights.

---

## Data Description
The dataset contains various attributes related to customers’ booking details.

---

## Data Dictionary

| Feature | Description |
|-------|-------------|
| **Booking_ID** | Unique identifier of each booking |
| **no_of_adults** | Number of adults |
| **no_of_children** | Number of children |
| **no_of_weekend_nights** | Number of weekend nights (Saturday or Sunday) booked |
| **no_of_week_nights** | Number of weeknights (Monday to Friday) booked |
| **type_of_meal_plan** | Type of meal plan booked |
| **required_car_parking_space** | Whether parking space is required (0 = No, 1 = Yes) |
| **room_type_reserved** | Type of room reserved (encoded by the hotel) |
| **lead_time** | Number of days between booking date and arrival date |
| **arrival_year** | Year of arrival |
| **arrival_month** | Month of arrival |
| **arrival_date** | Day of the month of arrival |
| **market_segment_type** | Market segment category |
| **repeated_guest** | Whether the customer is a repeated guest (0 = No, 1 = Yes) |
| **no_of_previous_cancellations** | Number of previous cancellations by the customer |
| **no_of_previous_bookings_not_canceled** | Number of previous bookings that were not canceled |
| **avg_price_per_room** | Average daily price of the room (in euros) |
| **no_of_special_requests** | Number of special requests made by the customer |
| **booking_status** | Target variable indicating if booking was canceled or not |


## Methodology

The project followed a structured machine learning workflow:

### 1. Data Preprocessing
- Handling missing values
- Encoding categorical variables
- Data cleaning and transformation

### 2. Exploratory Data Analysis (EDA)
- Distribution analysis
- Correlation analysis
- Visualization of booking patterns
- Identification of cancellation trends

### 3. Feature Engineering
- Creation of meaningful predictors
- Transformation of categorical variables
- Handling class imbalance

### 4. Model Building
Multiple classification models were developed and compared:

- Logistic Regression
- Decision Tree
- Random Forest
- Other classification algorithms

### 5. Model Evaluation
Models were evaluated using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **ROC-AUC**

The best-performing model was selected based on overall predictive performance and interpretability.

---

## Key Insights

- **Lead time** is a major driver of cancellations; bookings made far in advance are more likely to cancel.
- **Deposit type** significantly influences cancellation behavior.
- **Market segment** plays a key role in booking reliability.
- Customers with **previous cancellations** are more likely to cancel again.

---

## Business Impact

The final model helps hotels:

- Identify **high-risk cancellation bookings**
- Improve **revenue management strategies**
- Optimize **overbooking decisions**
- Implement **targeted customer retention campaigns**

These insights help reduce revenue loss and improve operational efficiency.

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn


