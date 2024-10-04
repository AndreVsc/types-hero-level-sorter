
# Hero Level Classifier Documentation

## Overview

This application categorizes heroes based on their experience points (XP) into different levels. The classification ranges from **Iron** to **Radiant**, depending on the hero's XP.

## Classification Criteria

| XP Range          | Hero Level |
|-------------------|------------|
| Less than 1,000   | Iron       |
| 1,001 - 2,000     | Bronze     |
| 2,001 - 5,000     | Silver     |
| 5,001 - 7,000     | Gold       |
| 7,001 - 8,000     | Platinum   |
| 8,001 - 9,000     | Ascendant  |
| 9,001 - 10,000    | Immortal   |
| Greater than 10,001 | Radiant  |

## Input/Output

### Input

- **Hero Name**: The name of the hero (e.g., "Arthur").
- **Experience Points (XP)**: A numeric value representing the hero's experience.

### Output

A message in the following format:
```
The Hero named {heroName} is at the level of {level}
```

### Example

**Input**:
```
Hero Name: Athena
XP: 7500
```

**Output**:
```
The Hero named Athena is at the level of Platinum
```

## Implementation Details

The hero's level is determined using a series of conditional statements (`if-else`). The XP values are compared to determine the appropriate level.

## Dependencies

- `readline-sync` for input handling via command line.
- TypeScript for type safety and cleaner JavaScript code.

## Running Tests

Testing can be done manually by executing the program multiple times with different inputs, or automated unit tests can be written using frameworks like Jest.

## Future Improvements

- Add more levels or customize the leveling system.
- Allow saving the hero's information in a database or a file.