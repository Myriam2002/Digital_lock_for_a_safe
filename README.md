# Digital Lock for a Safe

## Project Description

Due to the ever-growing scientific technological advancements, crime rates are subsequently increasing throughout the world each day. Therefore, our team has designed a simple, cheap yet secure, and reliable system of a digital lock for the safe using logic gates, comparators, registers, and flip-flops. This system aims to prevent intruders and thieves from accessing the safe unless they can provide a binary password that correctly matches the preset password.

## Features

- Binary Password Verification: The system compares each bit of the user-entered passcode with the corresponding bit in the preset code. This comparison is performed using 4 XNOR gates, ensuring that the output is one only if all the bits match.

- Overall Match Verification: The outputs of the four XNOR gates are passed through an AND gate, producing a one output if all the bits match and a zero output otherwise.

- Three Consecutive Incorrect Attempts Lockout: To limit unauthorized access attempts, the system utilizes a 2-bit synchronous counter implemented with two T flip-flops. The counter increments with each incorrect password entry. If the count reaches three, the safe will no longer accept any further entries until the user presses the reset button.

- Reset Functionality: The user can reset the digital lock by pressing the reset button after three consecutive incorrect attempts. This allows them to start trying to open the safe again.

- Safe Opening: If the binary passcode entered by the user is correct at any trial, the lock will open safely, granting access to the contents of the safe.

- Asynchronous Edge Detection: An asynchronous edge detector, implemented using NOT gates and XOR gates, is utilized to detect changes in input and acts as a clock signal for the two T flip-flops.

## System Design

The system design includes the following components:

- Logic Gates: XNOR gates are used for bit comparison, while an AND gate combines the outputs to determine the overall match.

- Synchronous Counter: A 2-bit synchronous counter, implemented with two T flip-flops, keeps track of the number of incorrect password entries.

- Decoder: The counter's output is passed through a decoder to display the count of the current entry attempt. If the count reaches three, the user should click the reset button to reset the digital lock.

- Asynchronous Edge Detector: NOT gates and XOR gates are used to detect changes in input and provide the necessary clock signal for the T flip-flops.

## Conclusion

Our digital lock system offers a cost-effective and reliable solution for securing safes. By utilizing logic gates, comparators, registers, and flip-flops, we have created a system that requires a correct binary passcode for access, prevents unauthorized attempts after three consecutive failures, and includes a reset functionality for continued safe usage. With these features, our digital lock system provides enhanced security and peace of mind.

For more details, please refer to the project documentation and schematic diagrams.

