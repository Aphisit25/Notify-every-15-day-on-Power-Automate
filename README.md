# Notify every 15 day

1. Create [Schedule]
2. Create [Get items]
3. Create [Apply to each]
    - Select an output from previous steps
      - Select [value] form Get items
    - Create [Compose]
      - Select [fields] form Get items
    - Create [Condition]
      - addDays(utcNow(),+15,'yyyy-MM-dd') '-- Date now
      - formatDateTime(outputs('fPlan'), 'yyyy-MM-dd') '-- fPlan = name form Compose
    - Send an email


![image](https://github.com/Aphisit25/Notify-every-15-day-on-Power-Automate/blob/main/image/A1.png)
