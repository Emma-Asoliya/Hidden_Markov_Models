# Human Activity Recognition Using Hidden Markov Models

A smartphone-based activity recognition system that uses Hidden Markov Models to classify four physical activities (still, standing, walking, jumping) from accelerometer and gyroscope sensor data, developed for physiotherapy rehabilitation monitoring.

---

## Project Structure

```
├── data/
│   ├── still/          # Training recordings - still activity
│   ├── standing/       # Training recordings - standing activity
│   ├── walking/        # Training recordings - walking activity
│   └── jumping/        # Training recordings - jumping activity
├── test_data/
│   ├── still/          # Unseen test recordings - still activity
│   ├── standing/       # Unseen test recordings - standing activity
│   ├── walking/        # Unseen test recordings - walking activity
│   └── jumping/        # Unseen test recordings - jumping activity
├── notebook/
│   └── hmm_activity_recognition.ipynb
├── report/
│   └── hmm_report.pdf
└── README.md
```

---

## Device & Recording Setup

| Parameter | Details |
|---|---|
| Device | Samsung SM-S901U (Android) |
| App | Sensor Logger |
| Sampling Rate | 100 Hz (10ms intervals) |
| Sensors | Accelerometer (m/s²) + Gyroscope (rad/s) |
| Activities | Still, Standing, Walking, Jumping |
| Recording Duration | 5-10 seconds per session |

---

## How to Run

1. Open `notebook/hmm_activity_recognition.ipynb` in Google Colab
2. Run Cell 0 to install dependencies:
   ```
   !pip install hmmlearn
   ```
3. Upload your data files into the correct `data/` and `test_data/` subfolders
4. Run all cells in order from top to bottom

---

## Requirements

- Python 3.10+
- numpy
- pandas
- matplotlib
- seaborn
- scipy
- scikit-learn
- hmmlearn

---

## Results

| Activity | Sensitivity | Specificity | Accuracy |
|---|---|---|---|
| Still | 1.000 | 1.000 | 1.000 |
| Standing | 0.903 | 0.979 | 0.961 |
| Walking | 1.000 | 0.951 | 0.961 |
| Jumping | 0.902 | 1.000 | 0.969 |
| **Overall** | | | **0.945** |

---

## Author

Emmanuella Briggs | Machine Learning Techniques II | July 2026
