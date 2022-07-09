- 👋 Hi, I’m @mdh97565
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
mdh97565/mdh97565 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import java.util.Scanner;

class student{
    String sub;
    int number;
    double cGpa;
    double total=0;

  void displayinfo(){

        if (number>=80 && number<=100){
         cGpa=4.00;
            System.out.println(sub+" Grade A+ and CGPA "+cGpa);
        }
        else if(number>=75&& number<=79) {
            cGpa = 3.75;
            System.out.println(sub + " Grade A and CGPA " + cGpa);
        }
        else if (number>=70&&number<=74){
             cGpa=3.5;
            System.out.println(sub+" Grade A- and CGPA "+cGpa);
        }
        else if (number>=65&&number<=69){
             cGpa =3.25;
            System.out.println(sub +" Grade B+ and CGPA "+cGpa);
        }
        else if(number>=60&& number<=64){
             cGpa= 3.00;
            System.out.println(sub+ " Grade B and CGPA "+cGpa);
        } else if (number>=55&&number<=59) {
             cGpa=2.75;
            System.out.println(sub+ " Grade B- and CGPA "+cGpa);
        }
        else if (number>=50&& number<=54){
            cGpa=2.50;
            System.out.println(sub+" Grade C+ and CGPA "+cGpa);
        }
        else if (number>=45&&number<=49){
             cGpa=2.25;
            System.out.println(sub+" Grade C and CGPA "+cGpa);
        }
        else if (number>=40&&number<=44){
             cGpa=2.00;
            System.out.println(sub+" Grade D and CGPA "+cGpa);
        }
        else if (number>=0&&number<=39){
         cGpa=0.00;
            System.out.println(sub+" Fail");
        }


    }

}

public class numbercgpa {



    public static void main(String[] args) {

        int subjectcoun;
        double sum=0;



        Scanner sc= new Scanner(System.in);
        student student1 = new student();

        System.out.println("How many subject ");
         subjectcoun=sc.nextInt();
        for (int i =1;i<=subjectcoun;i++) {

            System.out.println("Enter your subject name");
            student1.sub = sc.next();
            System.out.println("Enter your " + student1.sub + " mark");
            student1.number = sc.nextInt();
            student1.displayinfo();
            double a =student1.cGpa;
            sum+=a;

        }
        System.out.println("Total Grade point "+sum);
        System.out.println("CGPA= "+sum/subjectcoun);

    }

    }
