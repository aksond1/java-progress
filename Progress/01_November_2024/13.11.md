I tried to use the code below to count the time in the Statistics, but in the end I decided that it would be better without time shifting
```java
import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        System.out.println("Write spent time: ");
        double time = sc.nextDouble();
        
        int hours = (int) time;
        double fractional = time - hours;
        
        int minutes = (int) Math.round(fractional * 60);
        
        System.out.println("New time: " + hours + "." + minutes);
    }
}
```
