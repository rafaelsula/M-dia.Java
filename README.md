import java.util.Scanner;

public class Media {

    public static void main(String args []) {
        Scanner teclado = new Scanner(System.in);
        float nota1, nota2, nota3, media;
        
        System.out.println("Informe as notas: ");
        
        System.out.print("\n\tNota1: ");
        nota1 = teclado.nextFloat();
        
        System.out.print("\n\tNota2: ");
        nota2 = teclado.nextFloat();
        
        System.out.print("\n\tNota3: ");
        nota3 = teclado.nextFloat();
        
        media = calculamedia(nota1, nota2, nota3);
        
        System.out.println("\n\tA média é " + media);
        
        
    }
    
    public static float calculamedia (float n1, float n2, float n3) {
        float media;
        
        if (n1 < n2 && n1 < n3) {
            media = (n2 + n3) / 2;
        }
        else if (n2 < n3) {
            media = (n1 + n3) / 2;
        }else {
            media = ( n1 + n2) /2;
        }
        return media;
        
    }
}
