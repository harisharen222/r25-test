<p>Understanding</p>
<p>This project involves controlling a rover’s motors using a Sabertooth 2x60 motor driver. Data from an RC transmitter is received via an SBUS receiver. The goal is to interpolate this data to control the motor driver and make the rover move forward or backward.</p>
<p>Thought Process</p>
<p>To solve this, I first identified the need to interpolate the channel values from the SBUS receiver into a format compatible with the Sabertooth motor driver. I decided to use linear interpolation to map the RC transmitter's range to the motor driver’s expected range.</p>
<p>Implementation</p>
<p>1.  I implemented a linear interpolation function to convert the SBUS channel values into the Sabertooth’s PWM range .</p> <p>2.  The code includes functions for opening files, reading data, parsing SBUS packets, and writing PWM values to the Sabertooth driver.</p> <p>3. I tested the implementation by providing sample SBUS data files and verifying that the PWM values were correctly calculated and sent to the Sabertooth motor driver.But i am getting RUNTIME error </p>


<p>Errors and Resolutions</p>
<p>1. Errors were encountered due to mismatched function signatures in `serial.c` and `serial.h`. Resolved by updating the declarations and definitions to match in both files.</p> <p>2.  the error "No such file or directory" was encountered for `main.exe`. Ensured that the executable was properly built and available in the directory.

<p>1.Used the chatbot to clarify the tasks and debug errors in the code.</p> <p>2. asked help for implementing the interpolation function and fixing issues with file handling and compilation.
