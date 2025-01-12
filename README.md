# Mobile Price Range Prediction

This project aims to predict the price range of mobile devices based on their features. It uses a dataset containing various technical specifications of mobile phones, with the target variable being `price_range` (categorized as 0, 1, 2, or 3).

## Dataset

The dataset consists of the following features:

- `battery_power`: Total energy capacity of the battery (mAh).
- `blue`: Indicates whether the phone has Bluetooth (1: Yes, 0: No).
- `clock_speed`: Speed at which the microprocessor executes instructions (GHz).
- `dual_sim`: Indicates whether the phone supports dual SIM (1: Yes, 0: No).
- `fc`: Front camera megapixels.
- `four_g`: Indicates whether the phone supports 4G (1: Yes, 0: No).
- `int_memory`: Internal memory of the phone (GB).
- `m_dep`: Mobile depth in cm.
- `mobile_wt`: Weight of the mobile phone (grams).
- `n_cores`: Number of cores in the processor.
- `pc`: Primary camera megapixels.
- `px_height`: Pixel resolution height.
- `px_width`: Pixel resolution width.
- `ram`: Random Access Memory (MB).
- `sc_h`: Screen height of the mobile phone (cm).
- `sc_w`: Screen width of the mobile phone (cm).
- `talk_time`: Longest time the phone can be used without recharging (hours).
- `three_g`: Indicates whether the phone supports 3G (1: Yes, 0: No).
- `touch_screen`: Indicates whether the phone has a touchscreen (1: Yes, 0: No).
- `wifi`: Indicates whether the phone supports Wi-Fi (1: Yes, 0: No).
- `price_range`: Target variable, categorized into 4 classes:
  - 0: Low cost
  - 1: Medium cost
  - 2: High cost
  - 3: Very high cost

### Example Data:

| battery_power | blue | clock_speed | dual_sim | fc | four_g | int_memory | m_dep | mobile_wt | n_cores | pc | px_height | px_width | ram | sc_h | sc_w | talk_time | three_g | touch_screen | wifi | price_range |
|---------------|------|-------------|----------|----|--------|------------|-------|-----------|---------|----|-----------|----------|-----|-------|-------|-----------|---------|--------------|------|-------------|
| 842           | 0    | 2.2         | 0        | 1  | 0      | 7          | 0.6   | 188       | 2       | 2  | 20        | 756      | 2549 | 9     | 7     | 19        | 0       | 0            | 1    | 1           |
| 1021          | 1    | 0.5         | 1        | 0  | 1      | 53         | 0.7   | 136       | 3       | 6  | 905       | 1988     | 2631 | 17    | 3     | 7         | 1       | 1            | 0    | 2           |
| 563           | 1    | 0.5         | 1        | 2  | 1      | 41         | 0.9   | 145       | 5       | 6  | 1263      | 1716     | 2603 | 11    | 2     | 9         | 1       | 1            | 0    | 2           |
| 615           | 1    | 2.5         | 0        | 0  | 0      | 10         | 0.8   | 131       | 6       | 9  | 1216      | 1786     | 2769 | 16    | 8     | 11        | 1       | 0            | 0    | 2           |
| 1821          | 1    | 1.2         | 0        | 13 | 1      | 44         | 0.6   | 141       | 2       | 14 | 1208      | 1212     | 1411 | 8     | 2     | 15        | 1       | 1            | 0    | 1           |

## Project Structure

- `data/`: Contains the dataset files.
- `notebooks/`: Jupyter notebooks for data analysis and model development.
- `models/`: Saved machine learning models.
- `scripts/`: Scripts for preprocessing, training, and evaluation.
- `README.md`: This file.

## Installation

1. Clone the repository:
   ```bash
   git clone [https://github.com/PRIYANSHUNA/mobile_price_prediction.git](https://github.com/PRIYANSHUNA/mobile_price_prediction)
   ```
2. Navigate to the project directory:
   ```bash
   cd mobile_price_prediction
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Prepare the dataset:
   - Place the dataset file in the `data/` directory.

2. Run data preprocessing:
   ```bash
   python scripts/preprocess.py
   ```

3. Train the model:
   ```bash
   python scripts/train.py
   ```

4. Evaluate the model:
   ```bash
   python scripts/evaluate.py
   ```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes and push them to your branch.
4. Submit a pull request.

## Contact

For questions or feedback, please contact [Priyanshu Namdev](priyanshnamdev123@gmail.com).

