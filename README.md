# VHDL Integer Overflow Bug

This repository demonstrates a potential integer overflow bug in a simple VHDL counter.  The counter is designed to count from 0 to 15, but there's a lack of explicit overflow handling.

## Bug Description
The `integer` type in VHDL, while convenient, doesn't inherently prevent overflows. If the counter reaches its maximum value (15), incrementing it would lead to undefined behavior.  This could manifest as unexpected values or simulation errors.

## Solution
The provided solution incorporates explicit overflow handling to prevent this issue and ensure predictable behavior.