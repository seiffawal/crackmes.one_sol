---
title: Analysis Report for ezreverse.exe
updated: 2024-02-17 18:17:37Z
created: 2024-02-17 15:38:26Z
latitude: 30.22005020
longitude: 31.36888420
altitude: 0.0000
---

# Analysis Report for ezreverse.exe
`Challange Author: Clyax` `challange: ezreverse.exe` `website: crackmes.one`
## Challange Description:
Im currently starting learning C and want to apply what have i learn. Also i create this simple code to learn reversing. If there's a bug, tell me in the comment. (Also im looking for a discord server community to start learning code)
## Objective:
Our objective is to understand the functionality of the ezreverse.exe application using IDA Freeware.

## Application Overview:
The ezreverse.exe application is designed to accept a username and password from the user and determine whether the provided password is deemed "good" or "bad" based on certain criteria.

## Key Observations:
- Identification of Input Fields: Upon initial analysis, we identified strings within the executable related to "username" , "password,"and "good \n" indicating the presence of input fields for these credentials.

- Functionality Exploration: Utilizing IDA's interface, we proceeded to explore the functionality of the application.

- Conditional Checks: We observed the presence of conditional checks  within the code logic. These checks likely evaluate the input password against predefined criteria to determine its validity.

- Loop Structure: A loop structure was identified within the code, suggesting iterative processing of input data or repetitive execution of certain operations.

- Comparison with edx: Notably, there is a comparison operation involving the value stored in the edx register and a specific memory address [rsp+0C8h+pw]. This comparison likely plays a crucial role in determining whether the password is considered "good" or "bad."
<span style="color:red">**CODE DECOMPILED(ghidra)**</span>




![hello](https://github.com/seiffawal/crackmes.one_sol/assets/83987697/354f4dbf-aa5f-4360-bdfa-f87c9da85afb)
