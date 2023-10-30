public class DatosPersonalesConAprobacionYExperiencia {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Solicitar aprobación del usuario
        System.out.print("¿Acepta el uso de sus datos personales? (Sí/No): ");
        String aprobacion = scanner.nextLine();

        if (aprobacion.equalsIgnoreCase("Sí") || aprobacion.equalsIgnoreCase("si")) {
            
            // Crear un array para almacenar datos personales
            String[] datosPersonales = new String[4];

            // Solicitar datos personales al usuario
            System.out.println("Por favor, ingrese sus datos personales:");
            System.out.print("Nombre: ");
            datosPersonales[0] = scanner.nextLine();

            System.out.print("Apellido: ");
            datosPersonales[1] = scanner.nextLine();

            System.out.print("Edad: ");
            datosPersonales[2] = scanner.nextLine();

            System.out.print("Dirección: ");
            datosPersonales[3] = scanner.nextLine();

            // Mostrar los datos personales ingresados
            System.out.println("Datos personales ingresados:");
            System.out.println("Nombre: " + datosPersonales[0]);
            System.out.println("Apellido: " + datosPersonales[1]);
            System.out.println("Edad: " + datosPersonales[2]);
            System.out.println("Dirección: " + datosPersonales[3]);

            // Solicitar experiencia personal al usuario
            System.out.println("\nPor favor, comparte tu experiencia con nosotros:");
            String experienciaPersonal = scanner.nextLine();
            System.out.println("Gracias por compartir tu experiencia con nosostros!");
        } else {
            System.out.println("No se aceptó el uso de datos personales.");
        }
          
        // Cierra el scanner
        scanner.close();
    }
}
