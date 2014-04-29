beh_gui
=======
package javaapplication2;
import javax.swing.JFrame;
import javax.swing.JButton;
import java.awt.GridLayout;


public class JavaApplication2 {
   public class ButtonGrid {
          NewJFrame nj = new NewJFrame();
          JButton[][] grid;
     public ButtonGrid (int width, int length){
         nj.setLayout(new GridLayout(width,length));
         grid=new JButton[width][length];
         for(int y=0;y<length;y++){
             for (int x=0;x<width; x++){
                 grid[x][y]=new JButton("("+x+","+y+")");
                 nj.add(grid[x][y]);
             }
         }
         nj.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
         nj.pack();
         nj.setVisible(true);
             }
}
  
    public static void main(String[] args) {
       ButtonGrid buttonGrid;
       buttonGrid = new ButtonGrid(3,3);

    }
    
}
