# DistribuidoraTuppers
import java.util.Scanner;
public class Reparto_tuppers {

	public static void main(String[] args) {
	
		String	nombreEmpresa ="Distribuidora Tupperware";
		
		double costoUnitario=45;
		int cantidadProductos=200;
		
		double totalAPagar = costoUnitario*cantidadProductos;
		double precioDeVenta=50;
		final double IVA = 0.12;
		 double totalPorUnidadIVA=precioDeVenta*IVA;
		
		 Scanner entrada = new Scanner(System.in);
		
		 System.out.println("Costo por unidad:Q"+costoUnitario);
		 System.out.println("Cantidad de productos:Q"+cantidadProductos);
		 System.out.println("------------------");
		 System.out.println("Total:Q"+totalAPagar);
		 
		 System.out.println("Venderse a :Q"+precioDeVenta);
		 System.out.println("Impuesto establecido :"+  IVA);
		 System.out.println("Impuesto por unidad: Q"+totalPorUnidadIVA);
		 
		 int cantidadProductoVendido = 60;
		 double totalcobradoSinDescuento = cantidadProductoVendido*precioDeVenta;
		 double totalConDescuento = totalcobradoSinDescuento-0.5;
		 double impuestosADeclarar= totalConDescuento+IVA;
		 double tipoDeDescuento=8.5;
		 double ganancias = totalcobradoSinDescuento -(cantidadProductoVendido);
		 
		 System.out.println("");
		 System.out.println("------------------------------------");
		 System.out.println("Cantidad vendida:" +cantidadProductoVendido);
		 System.out.println("Total sin descuento:Q"+totalcobradoSinDescuento);
		 System.out.println("IVA a declarar:Q"+impuestosADeclarar);
		 System.out.println(" Tipo de descuento:Q"+tipoDeDescuento);
		 System.out.println("Ganancia: Q"+ganancias);
		 
		 
	}

}
Este pequeño programa tiene la funcion de atender las necesidades de la venta de tuppers,nos dice la cantidad vendida, el IVA, los descuentos,, total, precio de venta y algunas funciones mas

