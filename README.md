# Human Activity Recognition (HAR) - 3 Activities

This repository focuses on Human Activity Recognition (HAR) for three specific activities: **running**, **sitting**, and **climbing stairs**. HAR is a vital component of wearable technology applications, such as fitness tracking, health monitoring, and context-aware systems.

---

## Dataset Description

The dataset is structured to capture sensor readings from an accelerometer and gyroscope for six axes (‘acc_x’, ‘acc_y’, ‘acc_z’, ‘gyr_x’, ‘gyr_y’, ‘gyr_z’) and a corresponding activity label. The data is organized into the following format:

```
[
  [
    [acc_x_values],
    [acc_y_values],
    [acc_z_values],
    [gyr_x_values],
    [gyr_y_values],
    [gyr_z_values],
    [label]
  ],
  [
    [acc_x_values],
    [acc_y_values],
    [acc_z_values],
    [gyr_x_values],
    [gyr_y_values],
    [gyr_z_values],
    [label]
  ],
  ...
]
```

### Sensor Data Details:

- **Accelerometer values (`acc_x`, `acc_y`, `acc_z`)**: Measure acceleration forces along the x, y, and z axes.
- **Gyroscope values (`gyr_x`, `gyr_y`, `gyr_z`)**: Measure angular velocity along the x, y, and z axes.

### Labels:

- **0**: Running
- **1**: Sitting
- **2**: Climbing stairs

Each record in the dataset represents a set of 100 samples collected over a brief time window for the six sensor axes.

---

## Model Purpose

The model aims to:

1. **Classify Human Activities**: Distinguish between the three target activities (running, sitting, climbing stairs) based on sensor data.
2. **Improve Health and Fitness Monitoring**: By detecting activities, the system can provide real-time feedback to users about their physical state.
3. **Support Context-Aware Systems**: Enabling devices to adapt to user behavior and optimize their functionality based on detected activity.

---

## Workflow

### Data Preprocessing:

1. Sensor readings are collected and structured into the defined format.
2. Each sample is validated to ensure it contains exactly 100 values per sensor axis.
3. Labels are appended to indicate the corresponding activity.

### Model Training:

- A machine learning or deep learning model is trained on the dataset using the six sensor axes as input features and the labels as target outputs.
- The model leverages time-series analysis techniques for optimal performance.

### Model Evaluation:

- Metrics such as accuracy, precision, recall, and F1-score are used to evaluate the model’s effectiveness in classifying activities.

---

## Potential Applications

1. **Fitness Trackers**: Enhance the precision of step counters and activity monitors.
2. **Health Monitoring**: Provide insights into user mobility patterns, which are crucial for elderly care or rehabilitation.
3. **Smart Homes**: Enable adaptive environments that respond to user activities, such as adjusting lighting or suggesting posture corrections.
