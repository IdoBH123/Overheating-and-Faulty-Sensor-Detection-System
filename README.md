# Overheating-and-Faulty-Sensor-Detection-System #

Overheating and Faulty Sensor Detection System
This project involves developing a system to detect overheating and identify faulty sensors using data from multiple temperature sensors. The project focuses on parallel programming to optimize performance and resource utilization. It is implemented using Python.

Steps to Solve the System:

1. Data Reading: Read sensor data from the DATA folder, where each file line represents a temperature sample taken every minute.

2. EMA Algorithm: Apply the Exponential Moving Average (EMA) to minimize the impact of extreme samples (e.g., due to noise).

3. Segment Analysis: Analyze 30-minute time segments, considering the average, minimum, and maximum temperatures.

4. Overheat Detection: Trigger an overheat alert if the average temperature of most sensors exceeds 90°C in any segment, and log the event with the corresponding time segment (e.g., "Temperature alert detected at timeline 60-90").

5. Faulty Sensor Identification: Identify and report faulty sensors if their average temperature in at least half of the time segments falls outside the min-max range of other sensors. If no faulty sensors are detected, nothing will be printed.
