# I-know-Your-Birthday
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package Message.pack;

/**
 *
 * @author BRIGHT
 */

import javax.swing.JOptionPane;

public class Prank {
    public static void main(String []args){
        int counter = 0
        String set1 = 
                "\n1 3 5 7\n" +
                "9 11 13 15\n" +
                "17 19 21 23\n" +
                "25 27 29 31";
        String set2 = 
                "\n2 3 6 7\n" +
                "10 11 14 15\n" + 
                "18 19 22 23\n" + 
                "26 27 30 31";
        String set3 = 
                "\n4 5 6 7\n" +
                "12 13 14 15\n" + 
                "20 21 22 23\n" + 
                "28 29 30 31";
        String set4 = 
                "\n8 9 10 11\n" + 
                "12 13 14 15\n" + 
                "24 25 26 27\n" + 
                "28 29 30 31";
        String set5 = 
                "\n16 17 18 19\n" + 
                "20 21 22 23\n" + 
                "24 25 26 27\n" + 
                "28 29 30 31";
        String a = JOptionPane.showInputDialog(null,"What is your birth month");
        int answer = 
        JOptionPane.showConfirmDialog(null,
                "Is your date in this set : " +set1);
        if (answer == JOptionPane.YES_OPTION) {
            counter += 1;    
        }
        answer = 
        JOptionPane.showConfirmDialog(null,
                "Is your date in this set : " +
                set2);
        if (answer == JOptionPane.YES_OPTION) {
            counter += 2;
        }
        answer =         
        JOptionPane.showConfirmDialog(null,
                "Is your date in this set : " +
                set3);
        if (answer == JOptionPane.YES_OPTION) {
            counter += 4;
        }
        answer =         
        JOptionPane.showConfirmDialog(null,
                "Is your date in this set : " +
                set4);
        if (answer == JOptionPane.YES_OPTION){
            counter += 8;
        }
        answer =         
        JOptionPane.showConfirmDialog(null,
                "Is your date in this set : " + 
                set5);
        if (answer == JOptionPane.YES_OPTION) {
            counter += 16;
        }
        JOptionPane.showMessageDialog(null,
                "Your birthday is the " +
                        counter + "th of " + a  );
        System.out.println("Thanks for playing Louis Game.");
    }    
}
