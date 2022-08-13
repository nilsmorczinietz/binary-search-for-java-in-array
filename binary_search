import java.util.*;
import javax.swing.JOptionPane;

public class binary_search {
    public static void main(String[] args) throws InterruptedException {

        String ArrayGroesse = JOptionPane.showInputDialog("How big do you want your array to be?");
        int arraygroesse = Integer.parseInt(ArrayGroesse);
        int [] Zahlen = new int[arraygroesse];

        String ArrayAbstand = JOptionPane.showInputDialog("How big should the distance between the numbers be?");
        int arrayabstand = Integer.parseInt(ArrayAbstand);

        int temp = 1;
        for(int i=0; i<Zahlen.length; i++){
            Zahlen[i]=temp;
            temp = temp+arrayabstand;
        }

        String GesuchteZahl = JOptionPane.showInputDialog("What number are you looking for?");
        int gesuchtezahl = Integer.parseInt(GesuchteZahl);

        int min = 0;
        int max = Zahlen.length;
        int mid = max/2;

        while(Zahlen[mid] != gesuchtezahl){
            if(gesuchtezahl>Zahlen[mid]){
                min = mid+1;
                max = max;
                mid = (min+max)/2;
            }
            if(gesuchtezahl<Zahlen[mid]){
                min = min;
                max = mid-1;
                mid = max/2;
            }
        }
        JOptionPane.showMessageDialog(null,"The number  "+gesuchtezahl+" was found at position "+(mid)+" !");
    }
}
