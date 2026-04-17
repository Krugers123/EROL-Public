# EROL Public Architecture

## Purpose

This document explains the high-level public architecture direction of EROL.

## Public Architecture Reading

EROL should be read as an external response observability layer built around five public-safe layers:

1. `Multi-Source Signal Intake`
2. `Trajectory Reading Layer`
3. `Drift and Proportionality Interpretation`
4. `Cross-Region / Cross-System Comparison`
5. `Calibration Support Surface`

## 1. Multi-Source Signal Intake

EROL is built to aggregate heterogeneous signals rather than depend on a single indicator family.

These may include:

- capacity indicators
- morbidity and mortality trends
- intervention records
- behavior and mobility indicators
- adverse-event reporting

## 2. Trajectory Reading Layer

The system is not interested only in one data point or one policy action.

It studies:

- how pressure evolves
- how intervention intensity evolves
- how those trajectories align or diverge across time

## 3. Drift and Proportionality Interpretation

EROL translates signal trajectories into public-safe readings such as:

- proportionality drift
- response lag
- saturation mismatch
- overreaction / underreaction patterns
- calibration instability

## 4. Cross-Region / Cross-System Comparison

A core advantage of observability is comparison.

EROL should make it possible to compare:

- regions
- time windows
- intervention trajectories
- signal families

## 5. Calibration Support Surface

EROL does not decide policy.

It provides a calibration support surface that helps make visible when the response system itself may no longer be tracking real-world pressure proportionally.

## Architectural Principle

EROL is strongest when it remains:

- external
- neutral
- comparative
- trajectory-aware
- calibration-oriented
