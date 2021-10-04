# DigitalElectronics2
# Lab 1: Raul Gomez
My github repository

(https://github.com/raulgoi/DigitalElectronics2/blob/main/README.md)

## Blink example

1. The meaning of:

 * | : or bit to bit
 * & : and bit to bit
 * ^ : exclusive or
 * ~ : Complement to one or bit to bit negation
 * << : move to left
 * >> : move to right

2. Complete the table:


| b | a | b or a | b and a | b xor a | not b |
| - | - | ------ | ------- | ------- | ----- |
| 0 | 0 |
| 0 | 1 |
| 1 | 0 |
| 1 | 1 |


## Morse code


#define _delay_ms  SHORT_DELAY 5 ms

int main(void)
{
    // Set pin as output in Data Direction Register
    // DDRB = DDRB or 0010 0000
    DDRB = DDRB | (1<<LED_GREEN);

    // Set pin LOW in Data Register (LED off)
    // PORTB = PORTB and 1101 1111
    PORTB = PORTB & ~(1<<LED_GREEN);

    // Infinite loop
    while (1)
    {
        // Pause several milliseconds
        _delay_ms(SHORT_DELAY);
        //R
        DDRB = DDRB | (1<<LED_GREEN);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        DDRB = DDRB | (1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        DDRB = DDRB | (1<<LED_GREEN);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        //A
        DDRB = DDRB | (1<<LED_GREEN);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        DDRB = DDRB | (1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        //U
        DDRB = DDRB | (1<<LED_GREEN);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        DDRB = DDRB | (1<<LED_GREEN);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        DDRB = DDRB | (1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        //L
        DDRB = DDRB | (1<<LED_GREEN);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
         DDRB = DDRB | (1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        DDRB = DDRB | (1<<LED_GREEN);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);
        DDRB = DDRB | (1<<LED_GREEN);
        PORTB = PORTB & ~(1<<LED_GREEN);
        _delay_ms(SHORT_DELAY);

         }

    // Will never reach this
    return 0;
}


## Scheme



![SED 2](https://user-images.githubusercontent.com/91128806/135897888-bf547d81-d80b-4d1f-b8fc-f430f985fc46.png)



