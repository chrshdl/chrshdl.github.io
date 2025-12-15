---
layout: single
title: Product
permalink: /product/
---

This page explains all widgets shown on the instrument cluster and how to interpret them while driving in Gran Turismo 7.

The following widgets are available:

- [**Speed**](#speed)
- [**Gear**](#gear)
- [**RPM**](#rpm)
- [**Tire temperature**](#tire-temperature)
- [**Fastest lap**](#fastest-lap)
- [**Previous lap**](#previous-lap)
- [**Diff**](#diff)
- [**Predicted lap**](#predicted-lap)

<picture>
  <img alt="dashboard widgets" src="https://lh3.googleusercontent.com/pw/AP1GczOSUIj2s5i6_FBkbbuSE9K2bUN8DO2gndaDBjKAW8-ZoOl_3RGTz_5jgdiCrParf9QAKxjsaUCNQ2dkOKwMaAOSWAMSEhVWXxczfXxcpWvm11o5z0nffJ19wnNOtz3QSmDSiq4EpPMWrdkA7IHw_UjH=w1024-h600-s-no" width="100%" height="100%">
</picture>

---

## Speed

**What it shows**

- The current vehicle speed.

**Details**

Use this widget as your primary reference for braking points and speed through corners.

---

## Gear

**What it shows**

- The currently engaged gear (e.g. 1, 2, 3, ..., 6).

**Details**

- Updates in real time as you shift.
- May show **N** for neutral or **R** for reverse depending on the car.

This is useful for confirming that you are in the correct gear for a corner or a straight.

---

## RPM

**What it shows**

- The current engine RPM (revolutions per minute).
- Two alert bounds:
  - min RPM bound $\rightarrow$ this is the rev warning
  - max RPM bound $\rightarrow$ this is the rev limiter

**Details**

- The RPM bar/number increases as you accelerate and decreases when you lift or brake.
- The min alert bound marks the RPM range where you should consider shifting up soon.  
  Think of it as a shift warning: staying above this too long can be inefficient or put extra stress on the engine.
- The max bound marks the RPM where the rev limiter will kick in.  
  If you reach or exceed this, the engine will stop gaining power and may "bounce" on the limiter.

**Car-dependent behavior**

- Both min and max alert bounds are automatically updated whenever you change car.
- This allows the RPM widget to match each car's specific power band and rev limit.

**Use the RPM widget to time your upshifts**
- Aim to shift between the min and max bounds.
- Avoid spending too much time at or above the max bound, as you’re no longer gaining speed and just hitting the limiter.

---

## Tire temperature

**What it shows**

- The current temperature of your tires.

**Details**

- Visualizes how “warm” or “cold” the tires are.
- Helps you understand:
  - Whether you are generating enough heat (pushing hard enough).
  - Whether you may be overheating the tires during long stints.

Cold tires usually mean less grip; overheated tires can also lose grip and wear faster.

---

## Fastest lap

**What it shows**

- The **best (lowest) lap time** you have achieved in the current session.

**Details**

- Updates whenever you complete a lap faster than the previous best.
- This is the reference time you are trying to beat.

You can think of this as your personal “benchmark” for the current run.

---

## Previous lap

**What it shows**

- The **time of the last completed lap**.

**Details**

- Updates at the start/finish line when you complete a lap.
- Always shows the most recent lap time, even if it was slower than your fastest lap.

This is useful for quickly comparing your last lap to your fastest lap and your current pace.

---

## Diff

**What it shows**

- The **time difference (delta)** in seconds between your **predicted lap** and your **previous lap**.

In other words, it indicates how much faster or slower your current lap is trending compared to the last one.

> ℹ️ Note: The **first two laps are discarded** for delta calculations. Because of that, the Diff widget only shows valid values from lap 3 onwards. On lap 1 and lap 2, the widget will not display meaningful delta data and will stay empty.

---

## Predicted lap

**What it shows**

- The **predicted lap time** based on your current performance in the ongoing lap.

**Calculation**

- The predicted lap is calculated as:  
  **`predicted lap = previous lap + diff`**

Examples:

- If your **previous lap** was `1:40.000` and the **diff** is `-0.500`, the predicted lap would be around `1:39.500`.
- If your **previous lap** was `1:40.000` and the **diff** is `+0.300`, the predicted lap would be around `1:40.300`.

**Details**

- Updates continuously during the lap as the delta changes.
- Gives you an idea of what lap time you are "on for" if you keep up your current pace.

---

## Summary

- **Speed** and **Gear** help you drive consistently and hit your braking/shift points.
- **Tire temperature** tells you about grip and tire usage over time.
- **Fastest lap** and **Previous lap** give you simple, direct timing comparisons.
- **Diff** and **Predicted lap** give you `real-time feedback` on whether the current lap is faster or slower than the previous one.
- Remember: the **Diff** only becomes valid from **lap 3** onwards, because the first two laps are discarded for the delta logic.

