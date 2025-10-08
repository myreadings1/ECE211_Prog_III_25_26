### Q1
- Calculating the weight of a box gives us the following program.
```
/* Computes the dimensional weight of a box from input provided by the user */
#include <stdio.h>
int main(void)
{
int height, length, width, volume, weight;
printf("Enter height of box: ");
scanf("%d", &height);
printf("Enter length of box: ");
scanf("%d", &length);
printf("Enter width of box: ");
scanf("%d", &width);
volume = height * length * width;
weight = (volume + 165) / 166;
printf("Volume (cubic inches): %d\n", volume);
printf("Dimensional weight (pounds): %d\n", weight);
return 0;
}
```
- The output of the program has the following appearance (input entered by the user is underlined):

```
Enter height of box: 8
Enter length of box: 12
Enter width of box: 10
Volume (cubic inches): 960
Dimensional weight (pounds): 6
```
#############################################
### Q2

```
/* Converts a Fahrenheit temperature to Celsius */
#include <stdio.h>
#define FREEZING_PT 32.0f
#define SCALE_FACTOR (5.0f / 9.0f)
int main(void)
{
float fahrenheit, celsius;
printf("Enter Fahrenheit temperature: ");
scanf("%f", &fahrenheit);
celsius = (fahrenheit - FREEZING_PT) * SCALE_FACTOR;
printf("Celsius equivalent: %.1f\n", celsius);
return 0;
}
```
The statement
```
celsius = (fahrenheit - FREEZING_PT) * SCALE_FACTOR;
```
#############################################
### Q3

```
Try all the exercises on pages (33-35) of the reference book.
```


#############################################
### Q4

```
Try all the exercises on pages (49-51) of the reference book.
```

#############################################
### Q5

```
Try all the exercises on pages (68-72) of the reference book.
```

#############################################
### Q6

```
Try all the exercises on pages (93-97) of the reference book.
```

#############################################
### Q7

```
Try all the exercises on pages (121-124) of the reference book.
```
