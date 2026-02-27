import java.util.Scanner;

public class Mini_cal {
    
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Main.main(args);
        System.out.println("Que voulez vous faire?");
        System.out.println("1- Addition");
        System.out.println("2- Soustraction");
        System.out.println("3- Multiplication");
        System.out.println("4- Division");
        int choix = scanner.nextInt();
        System.out.print("Entrer a:");
        int a = scanner.nextInt();
        System.out.print("Entrer b:");
        int b = scanner.nextInt();
        switch (choix) {
            case 1:
                System.out.println("Résultat: " + (a + b));
                break;
            case 2:
                System.out.println("Résultat: " + (a - b));
                break;
            case 3:
                System.out.println("Résultat: " + (a * b));
                break;
            case 4:
                if (b != 0) {
                    System.out.println("Résultat: " + (a / b));
                } else {
                    System.out.println("Division par zéro impossible.");
                }
                break;
            default:
                System.out.println("Choix invalide.");
                break;
            }
            if (choix==1){
                System.out.println("Résultat: " + (a + b));
            }
            else if(choix==2){
                System.out.println("Résultat: " + (a - b));
            }
            else if(choix==3){
                System.out.println("Résultat: " + (a * b));
            }
            else if(choix==4){
                if(b!=0){
                    System.out.println("Résultat: " + (a / b));
                }
                else{
                    System.out.println("Division par zéro impossible.");
                }
            }
            else{
                System.out.println("Choix invalide.");
            }

        }
    }


