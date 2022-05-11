#include <18F4550.h>
#fuses INTRC, NOPROTECT, NOWDT, NOLVP, CPUDIV1, PLL1        
#use delay (clock = 8M)

#use rs232(rcv=pin_C7, xmit=pin_C6, baud=9600, bits=8, parity=n, stream = BTH)
#use rs232(rcv=pin_B5, xmit=pin_B4, baud=9600, bits=8, parity=n, stream = TTL)

#BYTE TRISD = 0xF95
#BYTE PORTD = 0xF83

int8 i = 0;
char letter;
char word[8];

void main()
{
   //letter = fgetc(BTH);
   while(True)
   {
      letter = fgetc(BTH);
      
      if(letter == '1')
      {
         output_high(pin_a0);
      
      }
      else if(letter == '2')
      {
         output_low(pin_a0);
      
      }
  
    }
    letter = 0;
   
   }
