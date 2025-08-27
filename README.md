package MyPackage;
import java.awt.*;
import javax.swing.*;
public class Main {

    public static void main(String[] args) {
    
        String input = JOptionPane.showInputDialog(null, "Enter the number of students:", "Student Count", JOptionPane.QUESTION_MESSAGE);
        
        JPanel panel1 = new JPanel(new GridLayout (3, 2));
        
        JLabel nameLabel = new JLabel("Student Name: "); 
        JLabel studentIDLabel = new JLabel("Student ID: ");
        JLabel courseCodeLabel = new JLabel("Student Course: ");
        
        JTextField nameTextField = new JTextField();
        JTextField studentIDTextField = new JTextField();
        JTextField courseCodeTextField = new JTextField();
        
        panel1.add(nameLabel);
        panel1.add(nameTextField);
        panel1.add(studentIDLabel);
        panel1.add(studentIDTextField);
        panel1.add(courseCodeLabel);
        panel1.add(courseCodeTextField);
        
        JOptionPane.showMessageDialog(null, panel1, "Enter Student " + (i + 1) + " Information", JOptionPane.QUESTION_MESSAGE);

        Student student = new Student(nameTextField, studentIDTextField, courseCodeTextField);
        JOption
        
        JLabel nameLabel = new JLabel("Student Name: "); 
        JLabel studentIDLabel = new JLabel("Student ID: ");
        JLabel courseCodeLabel = new JLabel("Student Course: ");
        
        JTextField nameTextField = new JTextField();
        JTextField studentIDTextField = new JTextField();
        JTextField courseCodeTextField = new JTextField();
        
        panel1.add(nameLabel);
        panel1.add(nameTextField);
        panel1.add(studentIDLabel);
        panel1.add(studentIDTextField);
        panel1.add(courseCodeLabel);
        panel1.add(courseCodeTextField);
        
    }
}







package MyPackage;

public class Student {
    private String name;
    private String studentID;
    private String courseCode;

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getstudentID() {
        return studentID;
    }

    public void setstudentID(String studentID) {
        this.studentID = studentID;
    }

    public String getCourseCode() {
        return courseCode;
    }

    public void setCourseCode(String courseCode) {
        this.courseCode = courseCode;
    }
    
    @Override
    public String toString(){
        return "Name: " + name + "\n" + "ID Number: " + studentID + "\n" +
                "Course Code: " + courseCode;
    }
}
