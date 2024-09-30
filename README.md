package encapsulando;
import java.util.Scanner;
public class Prt2_carro {
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		
		Carro carro = new Carro();
		
		System.out.print("Digite modelo do carro:");
		carro.setModelo(scanner.nextLine());
		
		System.out.print("Digite a cor do carro:");
		carro.setCor(scanner.nextLine());
		
		System.out.print("Digite o Ano:");
		carro.setAno(scanner.nextInt());
		
		System.out.println("Modelo:" + carro.getModelo());
		System.out.println("Cor:" + carro.getCor());
		System.out.println("Ano:" + carro.getAno());
	
	}

}

package encapsulando;

public class Carro {
	private String modelo;
	private String cor;
	private int ano;
	
	
	public void setModelo(String modelo) {
		this.modelo = modelo;
	}
	public String getModelo() {
		return modelo;
	}
	public void setCor(String cor) {
		this.cor = cor;
	}
	public String getCor() {
		return cor;
	}
	public void setAno(int ano) {
		this.ano = ano;
	}
	public int getAno() {
		return ano;
	}
}
