Making three tasks to glow three LEDs on the NUcleo H723ZG board.

The LEDs on the board are glowing. Monitor the ODR register in GPIOB SFR in debug perspective. Continuous pausing and running the program shoes that the respective pins are toggling to 0s and 1s. The LEDs are toggling very fast on the board.

Further the code can be updated by deleting two task functions and using a single LED toggle function by passing the LED pin number as argument to three tasks to toggle three LEDs.

The Yellow LED does not toggle on the board as it is connected to GPIOE. But the task sends only GPIOB as the argument, this explains why the yellow LED doesn not toggle.

Now it is to be explored if two parameters can be sent in the xTaskCreate argument list.