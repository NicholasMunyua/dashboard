# login form


import java.awt.Color;
import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JPasswordField;
import javax.swing.JTextField;


public class LoginForm {
    
    JFrame frame;//frame
    JTextField field;//to get username
    JPasswordField p;//field for password
    JLabel l;//to print on frame
    JButton button;
    
    LoginForm(){
        
        frame = new JFrame("login form");//initializing frame.argument passed to apper as title
        frame.setSize(500,200);
        frame.setLocation(300, 200);
        frame.getContentPane().setBackground(Color.red);
        frame.setLayout(null);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);//program exit when user clicks close
        
        l= new JLabel("Enter Username");
        l.setLocation(10,10);
        l.setSize(l.getPreferredSize());
        frame.add(l);
        
        field= new JTextField();
        field.setColumns(15);
        field.setSize(field.getPreferredSize());
        field.setLocation(150,10);
        field.setToolTipText("Enter Username");
        frame.add(field);
        
        l= new JLabel("Enter Password");
        l.setLocation(10,40);
        l.setSize(l.getPreferredSize());
        frame.add(l);
        
        p= new JPasswordField();
        p.setColumns(15);
        p.setSize(p.getPreferredSize());
        
        p.setLocation(150,40);
        p.setToolTipText("Enter Password");
        frame.add(p);
        
        JButton b = new JButton("OK");
        b.setSize(b.getPreferredSize());
        b.setLocation(150,80);
        frame.add(b);
        
        frame.setVisible(true);//to make it visible
    }//ending of constructor
    public static void main(String[] args) {
        
        LoginForm loginForm = new LoginForm();
    }
    
}
