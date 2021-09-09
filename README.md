package horasextras;

import java.util.Scanner;

public class HorasExtras {

    public static void main(String[] args) {
     Scanner entrada= new Scanner(System.in);
    long horasTrabajadas;
    long pagoxhora;
    long salario;
    String nombre;
    
    System.out.print("\t\tEmpresa Conductores A.C \n");
    System.out.print("\t\tSistema de pago Horas extras \n");
    
    System.out.print("Nombre del conductor: ");
    nombre = entrada.nextLine();
    System.out.print("Ingrese las horas trabajadas: ");
    horasTrabajadas=entrada.nextLong();
    System.out.print("Ingrese el pago por horas: ");
    pagoxhora=entrada.nextLong();
    
    if(horasTrabajadas<=40){
    pagoxhora=pagoxhora;
    }
    else{
    pagoxhora= (pagoxhora/2)+pagoxhora;
    }
    salario= horasTrabajadas*pagoxhora;
    System.out.println("El salario es de: "+salario);
}

}
