# Dart Programming
> 
```
import 'dart:math';

void main() {

		var n = 0;

		print("The number of rabbits increases as:\n");

		for (int years = 0; years <= 10; years++) {

			n = (2 * pow(e, log(15) * years)).round().toInt();

			print("After $years years:\t $n animals");

	}
}

int calculateRabbits(){
	retur 
}

```
> Function
```
import 'dart:math';

int rabbitCount = 0;
const int NO_YEARS = 10;
const int GROWTH_FACTOR = 15;

void main() {

  print("The number of rabbits increases as:\n");

  for (int years = 0; years <= NO_YEARS; years++) {
    rabbitCount = calculateRabbits(years);
    print("After $years years:\t $rabbitCount animals");
  }
  
}

int calculateRabbits(int years) {
  return (2 * pow(e, log(GROWTH_FACTOR) * years)).round().toInt();
}
```