public class LevelApp {
    
    // Levels enum declaration
    public enum Levels {LOW, MED, HIGH}
    
    public String directions(Levels level)
    {
        // Using a switch statement to return the correct string based on level
        switch (level) {
            case LOW:
                return "Down";
            case MED:
                return "Stay";
            case HIGH:
                return "Up";
            default:
                return "?";            
        }
    }
    
    public static void main(String[] args)
    {
        LevelApp la = new LevelApp();
        
        System.out.println(la.directions(Levels.LOW));
        System.out.println(la.directions(Levels.MED));
        System.out.println(la.directions(Levels.HIGH));
    }
}
