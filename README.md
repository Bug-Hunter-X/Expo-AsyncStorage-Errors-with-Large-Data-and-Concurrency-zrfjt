# Expo AsyncStorage Errors with Large Data and Concurrency

This repository demonstrates a common issue encountered when using AsyncStorage in Expo applications, particularly when dealing with large datasets or high concurrency.  The problem stems from AsyncStorage's limitations in handling large amounts of data and multiple simultaneous transactions.

## Problem

The primary issue is the potential for `AsyncStorage` to throw errors when storing or retrieving large objects, or when numerous storage operations happen concurrently.  This can lead to application freezes and crashes.

## Solution

The provided solution focuses on breaking large data into smaller chunks before storage and managing storage transactions effectively.  This mitigates the likelihood of hitting AsyncStorage's limits and improves the overall stability of storage operations.

## Setup

1. Clone the repository.
2. `npm install`
3. Run the app using Expo Go or a similar Expo environment.