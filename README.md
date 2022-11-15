# Embedded-Lab-4


Question 2: The code uses the SM clock to create the PWM signal. The period is set by setting TB0CCR0 = 16384 and TB0CCR1 = 1638. This code uses the polling process and has a 10% duty cycle and 500ms period. This ideally runs at 2Hz but our actuall measured values were slightly different. The measured values were 
duty cycle : 9.998%
Period : 499.81ms
Frequency : 2.0007Hz
Calculation for duty cycle: 500 * 32 = 16384 and this becomes the period, then we found 10 of this which ended up being 1638.

Question 3: For this code we chose to use the SM clock again to create the PWM signal. The period is set by setting TB0CCR0 = 8192 and keeping TB0CCR1 = 1638. This code gives the PWM signal a duty cycle of 20% and a period of 250ms. 
	        Calculated	Measured
Duty Cycle	20%	     19.995%
Period	    250ms  	 249.92ms
Frequency	  4Hz	     4.0012Hz
Calculation. We dived the period from the initial code by 2 since 250ms is half of 500ms. Then we just left the time code for the duty cycle the same since the period was half as long making thwe duty cycle 20% now.





