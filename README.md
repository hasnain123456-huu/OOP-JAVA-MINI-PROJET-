# OOP-JAVA-MINI-PROJET-
class Patient {

    private String name;
    private int age;

    Patient(String n,int a) {
        name=n;
        age=a;
    }

    public void show() {
        System.out.println(
                name+" "+age
        );
    }
}

class Doctor {

    private String doctorName;

    Doctor(String d) {
        doctorName=d;
    }

    public void treat(Patient p) {
        System.out.println(
                doctorName +
                " treated patient"
        );
    }
}

public class Main {

    public static void main(String[] args) {

        Patient p1 =
                new Patient(
                        "Ali",
                        20
                );

        Doctor d1 =
                new Doctor(
                        "Ahmed"
                );

        p1.show();

        d1.treat(p1);
    }
}