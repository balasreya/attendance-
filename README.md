# attendance-
import java.util.*;
interface student
{
    void getvalue();
}
interface department
{
    void getattendence();
}
class exam implements student,department
{
    int ro_no,attendence;
    String sname,class_n;
    Scanner s=new Scanner(System.in);
    void getvalue()
    {
        System.out.println("enter the name");
        sname=s.nextLine();
        System.out.println("enter the no");
        ro_no=s.nextInt();
        System.out.println("enter the class");
        class_n=s.nextLine();
    }
    void getattendence()
    {
        System.out.println("enter the attendence");
        attendence=s.nextInt();
    }
    void calattendence()
    {
        System.out.println("enter the name"+sname);
        System.out.println("enter the no"+ro_no);
        System.out.println("enter the class"+class_n);
        System.out.println("enter the attendence"+attendence);
    }
    void attendence()
    {
        if(attendence<75)
        {
            System.out.println("true");
        }
        else
        {
            System.out.println("false");
        }
    }
}
    class Main
    {
        public static void main(String[] args)
        {
            int i;
            Scanner s=new Scanner(System.in);
            System.out.println("enter the n");
            int n=s.nextInt();
            student o[]=new student[n];
            for(i=0;i<n;i++)
            {
                o[i]=new student();
                o[i].getvalue();
                o[i].getattendence();
                o[i].calattendence();
                o[i].attendence();
            }
        }
    }
    
