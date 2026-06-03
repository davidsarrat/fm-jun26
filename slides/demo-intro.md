## What the demo trains on

<div class="grid grid-cols-2 gap-8 mt-2">
<div>

**Real records, three real hospitals.** Every row is a real patient seen at one of the original UCI Heart Disease institutions:

- Cleveland Clinic, USA <span style="color:#8a7d70;">(303)</span>
- Hungarian Institute of Cardiology, Budapest <span style="color:#8a7d70;">(261)</span>
- VA Medical Center, Long Beach, USA <span style="color:#8a7d70;">(130)</span>

The records never leave the hospital that owns them.

<div class="mt-4">

**The goal.** Train one shared model that estimates a patient's probability of heart disease from ten routine cardiology measurements, without any site sharing a single record.

</div>

</div>
<div style="font-size: 0.82em;">

| feature | what it measures |
|---|---|
| `age` | age in years |
| `sex` | 1 = male, 0 = female |
| `cp` | chest pain type |
| `trestbps` | resting blood pressure (mm Hg) |
| `chol` | serum cholesterol (mg/dl) |
| `fbs` | fasting blood sugar > 120 mg/dl |
| `restecg` | resting ECG result |
| `thalach` | maximum heart rate achieved |
| `exang` | exercise-induced angina |
| `oldpeak` | ST depression from exercise |

</div>
</div>
