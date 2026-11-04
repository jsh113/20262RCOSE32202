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
