# README

This example demonstrates the following:
 * Configuriong GPIO pins
 * Toggling GPIO pins
 * Setting up and using GPIO interrupts
 * Unlocking protected GPIO pins
 * Controlling the system clock
 * Changing the system clock on the fly

Flashes the Red, Green and Blue diodes on the board, in order. The system clock
starts at 80MHz.
Pressing SW2 toggles the system clock between 80MHz, 57MHz, 40MHz ,20MHz, and
16MHz by changing the PLL divisor.
Pressing SW1 bypasses the PLL completely, and runs off the raw 16MHz clock
provided by the external crystal oscillator.
The LEDs will toggle at different speeds, depending on the system clock. The
system clock changes are handled within the interrupt service routine.
