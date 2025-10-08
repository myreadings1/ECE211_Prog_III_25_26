### Q1
- A volume of 166 would give a weight of 331/166, or 1, while a volume of 167 would yield 332/166, or 2. Calculating the weight in this fashion gives us the following program.
```
/* Computes the dimensional weight of a 12" x 10" x 8" box */
#include <stdio.h>
int main(void)
{
int height, length, width, volume, weight;
height = 8;
length = 12;
width = 10;
volume = height * length * width;
weight = (volume + 165) / 166;
printf("Dimensions: %dx%dx%d\n", length, width, height);
printf("Volume (cubic inches): %d\n", volume);
printf("Dimensional weight (pounds): %d\n", weight);
return 0;
}
```
- The output of the program is
```
Dimensions: 12x10x8
Volume (cubic inches): 960
Dimensional weight (pounds): 6
```
#############################################
### Q2
