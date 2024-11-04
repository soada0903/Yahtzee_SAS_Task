# Yahtzee API Test Cases


## Introduction
This repository contains test cases for the Yahtzee REST API, developed to validate the functionality of the endpoints defined in the provided OpenAPI specification. The tests cover key features such as player management, die management, and Yahtzee condition verification.


## Objective
The primary objective of these test cases is to ensure that the Yahtzee API behaves as expected under various conditions, handling valid and invalid inputs, respecting authentication requirements, and accurately representing game rules.


# Approach

## Test Structure
The test cases are structured using Gherkin syntax to provide a clear, readable format that outlines each scenario's conditions, actions, and expected results. The test cases were written with a focus on:
	Functional Testing: Confirming each endpoint works correctly with valid inputs.
	Boundary Testing: Ensuring endpoints handle both valid and invalid data within defined boundaries.
	Negative Testing: Validating proper error handling for unauthorized access, incorrect inputs, and other invalid conditions.
	Schema Validation: Checking that responses adhere to the expected JSON schema.
	Authorization Testing: Ensuring endpoints requiring authentication return appropriate responses when unauthorized access is attempted.
 

## Test Coverage

The test cases cover:
	Player Management: Retrieve and set the player’s name with both valid and invalid inputs.
	Die Management: Retrieve individual dice values, set values, and roll dice, including handling of valid and invalid IDs.
	Game Conditions: Verify the Yahtzee condition (all dice match or differ).
 

## Test Execution

Since running the service is not mandatory, I focused on writing comprehensive test cases rather than executing them locally. I included comments to ensure that some parts are clear for review.


## Test Case Highlights

Here is a brief overview of the test scenarios:

## 1.	Player Management:
	Retrieve the player’s name.
	Set the player’s name with valid input.
	Attempt to set an invalid or empty name.
	Attempt to set the name without authorization.
 
## 2.	Die Management:
	Retrieve a die’s value in multiple formats (integer, float, word, dots).
	Set and roll dice with valid and invalid IDs and values.
	Handle missing or incorrect authentication for restricted actions.
 
## 3.	Game Conditions:
	Verify Yahtzee state (all dice matching) and non-matching scenarios.
