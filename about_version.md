# Modulize-Version Specification
In a sense, this is a subset of **[SimVer](https://simversion.github.io)**. \
This document describes only differences.

## Definitions of MAJOR, MINOR, PATCH
### Conventions
**SimVer** and **SimVersion** references [SimVer](https://simversion.github.io).

**\d** Is a **DIGIT** in range of **0..9** \
*Examples* \d -> 0, *or* \d\d -> 00
**n\d** Is a **DIGIT** in range of **n..9** \
*Examples* \d -> 1, *or* 1\d\d -> 10
**~\d**  Is an ***OPTIONAL*-DIGIT** in range of **0..9** \
*Examples* \d\~\d -> 1, 11 *or* ~\d\d -> 10, 0 \
**~n\d**  Is an ***OPTIONAL*-DIGIT** in range of **n..9** \
*Examples* \d -> 1, *or* 1\d\d -> 10

### Differences from SimVer
- MAJOR \
  Defined as **YEAR-OF-RELEASE** \
  *Format* \d\d\d\d (YYYY) \
  *Example* 2020
- MINOR \
  Defined as **CALENDER-WEEK** \
  *Format* \d\d
  *Examples* 01 = first calender week
- PATCH \
  Same as SimVer: a **DIGIT** incremented by 1 starts from 0 


