# 20262RCOSE32202

Computer Networks - Congestion Control

## Project Overview

This repository contains notes and explanations about congestion control in computer networks.

The main goal is to understand how network bandwidth is managed and how congestion affects data transmission.

This repository focuses on theoretical concepts and learning experiences rather than source code.

## Congestion Control

Congestion control is used to prevent too much data from being sent into a network at once.

If too much data is transmitted, packet loss can occur and network performance can decrease.

In this project, I tried to find a way to send as much data as possible without causing too much packet loss. It was difficult because the available bandwidth changed over time.

## Bandwidth

Bandwidth is the amount of data that a network can transmit in a given time.

In our project, the available bandwidth changed every round, so it was difficult to decide how much data to send.

If the requested amount was too high, it could cause packet loss. However, sending too little data also reduced the total amount of data transmitted.

I had to consider both situations when designing the algorithm.

## Packet Loss

Packet loss occurs when data fails to reach its destination.

In our project, requesting too much bandwidth could cause packet loss and a penalty.

After a loss occurred, I had to wait several rounds before sending data again.

Because of this, I tried to adjust the requested bandwidth to avoid unnecessary losses.

## Penalty System

In our project, a penalty was applied when the requested bandwidth exceeded the available bandwidth.

A high penalty made it harder to transmit data efficiently in later rounds.

At first, I tried to send more data by increasing the requested bandwidth, but this often caused losses.

I learned that avoiding penalties was just as important as sending a large amount of data.

## Week 1 Experiment

In Week 1, I tested different bidding values to find a good way to transmit data.

At first, I tried using higher bids, but this sometimes caused packet loss and penalties.

I compared the results of several tests and adjusted the bidding values to improve performance.

Through these experiments, I learned that sending more data does not always lead to better results.

## Week 2 Experiment

In Week 2, the available bandwidth changed more frequently than in Week 1.

I noticed that periods of low and high bandwidth often appeared repeatedly.

I tested different bidding strategies to handle these changes.

It was difficult to predict the bandwidth, so I tried to make the algorithm work well under different conditions.

## Algorithm Design

I designed the algorithm to adjust bidding values based on previous results.

The algorithm considered factors such as bandwidth, packet loss, and remaining data.

I also tested different strategies to find a balance between high transmission rates and low penalties.

Some strategies worked well in Week 1 but performed poorly in Week 2, so finding a strategy that worked in both weeks was challenging.

## Remaining Data

In this project, each player started with a certain amount of data to transmit.

The goal was to send as much data as possible within 1,000 rounds.

I compared different algorithms by checking how much data remained after each experiment.

An algorithm with less remaining data generally performed better.

## Simulation and Testing

I ran several simulations to compare different algorithms.

I tested them under different bandwidth conditions to see how their performance changed.

Some algorithms worked well in certain situations but had worse results in others.

By comparing the results, I tried to find a strategy that could perform consistently across different network conditions.
