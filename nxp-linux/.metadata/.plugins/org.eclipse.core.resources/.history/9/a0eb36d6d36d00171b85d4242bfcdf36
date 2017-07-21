/*
===============================================================================
 Name        : dma_tst.c
 Author      : $(author)
 Version     :
 Copyright   : $(copyright)
 Description : main definition
===============================================================================
*/

#if defined (__USE_LPCOPEN)
#if defined(NO_BOARD_LIB)
#include "chip.h"
#else
#include <brd.h>
#endif
#endif

#include <cr_section_macros.h>

// TODO: insert other include files here
#include "brd.h"

// TODO: insert other definitions and declarations here

int main(void) {

#if defined (__USE_LPCOPEN)
    // Read clock settings and update SystemCoreClock variable
    SystemCoreClockUpdate();
#if !defined(NO_BOARD_LIB)
    // Set up and initialize all required blocks and
    // functions related to the board hardware
    Board_Init();
    // Set the LED to the state of "On"
    Board_LED_Set(0, true);
#endif
#endif

    // TODO: insert code here
    Board_Init();
    // Enter an infinite loop, just incrementing a counter
    while(1) {

    }
    return 0 ;
}

void SysTick_Handler(void) {
	Chip_GPIO_SetPinToggle(LPC_GPIO_PORT, 0, tstPin0);
}
