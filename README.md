# 33.-Run-time-polymorphism-
package vehicletest;
class vehicle {
    public void start() {
        System.out.println("Vehicle is starting");
    }
}
class car extends vehicle {
    @Override
    public void start() {
        System.out.println("Car is starting with key");
    }
}
class motorcycle extends vehicle {
    @Override
    public void start() {
        System.out.println("Motorcycle is starting with a kick");
    }
}
public class VehicleTest {
    public static void main(String[] args) {
        vehicle v1=new vehicle();
  vehicle v2=new car();
  vehicle v3=new motorcycle();
  v1.start();
  v2.start();
  v3.start();
  
    }
    
}
output
Vehicle is starting
Car is starting with key
Vehicle is starting
