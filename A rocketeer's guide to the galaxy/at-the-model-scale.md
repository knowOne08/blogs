---
description: >-
  What does everything look like at the model-level rockets that we are
  building!
---

# At the Model Scale

### The States of Flight

The whole flight of the rocket is divided into different states to make the flow of the flight algorithm simple and more efficient.&#x20;

There are six different states of flight of rocket

1. Ground Idle
2. Powered Flight
3. Unpowered Flight
4. Ballistic Descent
5. Parachute Descent
6. Landing&#x20;

#### State Transition&#x20;

1. Ground  Idle -> Powered Flight = Liftoff
2. Powered Flight -> Unpowered Flight = Burnout&#x20;
3. Unpowered Flight -> Ballistic Descent = Apogee
4. Ballistic Descent -> Parachute Descent = Pyro Fire (Parachute ejection)
5. If we are <5m Above ground level then, we have landed safely.

#### Liftoff Algorithm&#x20;

```
// Detecting launch
If Acceleration Z >= Threshold 
then 
    If count_time > 0.1 sec // preventive measure for a false spike in measurement 
        'LIFTOFF'
    else 
        'NO'
else 
    'NO'    
```

#### Burnout Algorithm

```
// Detecting Burnout 
If Acceleration Z <= Threshold 
then 
    If count_time > 0.1 sec // preventive measure for a false spike in measurement 
        'MECO'
    else 
        'NO'
else 
    'NO' 
```

#### Apogee Detection&#x20;

We take readings 1 second apart&#x20;

<pre><code>// Apogee Detection
if current_altitude > (current_altitude - 1 sec)
then 
    'ASCENDING'
<strong>else if current_altitude &#x3C; (current_altitude - 1 sec)
</strong>then 
    'DESCENDING'
</code></pre>

#### Detecting parachute

```
// Detecting parachute
If 25m above ground in a ballistic descent state
then 
    Switch state and fire parachute

```

#### Landed

```
// Safe state
If 5m or less AGL for more than 5 sec
then 
    'LANDED'
```
