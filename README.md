# Java_arrays_ordenamiento
2(Ejercicio_ metodo_ burbuja)
MARIA ALEJANDRA ROMERO MENDEZ
DAVID ESTEBAN RODRIGUEZ PINEDA
descargar 
De: MARIA ALEJANDRA ROMERO MENDEZ
Enviado: martes, 21 de mayo de 2019 19:34
Para: JHONATHAN ELIAS RUIZ BUITRAGO
Asunto: 2

package metodosdeordenamiento;

import java.applet.Applet;
import java.awt.Graphics;


public class Ejercicio4 extends Applet{
    
    
    int [] x =  new int[10];
    
    public Ejercicio4 (){
         for (int i = 0; i < 10; i++) 
             x[i] = 12-i;
         
     }
     

    void f(int[] a) {
        int i, j;
        for (i = 0; i < 9; i++) {
            for (j = i + 1; j < 10; j++) {
                a[i] = a[i] + a[j];
                a[j] = a[i] - a[j];
                a[i] = a[i] - a[j];
            }
        }
    }
    
    
     public void paint(Graphics g)
     {
         for (int j=0; j<10; j++)
         g.drawString(" "+x[j],20 + j*20,10);
         f(x);
         for (int j = 0; j < 10; j++)
         g.drawString(" " + x[j],20 + j*20, 40);
         
     }
    
}
