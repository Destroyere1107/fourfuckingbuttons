DestroyrCo D-4FB - four fucking buttons.

The D-4FB will be the reference implementation of the F4B codebase.

The D-4FB will utilize a menu-based approach to maximize the possibilities of limited inputs. As of now, there is a menu for each button planned (But only the CALCULATE menu will be implemented in v0.0).

The buttons will be arranged as (1) (2) (3) (4), and controls below will assume this order.

MODE SELECTION (Home screen, to be implemented in v0.1):
(CALCULATE) (ADVANCED) (PRGMS) (SETTING)

CALCULATE - The user will do simple arithmetic with four functions. Since four buttons is very little, we will use binary to input numbers.
The initial screen in the CALC mode is a binary input screen, where the user can input a signed 32-bit integer of their choice. The cursor will start on the right side, and the rightmost bit will indicate wether the number is positive or negative (signed 32-bit integer).
Controls: (LEFT/HIGHER BIT) (RIGHT/LOWER BIT) (FLIP) (CONFIRM NUMBER)
Using the LEFT and RIGHT keys, the user should select which bits they want to change and individually do so with FLIP. Once the user is satisfied, they should press CONFIRM. The screen will show a translated version of the number initially; once the user starts inputting the screen will show the second binary number. Controls are the same.
Then, once both numbers have been inputted, the user must input which function they wish to use.
Controls: (ADD/+) (SUB/-) (MUL/×) (DIV/÷)
The calculator will show the result of the calculation after the user selects the operation, and the next controls set will be shown.
Controls: (INPT_V1) (INPT_V2) (INCREMENT( (MAIN_MENU)
INPT_V1 and INPT_V2 return to the CALCULATE mode, selecting the final value as either the first or second operand, respectively. INCREMENT performs the same operation again, using the final value as the 1st operand and reusing the previous operator and 2nd operand, which is useful for finding the results of an exponent. 
If the calculator has multiple modes, MAIN_MENU returns to the MODE SELECTION screen, which is required to start a completely new calculation. Otherwise, it returns to the start of the CALC screen with empty values, akin to the AC (All Clear) key on some other calculators.


ADVANCED - As the name suggests, the ADVANCED mode allows for more complicated math, using a menu-based approach to access more functions. In addition, this mode also allows non-integer numbers via the use of floating-point.
(This mode is not ready for implementation.)

PRGMS - This mode allows for accessing user programs.
(This mode is not ready for implementation.)

SETTINGS - This menu will be dedicated to a few small items. As planned, it will determine wether dots or commas are used in decimals in ADVANCED mode. 
(This mode is not ready for implementation.)
