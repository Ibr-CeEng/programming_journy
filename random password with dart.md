## Generat a random password that consist of numbers 

```dart
import 'dart:math';


String genreatPassword (len){
   String password ='';
   for(int i =0;i<len;i++){
       int randomIndex = Random().nextInt(10);
       password += randomIndex.toString() ;
   }
  return password;
}

void main() {
  int len = 5;
  print("Random Password of legth: ${genreatPassword(len)}");
}
