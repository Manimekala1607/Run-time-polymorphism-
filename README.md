# Run-time-polymorphism-
package run.time.polymorphism;
class animal{
    void sound(){
        System.out.println("animal makes a sound");
    }
}
class dog extends animal{
    @Override
    void sound(){
        System.out.println("dog barks");
    }
}
class cat extends animal{
    @Override
    void sound(){
        System.out.println("cat meows");
    }
}  
    
public class RunTimePolymorphism {
    public static void main(String[] args) {
        // TODO code application logic here
        animal animal;
        animal=new dog();
        animal.sound();
        animal=new cat();
        animal.sound();
    }
    
}

output:
dog barks
cat meows
BUILD SUCCESSFUL (total time: 0 seconds)
