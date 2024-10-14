# LEDBlinking-with-Timers-and-MISRA-2012-Compliance-Check.
------------------------------------------------------------
This project involves implementing a scheduling mechanism to control the toggling of three LEDs at different time intervals using a timer. Additionally, the code will be checked for compliance with the MISRA C:2012 guidelines using the Cppcheck static analysis tool.

## Objectives
Toggle three LEDs with different intervals using a timer-based scheduling mechanism.
Ensure code complies with MISRA C:2012 guidelines.
Generate a report using Cppcheck to verify compliance.
LED Toggling Intervals
The task requires the LEDs to be toggled at the following intervals:
----------------------------------------------------------------------
- **LED1:** Toggles every 50 ms
- **LED2:** Toggles every 100 ms
- **LED3:** Toggles every 200 ms

## Implementation Details
- **GPIO Driver:** The project uses the GPIO driver to control the LEDs.
- **Timer Scheduler:** A timer (or multiple timers) will be configured to generate interrupts at the specified intervals for each LED.
- **Interrupts:** The timer interrupt handler will be responsible for toggling the LEDs at the correct intervals.

## Steps:
- **Configure Timer(s):** Set up the timer(s) to trigger interrupts at 50 ms, 100 ms, and 200 ms intervals.
- **Interrupt Handlers:** Use interrupt service routines (ISRs) to toggle the LEDs when the timer expires.
- **MISRA C:** 2012 Compliance: Ensure all code follows the MISRA C:2012 guidelines for safety, portability, and reliability.
- **Static Analysis:** Use Cppcheck to check the code for any violations of MISRA C:2012 guidelines.

## Tools and Requirements
### Hardware:
A microcontroller board with three GPIO pins is configured for LED control.
### Software:
- **Cppcheck:** A static analysis tool used to verify MISRA compliance.
- **IDE:** Any C development environment that supports embedded programming and GPIO configurations.

## Compliance Verification
- **MISRA C:** 2012 Guidelines
The code will adhere to MISRA C:2012 guidelines, which aim to enforce best practices for safety-critical systems, specifically in the automotive and embedded domains.
Guidelines cover areas such as:
Avoiding unsafe practices (e.g., direct pointer arithmetic, non-deterministic constructs).
Enforcing strong type-checking and preventing implicit type conversions.
Ensuring maintainability and portability across platforms.
## Cppcheck Report:
After writing the code, the Cppcheck tool will be used to analyze the code and generate a report.
The report will indicate any deviations or violations of MISRA C:2012.
The report will be submitted along with the source code.

## Project Demo
https://github.com/user-attachments/assets/ea393d72-e873-4891-ae47-1030ca61bd6c

## How to Run the Project
1. Clone this repository:
   ```sh
   git clone https://github.com/AhmedKamalMohammedElSayed/LEDBlinking-Timers-MISRA2012.git
    ```
2. Build the Project: Ensure your IDE is set up for the target microcontroller, and build the project.

3. Deploy to the Microcontroller: Flash the compiled firmware to the microcontroller using your preferred programmer.

4. Run Cppcheck for MISRA Compliance: Use the following command to generate a MISRA compliance report
   ```sh
    cppcheck --enable=misra --xml-version=2 . 2> cppcheck-report.xml
    ```
## Author
Ahmed Kamal
