# DistribuidoraTuppers
import java.util.Scanner;

public class PruebaEmpresaTuppers {

	public static void main(String[]args) {

		String	nombreEmpresa;
		
		double costoUnitario;
		
		int cantidadProductos;
		
		
		double precioDeVenta;
		final double IVA = 0.12;
		
	     
		 Scanner entrada = new Scanner(System.in);
		 
		 System.out.println("Introduzca el nombre de su empresa:");
		 nombreEmpresa = entrada.next();
		 System.out.println("Introduce costo por unidad:");
		 costoUnitario =entrada.nextDouble();
		 
		 System.out.println("Introduce el precio de venta:");
		 precioDeVenta = entrada.nextDouble();
		 
		 System.out.println("Introduce la cantidad de productos");
		 cantidadProductos = entrada.nextInt();
		 
		 double totalPorUnidadIVA=precioDeVenta*IVA;
		 double totalAPagar = costoUnitario*cantidadProductos;
		 
		 System.out.println(nombreEmpresa);
		 System.out.println("-"+"Costo por unidad:Q"+costoUnitario);
		 System.out.println("-"+"Cantidad de productos:"+cantidadProductos);
		 System.out.println("----------------------------------------------------------");
		 System.out.println("-"+"Total:Q"+totalAPagar);
		 
		 System.out.println("-"+"Precio de venta:Q"+precioDeVenta);
		 System.out.println("-"+"Impuesto establecido :"+  IVA);
		 System.out.println("-"+"Impuesto por unidad: Q"+totalPorUnidadIVA);
		 
		 System.out.println("----------------------------------------------------------");
		 
		 
		 System.out.println("----------------------------------------------------------");
		 
		 int cantidadProductoVendido;
		 System.out.println("Introduzca la cantidad de productos vendidos:");
		 cantidadProductoVendido = entrada.nextInt();
		 
		 
		 double descuento=0;
		 double descuento1=10;
		 double descuento2=20;
		 double descuento3 =25;
		  if(cantidadProductoVendido>=20) {
			descuento=descuento1;
		 }
		 else if(cantidadProductoVendido>=40) {
			 descuento=descuento2;
		 }
		 else if(cantidadProductoVendido>=60)
		 {
			 descuento=descuento3;
		 }
			 
		 double totalcobradoSinDescuento = cantidadProductoVendido*precioDeVenta;
		 double totalConDescuento = totalcobradoSinDescuento-(totalcobradoSinDescuento*descuento/100);
		 double impuestosADeclarar= totalConDescuento+IVA;
		 double tipoDeDescuento=8.5;
		 double ganancias = totalcobradoSinDescuento -(cantidadProductoVendido);
		 
		
		 System.out.println("");
		 System.out.println("------------------------------------");
		 System.out.println("-"+"Cantidad vendida:" +cantidadProductoVendido);
		 System.out.println("-"+"Total sin descuento:Q"+totalcobradoSinDescuento);
		 System.out.println("-"+"Total con descuento:Q"+totalConDescuento);
		 System.out.println("-"+"IVA a declarar:Q"+impuestosADeclarar);
		 System.out.println("-"+"Tipo de descuento:Q"+tipoDeDescuento);
		 System.out.println("-"+"Ganancia: Q"+ganancias);
	}
}

Este pequeño programa tiene la funcion de atender las necesidades de la venta de tuppers,nos dice la cantidad vendida, el IVA, los descuentos,, total, precio de venta y algunas funciones mas lo que nos pide el cliente 

• Costo unitario del producto

• Cantidad de producto solicitado

• Total del costo a pagar por la cantidad del producto

• Precio de venta al público por unidad

• IVA

• Total del IVA por unidad

• Cantidad de unidades a vender

• Total a cobrar sin descuento

• Total a cobrar con el descuento

• Total del IVA sobre el cobro final

• Indicar el tipo de descuento que se realizó (ninguno, 10%, 15% o 25%)

• Ganancias obtenidas por la venta


