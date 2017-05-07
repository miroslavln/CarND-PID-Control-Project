Initially I started experimenting with different P values.
I started with 0.5 initially but the car quickly started wobbling and leaving the pavement.
I started decreasing the value and that produced better results on the straight portion of the road but when the car
reached the first turns it was leaving the pavement again.
I settled on 0.15 and started tuning the D parameter as it is supposed to smooth the turns and decrease the wobbling.
I tried with 0.3 and kept increasing until the car was making the turns correctly which ended up being the value of 3.0.

I tried experimenting with the I parameter which is controlling the bias but it had no effect of improving the performance
so I left it at 0.

I also created a throttle PID controller which is controlling the speed. I chose the acceleration parameters based on a desired speed
which I chose to be 50 mph I tried using a higher speed but the steering controller could not handle it.
