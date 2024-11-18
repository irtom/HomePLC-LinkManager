# HomePLC-LinkManager

TwinCAT library for linking input groups to output groups that is part of the HomePLC library.

## Dependencies

- [HomePLC DIO](https://github.com/irtom/HomePLC-DIO)
- [HomePLC Logging](https://github.com/irtom/HomePLC-Logging)

## Contents

- FB_LinkManager
  - Contains a list of all links
- FB_Link
  - A link is a relation from an input group to an output group
  - The link defines what the output group does when the input group issues a command
- FB_DIGroup, FB_DOGroup
  - An input group contains digital inputs, an output group contains digital outputs
  - For a list of all possible output group actions and input group commands, see the DIO library
  - An output group constists of digital outputs which is split up in two categories: outputs (relays, lights, ...) and indicators. Outputs can also be manipulated externally (e.g. ADS) while the indicators always show the status of the outputs. 
